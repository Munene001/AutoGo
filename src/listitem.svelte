<script>
  import { onMount } from "svelte";
  import {navigate} from "svelte-routing"
  import Icon from "@iconify/svelte";
  export let name = "Mazda Atenza";
  export let price = "KSH 1700/HR";
  export let src = "/car1.jpg";
  export let description = "Fast and sleek.2.5-liter engine . Fuel efficiency of 28mpg in the suburbs and 36mpg on the highway.";
  export let seats = "4";
  export let id;
  let showInfo = false;
  onMount(() => {
    const moreInfoButton = document.querySelector(`#${id}`);

    moreInfoButton.addEventListener("click", () => {
      showInfo = !showInfo;
    });
  });
</script>

<div class="div clearfix">
  <div class="div1">
    <img {src} alt="h2" />
  </div>
  <div class="div2">
    <div class="layer1">
      <div class="name">{name}</div>
      <div><button  class="select" on:click={(e)=> navigate("/contact")}>Select</button></div>
    </div>
    <div class="layer2">{price}</div>
    <div class="layer3">
      <div class="layer31">
        <div>
          <button {id} class="bt">more info </button>
        </div>
      </div>
      {#if showInfo}
        <div class="additional-info"><p>
          {description}</p>
        </div>
      {/if}
      <div class="layer32">
        <div class="icon1" style=" color:#00FF00; font-size:17px">
          <Icon icon="bi:fuel-pump-diesel-fill" />
        </div>
        <div class="icon2" style="color:chocolate; font-size: 20px;">
          <Icon icon="mdi:petrol" />
        </div>
        <div class="icon3" style="color:blue; font-size:20px">
          <Icon icon="material-symbols:speed-outline" />
        </div>
      </div>
      <div class="layer33">
        <div
          class="layer331"
          style="border:2px solid white; padding:6px; color:white; font-size: 13px;"
        >
          {seats}<Icon icon="material-symbols:person-add-outline" />
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  .div {
    padding: 20px;
    background-color: black;
    height:auto;
    display: flex; /* Use flexbox to align child divs */
    /* Vertically center child divs */
    position:relative;
  }

  .div1 {
    width: 37%;
    background-color: black;
  }

  .div1 img {
    object-fit: cover;
    width: 100%;
    height: auto;
  }

  .div2 {
    width: 63%;
    display: flex;

    /* Vertically center content */
    /* Add some space between the two child divs */
    margin-left: 10px;
    flex-direction: column;
  }
  .layer1 {
    width: 100%;
    height: auto;

    color: white;
    flex-direction: row;
    display: flex;
    justify-content: space-between;
  }

  .name {
    color: white;
    font-size: 12px;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  }

  .select {
    background-color: white;
    color: black;
    padding: 3px;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    /* Add padding to the select button */
    font-size: 12px;
  }
  .select:hover {
    background-color: chocolate;
  }
  .layer2 {
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    font-size: 13px;
    color: chocolate;
    
  }
  .layer3 {
    margin-top: auto;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
  .layer31 {
    display: flex;
    flex-direction: row;
  }
  .layer32 {
    display: flex;
  }
  .layer33 {
    display: flex;
  }
  .bt {
    background-color: transparent;
    color: white;
    padding: 4px;
    border-radius: 15%;
    font-size: 9px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
  }
  .bt:hover {
    background-color: chocolate;
  }
  @media (min-width: 768px) {
    .name {
      font-size: 20px;
    }
    .select {
      font-size: 17px;
    }
    .layer2 {
      display: flex;
      font-size: 25px;
      margin-top: 25px;
    }
    .bt {
      font-size: 17px;
    }
    .icon1 {
      font-size: 30px;
    }
    .icon2 {
      font-size: 30px;
    }
    .icon3 {
      font-size: 30px;
    }
    .layer331 {
      font-size: 17px;
    }
  }
  .additional-info{
    position: absolute;
    color:whitesmoke;
    font-size: 9px;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    z-index: 1;
    top: 33%;
    left:40%;
  }
  @media (max-width:768px){
    .layer2{
      position:absolute;
      top: 26%;
      left:39.6%;
    }
  }
  @media (min-width:768px){
    .additional-info{
      font-size: 17px;
      top: 40%;
      left:40%;
      right:10%;
    }
  }
</style>
