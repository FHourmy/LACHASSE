<script>
  export let isFocused = false;
  export let text = "GO";
  const className = "button" + (isFocused ? " focused-button" : "");
</script>

<div class={className}>{text}</div>

<style>
  /* CSS */
  .button {
    align-items: center;
    background-clip: padding-box;
    background-color: #f5eded;
    border: 1px solid transparent;
    border-radius: 0.25rem;
    box-sizing: border-box;
    cursor: pointer;
    display: inline-flex;
    font-family: system-ui, -apple-system, system-ui, "Helvetica Neue",
      Helvetica, Arial, sans-serif;
    font-size: 16px;
    justify-content: center;
    line-height: 1;
    margin: 0;
    padding: 0.7rem 0.7rem 0.8rem 0.7rem;
    position: relative;
    text-decoration: none;
    transition: all 250ms;
    user-select: none;
    -webkit-user-select: none;
    touch-action: manipulation;
    vertical-align: baseline;
    vertical-align: baseline;
    width: 3rem;
    height: 3rem;
    font-weight: 900;
  }

  .button:hover,
  .button:focus {
    background-color: #dee1ec;
  }

  .button:active {
    background-color: #dee1ec;
  }
  .focused-button {
    background-color: #dee1ec;
  }
</style>
