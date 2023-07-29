<script lang="ts">
  export let icon: string;
  export let text: string;
</script>

<button
  class="rounded-full border-solid border-[1px] w-[197px] h-[30px] text-white text-[15px] mb-3"
  ><img src={icon} alt="icon" /> {text}</button
>
