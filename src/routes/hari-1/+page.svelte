<script>
  import Button from "$lib/Button.svelte";
  import Field from "$lib/Field.svelte";
  import Selection from "../../lib/Selection.svelte";
</script>

<!-- <Button /> -->
<div class="flex flex-col mx-auto font-bold text-white text-center my-10">
  <!-- Silahkan masuk melalui QR Code yang disediakan :) -->

  <img src="/gmbrmagang.jpg" alt="logo MJE" class="mx-auto w-100 my-5" />

  <a
    href="/gmbrmagang.jpg"
    class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
    download>Download</a
  >

  <a
    href="/"
    class="bg-sky-400 rounded-xl p-3 text-white border-b-2 border-sky-600 font-bold mt-5"
    >Back</a
  >

  <!-- <a
    href="https://forms.gle/baD6bcH9Y9rFb2Lz5"
    class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
    >Hari 2</a
  >
  <a
    href="https://forms.gle/rtWuohzxRbf4BhGi7"
    class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
    >Hari 3</a
  > -->

  <!-- 
  <br />
  <div class="bg-[#00933B] rounded-xl px-3 py-6 space-y-4">
    <Field id="123" name="Nama" placeholder="Masukkan nama" />
    <Field id="234" name="Alamat" placeholder="Masukkan alamat" />
    <Selection name="Apakah Anda Memiliki KTAM" />
  </div>
  <Button>Selanjutnya</Button> -->
</div>
