# Cards

## Case
![image](./../../_media/examples/cards/project-card.png)
> parameters
<br>
**$title** - string
<br>
**$categorie** - string
<br>
**$slot** - string
---

```.blade
<div class="project-card">
    <div class="project-card-container">
        <div class="category-span-position">
            <span class="category-span">
                {{$categorie}}
            </span>
        </div>
        <!-- -->
        @if ($style->isNotEmpty())
            <div class="project-card-container-image {{$style}}">
                @else
                    <div class="project-card-container-image">
                        @endif
                        <img class="project-card-container-image-style" src="{{$image}}" alt="">
                    </div>
                    <div class="project-card-content-container">
                        <p class="project-card-content-title">{{$title}}</p>
                        <p class="project-card-content-subtext">{{ substr($slot ?? '', 0,50)}}...</p>
                        <div class="project-card-redirect">
                            <a href="#">
                                <x-ui.buttons.small.alternative-outline>
                                    Website bezoeken
                                </x-ui.buttons.small.alternative-outline>
                            </a>
                        </div>
                    </div>
            </div>
    </div>
</div>


```
<!--
## Service
> parameters
<br>
**$title** - string
<br>
**$price** - integer
<br>
**$slot** - string
---


```.html
<div class="max-w-sm rounded shadow-lg">
    <div class="px-6 py-4">
        <p class="flex pt-2 pb-4 text-medium text-xl justify-center">{{$title}}</p>
        <div class="flex flex-row space-x-1 justify-center items-end pb-4">
            <div class="font-bold text-4xl ">€{{$price}}</div>
            <div class="text-gray-600 text-md">/maand</div>
        </div>
        {{$slot}}
    </div>

    <div class="px-6 pt-4 pb-4">
        <div class="flex flex-row gap-4 pb-4 align-super">
            <i class="fa-solid text-primary text-xl fa-check"></i>
            <p class="text-gray-800 text-base align-middle">
                Feature #1
            </p>
        </div>
    </div>
    <div class="flex justify-center pb-8 px-6">
        <x-ui.buttons.medium.primary class="w-full h-3 text-4xl text-white text-bold">
            Select
        </x-ui.buttons.medium.primary>
    </div>
</div>
``` -->

## Consult
![image](./../../_media/examples/cards/consult.png)
> parameters
<br>
**$title** - string
<br>
**$slot** - string
---

```.blade
<div class="consult-card">
    <div class="consult-card-container">
        <h1 class="consult-card-title">{{$title}}</h1>
        <p class="consult-card-content">{{$slot}} </p>
    </div>
</div>
```


## Explanatory
![image](./../../_media/examples/cards/explanatory.png)
> parameters
<br>
**$title** - string
<br>
**$slot** - string
---

```.blade
<div class="explanatory-card">
    <div class="explanatory-card-content">
        <h3 class="explanatory-card-title">{{$title}}</h3>
        <p class="explanatory-card-sub">{{$slot}}</p>
    </div>
    <div class="inline-block bottom-0">
        <div class="explanatory-card-url">
            <a href="{{$url}}">
                <x-ui.buttons.small.primary>
                    Meer lezen
                </x-ui.buttons.small.primary>
            </a>
        </div>
        <div class="explanatory-card-image">
            {{$image}}
        </div>
    </div>
</div>

```
