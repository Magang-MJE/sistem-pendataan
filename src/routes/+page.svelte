<script>
  import { onMount } from "svelte";

  let showLink = false;
  let tanggal;
  let hari;
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

    const jamShowLink = date.getHours();
    const ampm = jamShowLink >= 12 ? "PM" : "AM";
    const convertJam12 = jamShowLink % 12 || 12;

    showLink =
      tanggal >= 24 &&
      tanggal <= 26 &&
      convertJam12 >= 1 &&
      convertJam12 < 5 &&
      ampm === "PM";
  });
</script>

<div class="flex flex-col mx-auto font-bold text-white text-center my-10">
  <a
    href={mappingTanggal[`${tanggal}`]}
    class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
  >
    Form Pengunjung {tanggal} November 2023
  </a>

  <a
    href="/pendataan-harian"
    class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
  >
    Susunan Acara MJE#3
  </a>

  {#if showLink}
    <a
      href="https://forms.gle/8sBcryxtchLoAh2E9"
      class="bg-[#D7A652] rounded-xl p-3 text-white border-b-2 border-[#D7A652] font-bold mt-5"
      >Tiket Talk Show Muda Mendunia
    </a>
  {/if}
</div>
