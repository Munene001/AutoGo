<script>
  import Footer from "../footer.svelte";
  import Icon from "@iconify/svelte";
  import Header from "../Header.svelte";
  import {navigate} from "svelte-routing";
 
 
</script>
<Header/>
<div class="Home">
  <img src="home1.jpg" alt="x0" />
  <div class="overlay">
    <h1 class="header">Renting a car has never been this easy</h1>
  </div>
  <div class="front">
    <div class="arrow">
      <Icon icon="material-symbols:double-arrow" />
    </div>
    <div><button class="book" on:click={(e)=>navigate("/carlisting")}>Book Us</button></div>
  </div>
</div>

<div class="bottom">
  <div class="lower">
    <div class="icon-container" style="color:#00FF00;">
      <Icon icon="material-symbols:car-rental" />
    </div>
    <div style="margin-top: 15px;">Select car</div>
  </div>
  <div class="inbetween"><Icon icon="material-symbols:double-arrow" /></div>
  <div class="lower">
    <div class="icon-container" style="color:#00FF00;">
      <Icon icon="tabler:brand-booking" />
    </div>

    <div style="margin-top: 15px;">Do booking</div>
  </div>

  <div class="inbetween"><Icon icon="material-symbols:double-arrow" /></div>

  <div class="lower">
    <div class="icon-container" style="color:#00FF00;">
      <Icon icon="mdi:account-payment" />
    </div>
    <div style="margin-top: 15px;">Pay payment</div>
  </div>
</div>


<style>
  .Home {
    position: relative;
    width: 100%;
    height: 100vh;
    
    
  }
  .Home img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .overlay {
    position: absolute;
    top: 30%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .header {
    color: black;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    font-weight: bold;
  }
  .front {
    position: absolute;
    top: 45%;
    left: 30%;
    display: flex;
    flex: column;
  }

  .book {
    display: flex;
    flex: column;
    flex-wrap: wrap;
    border-radius: 50px;
    align-items: center;
    padding: 20px;
    background-color: transparent;
    color: white;
  }
  button:hover {
    background-color: chocolate;
  }

  .bottom {
    position: relative;
    background-color: black;
    display: flex;
    flex-wrap: nowrap;
    padding: 23px;
    flex: column;
    color: white;
    justify-content: space-around;
  }
  .lower {
    display: flex;
    flex-direction: column;
    align-items: center;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  }
  .icon-container {
    display: inline-block;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    border: 1px solid white; /* Set your desired border color and thickness */
    text-align: center;
    line-height: 50px;
  }
  .inbetween {
    font-size: 30px;
    align-items: center;
    animation-name: right;
    animation-duration: 5s;
    animation-iteration-count: infinite;
    color: #00ff00;
  }
  @keyframes right {
    0% {
      transform: translateX(-100%);
    }
    100% {
      transform: translateX(100%);
    }
  }
  .arrow {
    color: #00ff00;
    font-size: 55px;
    color: white;
    width: min-content;
    height: 70px;
    
  }
</style>
