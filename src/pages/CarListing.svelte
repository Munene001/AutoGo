<script>
  import Footer from "../footer.svelte";
 
  import Listitem from "../listitem.svelte";
  import Icon from "@iconify/svelte";
  import Header from "../Header.svelte";
</script>
<Header class = cs/>

<div class="uno">
  <div class="journey">AutoGo <Icon icon="mdi:car-hatchback" /></div>
  <div class="first"><img src="/wall2.jpg" alt="Xo" /></div>
  <div class="second"><img src="/wall1.jpg" alt="Xo" /></div>
</div>

<div class >
  <Listitem  id="button1"seats="2"  />
  <Listitem  id="button2"src="/car2.jpg" seats="4" name="Bentley 360" price="KSH 2500/HR"  description = "Exquisite and refined. 6.0-liter W12 engine. Fuel efficiency of 12mpg in the suburbs and 19mpg on the highway."/>
  <Listitem  id="button3"src="/car6.jpg" name="Mercedes Mayback" price="KSH 2300/HR"  description = "Luxurious and powerful. 4.0-liter V8 engine. Fuel efficiency of 22mpg in the suburbs and 30mpg on the highway." />
  <Listitem
    src="/car4.jpg"
    name="Chevrolet SUV"
    seats="5"
    price="KSH 3000/HR"
    id="button4"
    description = "Versatile and robust. 3.6-liter V6 engine. Fuel efficiency of 18mpg in the suburbs and 25mpg on the highway."
    
  />
  <Listitem name = "Mercedes GLS" src="/car8.jpg" id="button5"  description="Dynamic and elegant.  3.6-liter V6 engine. Fuel efficiency of 18mpg in the suburbs and 25mpg on the highway"/>
</div>
<Footer/>

<style>
  .journey {
    position: absolute;
    font-size: 11px;
    color:#00FF00;
    background-color: blue;
    border: 1px solid white;
    padding: 5px;
    animation-name: example;
    animation-duration: 16s;
    animation-iteration-count: infinite;
    z-index: 1; /* Ensure the element appears on top of other elements */
    border-radius: 30%;
  }
  
  @keyframes example {
    0% {
    background-color: chocolate;
      left: 0;
      top: 0;
    }
    25% {
    background-color: transparent;
      left: calc(100% - 2em);
      top: 0;
    }
    50% {
    background-color: chocolate;
      left: calc(100% - 2em);
      top: calc(100% - 2em);
    }
    75% {
    background-color:chocolate;
      left: 0;
      top: calc(100% - 2em);
    }
    100% {
    background-color: transparent;

      left: 0;
      top: 0;
    }
  }
  
  .uno {
    position: relative;
    height: auto;
    display: flex; /* Use flexbox to align child divs */
    border: 10px solid transparent;

    /* Vertically center child divs */
    border-image: url(/wall5.jpg) 10% round;
  }

  .first {
    width: 50%;
    position: relative;
  }

  .first img {
    object-fit: cover;
    width: 100%;
    height: auto;
  }

  .second {
    position: relative;
    width: 50%;
    display: flex;
  }
  .second img {
    object-fit: cover;
    width: 100%;
    height: auto;
  }
  @media (min-width:768px){
    .journey{
      font-size: 17px;
      animation-duration:22s;

    }
  }
    
  
</style>
