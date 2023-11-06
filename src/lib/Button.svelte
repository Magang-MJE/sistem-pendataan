<script>
  import { bgColor, primaryColor, accentColor } from "./colors.js";
  export let onclick;
  export let type = "submit";
</script>

<button
  {type}
  on:click={onclick}
  class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
>
  <!-- Button -->
  <slot />
</button>
