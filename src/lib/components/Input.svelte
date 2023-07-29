<script lang="ts">
  export let id: string;
  export let type: string = "text";
  export let required: boolean = false;
  export let disabled: boolean = false;
  export let placeholder: string;
  export let eclasses: ClassValue = undefined;
  import clsx, { type ClassValue } from "clsx";
</script>

<div class="pt-0 pb-0 {eclasses}">
  <input
    {id}
    {type}
    autocomplete={id}
    {disabled}
    {placeholder}
    {required}
    class={clsx(
      `
    form-input
    border-0
    w-[431px]
    h-[59px]
    rounded-[20px]
    bg-[#D9D9D9]
    box-shadow[0,4px,4px,0,rgba(0,0,0,0.25)]
    pl-[29px]
    pr-[29px]
    placeholder:text-[#00000040]`,
      disabled && "opacity-50 cursor-default"
    )}
  />
</div>
