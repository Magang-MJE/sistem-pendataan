<script>
  export let name = "nama";
  export let placeholder = "isi";
  export let id;
</script>

<div class="text-left">
  <label class="flex flex-col">
    <span>
      {name}
    </span>
    <input
      type="text"
      {id}
      {placeholder}
      class="bg-[#007E33] border-[#299F59] border-2 rounded-xl py-2 px-3 font-normal placeholder:text-[#78B791]"
    />
  </label>
</div>
