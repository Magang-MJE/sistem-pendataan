<script>
  import Button from "../lib/Button.svelte";
  import Field from "../lib/Field.svelte";
</script>

<!-- <Button /> -->
<div class="mx-auto font-bold text-white text-center my-10">
  <!-- Silahkan masuk melalui QR Code yang disediakan :) -->

  <a href="/hari-1">(hari 1)</a>
  <a href="/hari-2">(hari 2)</a>
  <a href="/hari-3">(hari 3)</a>

  <Button>hari 1</Button>
  <br />
  <Field id="123" name="Nama" placeholder="isi" />
</div>
