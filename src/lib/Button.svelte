<script>
  import { bgColor, primaryColor, accentColor } from "./colors.js";
  export let onclick;
</script>

<button
  on:click={onclick}
  class="bg-[#00933B] rounded-xl p-3 text-white border-b-2 border-[#006F2C] font-bold"
>
  <!-- Button -->
  <slot />
</button>
