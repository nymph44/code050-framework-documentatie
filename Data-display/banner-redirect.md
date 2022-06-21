# Banner redirect
![](../_media/examples/banner-redirect/banner.jpg)
### Usage

```blade
 <x-navigation.project-redirect>
    <x-slot:image>URL TO IMAGE</x-slot:image>
    <x-slot:title>Title</x-slot:title>
    Sub text can be placed here and will be display using the $slot tag
</x-navigation.project-redirect>
```

### Structure
```Blade
<div
    style="background:linear-gradient(90deg, rgba(0,0,0,1) 0%, rgba(0,0,0,0.8015581232492998) 47%, rgba(0,0,0,0) 100%), url({{$image}}); background-size: cover;"
    class="project-redirect">
    <div class="project-redirect-container">
        <img class="project-redirect-container-image" src="{{asset('./assets/images/logo/logo-white.svg')}}"
             alt="code050 logo"/>
        <h1 class="project-redirect-container-title">{{$title}}</h1>
        <!--Ondertitel-->
        <p class="project-redirect-container-slot">{{$slot}}</p>
        <div>
            <x-ui.buttons.small.primary>
                <p class="mr-2">{{__('Lees meer')}}</p>
                <i class="fa-solid fa-arrow-right"></i>
            </x-ui.buttons.small.primary>
        </div>
    </div>
</div>
```