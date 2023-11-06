<script>
  import "../app.postcss";
</script>

<div class="bg-[url('./bg.webp')] min-h-screen bg-no-repeat bg-cover">
  <div class="border border-transparent mx-auto max-w-2xl px-5">
    <img src="./logo.png" alt="logo MJE" class="mx-auto w-44 my-5" />
    <slot />
  </div>
</div>
