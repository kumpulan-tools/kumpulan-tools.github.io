<script>
  let banyak_kesalahan = "";
  let nilai = "";

  $: nilai = ~~(((210 - banyak_kesalahan) * 100) / 210);
</script>

<div class="form-control w-full">
  <label class="label">
    <span class="label-text">Banyak Kesalahan</span>
    <span class="label-text">Max 5 per hadits</span>
  </label>
  <input
    type="tel"
    bind:value={banyak_kesalahan}
    placeholder="Tulis di sini"
    class="input input-bordered w-full"
  />
</div>
<div class="form-control w-full">
  <label class="label">
    <span class="label-text">Nilai</span>
  </label>
  <input
    type="tel"
    readonly
    bind:value={nilai}
    placeholder=""
    class="input input-bordered w-full"
  />
</div>
