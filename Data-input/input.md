# input
Text fields let users enter and edit text.

![](./../_media/examples/input/input.png)


## Basic TextField
The TextField wrapper component is a complete form control including a label, input, and help text. It comes with three variants: outlined (default), filled, and standard.

## Usage
!> Blade component yet to be implemented!
```blade
<x-input-labeledfield>
  <x-slot:id>name<x-slot:id>
</x-input-labeledfield>
```

## Structure
```blade
<div class="contact-form-textinput-container group">
        <input class="contact-form-textinput peer" type="text" id="{{$id}}" name="{{$id}}"
         placeholder="{{$id}}"/>
    <label for="{{$id}}" class="contact-form-text-input-label  z-13">{{$id}}</label>
</div>
```
