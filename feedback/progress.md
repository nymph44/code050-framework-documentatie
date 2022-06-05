# Progress

## Progress scroll bar

> To use the progress bar on scroll, the following script needs to be included.
```.js
<script>
    window.onscroll = function () {
        progressBar()
    };
    function progressBar() {
        var winScroll = document.body.scrollTop || document.documentElement.scrollTop;
        var height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
        var scrolled = (winScroll / height) * 100;
        document.getElementById("myBar").style.width = scrolled + "%";
    }
</script>
```

!> The script will look for an element called myBar using the DOM.

add the folowing HTML in your page

```.html
    <div class="progress-container bg-base-200 dark:bg-stone-900">
        <div class="progress-bar" id="myBar"></div>
    </div>
```