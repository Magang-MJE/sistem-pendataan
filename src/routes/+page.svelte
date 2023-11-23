<script>
  import Button from "../lib/Button.svelte";
  import Field from "../lib/Field.svelte";

  import { onMount } from "svelte";
  let hari;
  let tanggal;

  const mappingTanggal = {
    24: "https://forms.gle/58JJV1SG2Ae3hZpx7",
    25: "https://forms.gle/baD6bcH9Y9rFb2Lz5",
    26: "https://forms.gle/rtWuohzxRbf4BhGi7",
  };

  onMount(() => {
    const date = new Date();
    hari = new Intl.DateTimeFormat("id-ID", {
      dateStyle: "full",
    }).format(date);
    tanggal = date.getDate();

    console.log(hari);

    tanggal = tanggal < 24 ? 24 : tanggal > 26 ? 26 : tanggal;
  });
</script>

<div class="flex flex-col mx-auto font-bold text-white text-center my-10">
  <a
    href={mappingTanggal[`${tanggal}`]}
    class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
    >Form Pengunjung {tanggal} November 2023</a
  >

  <a
    href="/pendataan-harian"
    class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
    >Susunan Acara MJE#3</a
  >
</div>
