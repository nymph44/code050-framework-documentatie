# input
Text fields let users enter and edit text.

![](./../_media/examples/input/input.png)


## Basic TextField
The TextField wrapper component is a complete form control including a label, input, and help text. It comes with three variants: outlined (default), filled, and standard.

```.html
 <input
    class="placeholder-white dark:placeholder-stone-950 rounded-xl block px-4 w-full text-sm text-base-990 bg-transparent border border-b-2 border-gray-300 appearance-none dark:text-white dark:border-gray-400 dark:focus:border-primary focus:outline-none focus:ring-0 focus:border-primary peer"
    type="text"
    id="placeholder-id"
    name="name"
    placeholder="{{__('placeholder')}}"
/>

<label for="name"
    class="peer-focus:font-medium absolute text-sm text-neutral
        dark:text-base-100 duration-300 transform-translate-y-7
        scale-75 top-2 left-2.5 -z-13 origin-[0]
        peer-focus:left-2.5 peer-focus:px-2.5
        peer-focus:text-primary peer-focus:dark:text-primary
        peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0
        peer-focus:scale-75 peer-focus:-translate-y-4
        bg-white dark:bg-stone-950
        ">
        {{__('name')}}
</label>
```