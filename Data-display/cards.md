# Cards

## Default
![image](./../../_media/examples/cards/project-card.png)
> parameters
<br>
**$image** - string
<br>
**$title** - string
<br>
**$slot** - string

```.html
<card class="max-w-sm flex mx-auto justify-start border-gray-300  border rounded py-2">
    <!-- Image -->
    <div class="w-32">
        {{$image}}
    </div>
    <!-- Description -->
    <div class="w-3/4">
        {{$title}}
        {{$slot}}
    </div>
</card>
```

## Case

> parameters
<br>
**$title** - string
<br>
**$categorie** - string
<br>
**$slot** - string
---

```.html
<card>
    <div class="max-w-sm   relative  rounded overflow-hidden shadow-lg">
        <div class="absolute top-36 z-10 px-6 ">
            <div>
                {{$title}}
            </div>
            <span
                class="inline-block bg-error-content rounded-full px-3 py-1 text-base font-semibold text-gray-700 mr-2 mb-2">
                {{$categorie}}
            </span>
        </div>
        <img class="w-full h-60 object-cover"
             src="https://play-lh.googleusercontent.com/MMBG4AZmpMhSfhF5k7QnFmhvFbaF5ZC_BtEOIKRt9TIkUZjul2lWwPZV75PwTfoSm23-jgMxkroRGA-vkDg"
             alt="Mountain">
        <div class="px-6 py-4">
            {{$slot}}
        </div>
    </div>
</card>
```

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
    <!-- Add multiple features -->
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
```

## Consult
![image](./../../_media/examples/cards/consult.png)
> parameters
<br>
**$title** - string
<br>
**$slot** - string
---

```.html
<div class="md:w-1/2 pb-8 pr-8 ">
    <div class="border-2 h-48 border-primary dark:border-secondary rounded-2xl p-4">
        <h1 class="mb-4 font-bold text-2xl text-primary dark:text-secondary">{{$title}}</h1>
        <p class="text-lg leading-6 text-stone-990 dark:text-base-200">{{$slot}} </p>
    </div>
</div>
```

> To use the buttons inside a Laravel Blade project we add it as following. Inside the tag we pass text as prop to be displayed inside the button.
```.blade
    <x-cards.consult>
        <x-slot:title>

        // your title

        </x-slot:title>

        // description goes here

    </x-cards.consult>
```

The buttons are structured as follows:
```.html
    <div class="md:w-1/2 pb-8 pr-8 ">
        <div class="border-2 h-48 border-primary rounded-2xl p-4">
            <h1 class="mb-4 font-bold text-xl text-stone-990 dark:text-base-100">{{$title}}</h1>
            <p class="text-lg leading-6 text-stone-990 dark:text-base-200">{{$slot}} </p>
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

```.html
<div class="md:w-1/2 pb-8 pr-8 ">
    <div class="border-2 h-48 border-primary dark:border-secondary rounded-2xl p-4">
        <h1 class="mb-4 font-bold text-2xl text-primary dark:text-secondary">{{$title}}</h1>
        <p class="text-lg leading-6 text-stone-990 dark:text-base-200">{{$slot}} </p>
    </div>
</div>
```

> To use the buttons inside a Laravel Blade project we add it as following. Inside the tag we pass text as prop to be displayed inside the button.
```.blade
    <x-cards.consult>
        <x-slot:title>

        // your title

        </x-slot:title>

        // description goes here

    </x-cards.consult>
```

The buttons are structured as follows:
```.html
    <div class="md:w-1/2 pb-8 pr-8 ">
        <div class="border-2 h-48 border-primary rounded-2xl p-4">
            <h1 class="mb-4 font-bold text-xl text-stone-990 dark:text-base-100">{{$title}}</h1>
            <p class="text-lg leading-6 text-stone-990 dark:text-base-200">{{$slot}} </p>
        </div>
    </div>
```