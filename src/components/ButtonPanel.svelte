<script>
  import Button from "./Button.svelte";
</script>

<div class="container">
  <div><Button isFocused={false} text={"↑"} /></div>
  <div>
    <Button isFocused={false} text={"←"} />
    <Button isFocused={false} text={"GO"} />
    <Button isFocused={false} text={"→"} />
  </div>
  <div><Button isFocused={false} text={"↓"} /></div>
</div>

<style>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>
