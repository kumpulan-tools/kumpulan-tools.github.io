<script>
  let isinya = "";
  if (localStorage.isinya) {
    isinya = localStorage.isinya;
  }
  $: localStorage.isinya = isinya;
</script>

<textarea
  class="textarea textarea-bordered h-[calc(100vh-130px)]"
  placeholder=""
  bind:value={isinya}
/>
