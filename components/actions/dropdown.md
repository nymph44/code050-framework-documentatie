# Select

Select components are used for collecting user provided information from a list of options.

![image](./../../_media/examples/select/select.png)

---
```blade
<label for="countries" class="block mb-2 text-sm font-medium text-gray-900 dark:text-base-100">
    your label
</label>
<select
    class="border-b-2 border border-gray-300 text-gray-900 text-sm rounded-xl focus:ring-primary focus:border-primary
    block w-full p-2.5 bg-white dark:bg-stone-990 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white
    dark:focus:ring-primary dark:focus:border-primary"
    required
    name="dropdown"
>
    <!-- dropdown options -->
    <option selected disabled>{{__('Select an option')}}</option>
    <option class="rounded-xl">{{__('Diensten')}}</option>
    <option>{{__('Maatwerk applicaties')}}</option>
</select>
```