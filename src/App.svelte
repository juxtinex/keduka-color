<script>
import Sliider from "./Sliider.svelte";
let redColor = 100;
let greenColor = 0;
let blueColor = 0;
</script>
<div class="row">
  <div class="col">
    <h1 style="color: rgb({redColor}, {greenColor}, {blueColor});">KEDUKA- JUST COLOR YOUR WORLD</h1>
  </div>
</div>
<div class='row'>
<div class="column">
  <form>
    <Sliider colorName="Red" bind:colorValue={redColor}/>
    <Sliider colorName="Green" bind:colorValue={greenColor}/>
    <Sliider colorName="Blue" bind:colorValue={blueColor}/>
  </form>
</div>
</div>
<div class="row">
  <div class="column">
    <div id="color" style="background-color: rgb({redColor}, {blueColor}, {greenColor});"></div>
  </div>
  <div class="row">
    <div class="column">
      <h2>rgb({redColor}, {blueColor}, {greenColor})</h2>
    </div>
  </div>
</div>
<style>
  #color{
    height: 300px;
    border: dashed 5px;
  }
  h2{
    text-align: center;
    margin-top: 20px;
  }
 
  
</style>
