# Text area
Text fields let users enter and edit text.

Text fields allow users to enter text into a UI. They typically appear in forms and dialogs.

![](./../../_media/examples/textarea/textarea.gif)

## Basic Textarea
The TextField wrapper component is a complete form control including a label, input, and help text. It comes with three variants: outlined (default), filled, and standard.

## Usage
```Blade
<x-input.textarea>
  <x-slot:type>email</x-slot:type>
  <x-slot:placeholder>placeholder</x-slot:placeholder>
  <x-slot:labelFor>Label for slot</x-slot:labelFor>
  <x-slot:label>label slot</x-slot:label>
</x-input.textarea>
```

## Structure
```blade
<div class="contact-form-container-right ">
    <div class="contact-form-textinput-container group">
        <textarea class="contact-form-textarea peer" type="{{$type}}" required name="{{$name}}" placeholder="{{$placeholder}}"></textarea>
        <label for="{{$labelFor}}" class="contact-form-text-input-label">
            {{$label}}
        </label>
    </div>
</div>
```
