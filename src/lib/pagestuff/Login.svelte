<script lang="ts">
  import Button from "../components/Button.svelte";
  import Input from "../components/Input.svelte";
  import SocialButton from "../components/SocialButton.svelte";
</script>

<main>
  <div class="flex items-center justify-center h-screen overflow-hidden">
    <div
      class="bg-black/50 w-[545px] h-[596px] flex flex-col justify-center items-center rounded-xl box-shadow[0,4px,4px,0,rgba(0,0,0,0.25)] text-center center"
    >
      <span class="text-white text-[40px] select-none">Log In</span>
      <span class="text-white/50 text-[15px] select-none pt-8 pb-0.5"
        >Or don’t have an account yet? Sign Up</span
      >
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
      <form class="space-y-0" on:click|preventDefault>
        <Input
          required
          id="email"
          type="email"
          placeholder="Enter your email"
          eclasses="pb-[53px]"
        />
        <Input
          required
          id="password"
          type="password"
          placeholder="Enter your password"
          eclasses="pb-[13px]"
        />
        <Button text="Continue" />
      </form>
      <span class="font-[15px] py-[25px] text-white">or</span>
      <SocialButton icon="Apple" text="Log in with Apple" />
      <SocialButton icon="" text="Log in with Google" />
      <SocialButton icon="" text="Log in with Github" />
    </div>
  </div>
</main>
