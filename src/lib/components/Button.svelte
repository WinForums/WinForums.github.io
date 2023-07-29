<script lang="ts">
  import clsx from "clsx";

  type buttontypetype = "button" | "submit" | "reset" | undefined;
  export let buttontype: buttontypetype = "button";
  export let text: string;
</script>

<button
  class={clsx(`
  rounded-[20px]
  bg-[#002977]
  text-white
  hover:bg-[#003BAC]
  w-[199px]
  h-[59px]
  box-shadow[0,4px,4px,0,rgba(0,0,0,0.25)]
`)}
>
  {text}
</button>
