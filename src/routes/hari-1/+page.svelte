<script>
  import Button from "$lib/Button.svelte";
  import Field from "$lib/Field.svelte";
  import Selection from "../../lib/Selection.svelte";
</script>

<!-- <Button /> -->
<div class="flex flex-col mx-auto font-bold text-white text-center my-10">
  <!-- Silahkan masuk melalui QR Code yang disediakan :) -->

  <br />
  <div class="bg-[#00933B] rounded-xl px-3 py-6 space-y-4">
    <Field id="123" name="Nama" placeholder="Masukkan nama" />
    <Field id="234" name="Alamat" placeholder="Masukkan alamat" />
    <Selection name="Apakah Anda Memiliki KTAM" />
  </div>
  <Button>Selanjutnya</Button>
</div>
