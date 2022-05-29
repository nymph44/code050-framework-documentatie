# Cards

## Default
> Default card usage

## Case
> Case card usage

## Service
> Service card usage

## Consult
> parameters
<br>
**$title** - string
<br>
**$slot** - string
---

> To use the buttons inside a Laravel Blade project we add it as following. Inside the tag we pass text as prop to be displayed inside the button.

    <x-cards.consult>
        <x-slot:title>

        // your title

        </x-slot:title>

        // description goes here

    </x-cards.consult>


The buttons are structured as follows:

    <div class="md:w-1/2 pb-8 pr-8 ">
        <div class="border-2 h-48 border-primary rounded-2xl p-4">
            <h1 class="mb-4 font-bold text-xl text-stone-990 dark:text-base-100">{{$title}}</h1>
            <p class="text-lg leading-6 text-stone-990 dark:text-base-200">{{$slot}} </p>
        </div>
    </div>