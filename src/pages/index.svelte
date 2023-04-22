<script>
  import kode_bank from "../data-kode-bank";
  import AnakTabel from "../anak-tabel.svelte";
</script>

<div class="text-center py-3">KODE BANK</div>
<div class="px-3">
  <table>
    <thead>
      <tr>
        <AnakTabel komponen="th" isi="Nama Bank" />
        <AnakTabel komponen="th" isi="Kode Bank" />
      </tr>
    </thead>
    <tbody>
      {#each kode_bank as x}
        <tr>
          <AnakTabel komponen="td" isi={x.nama_bank} />
          <AnakTabel komponen="td" isi={x.kode_bank} />
        </tr>
      {/each}
    </tbody>
  </table>
</div>
