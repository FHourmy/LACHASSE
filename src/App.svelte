<script>
  import { onMount } from "svelte";
  import ButtonPanel from "./components/ButtonPanel.svelte";
  import PosInput from "./components/PosInput.svelte";
  import SelectHint from "./components/SelectHint.svelte";
  import ioHook from "iohook";
  onMount(() => {
    ioHook.on("mousemove", (event) => {
      console.log(event); // { type: 'mousemove', x: 700, y: 400 }
    });
    ioHook.start();
  });
</script>

<div class="container">
  <PosInput />
  <PosInput isDisabled />
  <SelectHint />
  <ButtonPanel />
</div>

<style>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>
