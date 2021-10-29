<script>
  export let hints = ["test", "test2"];
  export let currentHint;
</script>

<select value={currentHint}>
  {#each hints as hint}
    <option>{hint}</option>
  {/each}
</select>
