<script>
  export let colorName;
  export let colorValue;
</script>
<label for={colorName}>{colorName} ({colorValue})</label>
    <input type="range" id= {colorValue} bind:value={colorValue} min="0" max="255">
<style>
  input{
    width:100%;
  }
</style>