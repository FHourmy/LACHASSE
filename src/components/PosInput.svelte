<script>
  export let isDisabled = false;
  export let valueX;
  export let valueY;
</script>

<div>
  <input disabled={isDisabled} bind:value={valueX} />
  <input disabled={isDisabled} bind:value={valueY} />
</div>

<style>
</style>
