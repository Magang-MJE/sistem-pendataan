<script>
  import Field from "./Field.svelte";
  let kondisi = " ";
  export let name = "";
  export let id = "";
  export const placeholder = " ";
</script>

<div class="text-left">
  <label class="flex flex-col">
    <span>
      {name}
    </span>
    <select
      class="bg-[#007E33] border-[#299F59] border-2 rounded-xl py-2 px-3 font-normal placeholder:text-[#78B791]"
      bind:value={kondisi}
      name="ktam"
      required
    >
      <!-- <option value="">Pilih</option> -->
      <option value="true">Iya</option>
      <option value="false">Tidak</option>
    </select>
  </label>
</div>
{#if kondisi == "true"}
  <Field {id} name="No. Anggota" placeholder="Masukkan No. Anggota" />
{/if}
