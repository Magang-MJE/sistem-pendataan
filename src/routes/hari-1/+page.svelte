<script>
  import Button from "$lib/Button.svelte";
  import Field from "$lib/Field.svelte";
  import Selection from "../../lib/Selection.svelte";
</script>

<!-- <Button /> -->
<div class="mx-auto font-bold text-white text-center my-10">
  <!-- Silahkan masuk melalui QR Code yang disediakan :) -->

  <a href="/hari-1">(hari 1)</a>
  <a href="/hari-2">(hari 2)</a>
  <a href="/hari-3">(hari 3)</a>

  <br />
  <div class="bg-[#00933B] rounded-xl px-3 py-6 space-y-4">
    <Field id="123" name="Nama" placeholder="Masukkan nama" />
    <Field id="234" name="Alamat" placeholder="Masukkan alamat" />
    <Selection name="Apakah Anda Memiliki KTAM" />
  </div>
  <Button>Selanjutnya</Button>
</div>
