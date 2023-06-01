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
  <Listitem  id="button1"seats="2" src="/veh2.jpg" />
  <Listitem  id="button2"src="/veh1.jpg" seats="4" name="Bentley 360" price="KSH 2500/HR"  description = "Exquisite and refined. 6.0-liter W12 engine. Fuel efficiency of 12mpg in the suburbs and 19mpg on the highway."description2 = "Bentley is a renowned British luxury car manufacturer known for producing high-end and handcrafted vehicles. Bentley models are characterized by their luxurious interiors, powerful engines, and refined driving experiences. Some popular Bentley models include the Bentley Continental GT, Flying Spur, and Bentayga SUV, which offer a combination of performance, comfort, and craftsmanship." desc= "Bentley is a renowned British luxury car manufacturer known for producing high-end and handcrafted vehicles. "/>
  <Listitem  id="button3"src="/veh5.jpg" name="Mercedes" price="KSH 2300/HR"  description = "Luxurious and powerful. 4.0-liter V8 engine. Fuel efficiency of 22mpg in the suburbs and 30mpg on the highway." description2= " Mercedes-Maybach is the luxury sub-brand of Mercedes-Benz, known for producing exceptionally luxurious and exclusive vehicles. Maybach models represent the pinnacle of automotive opulence and craftsmanship. These vehicles offer exquisite design, sumptuous interiors with premium materials, advanced technology, and exceptional performance. The Mercedes-Maybach lineup includes sedans like the Mercedes-Maybach S-Class, offering an unparalleled level of luxury and comfort." desc = "Mercedes-Maybach is the luxury sub-brand of Mercedes-Benz, known for producing exceptionally luxurious and exclusive vehicles." />
  <Listitem
    src="/veh4.jpg"
    name="Chevrolet"
    seats="5"
    price="KSH 3000/HR"
    id="button4"
    description = "Versatile and robust. 3.6-liter V6 engine. Fuel efficiency of 18mpg in the suburbs and 25mpg on the highway."
    description2="Chevrolet offers a range of SUVs catering to various needs and preferences. One popular model is the Chevrolet Suburban, a full-size SUV known for its spaciousness and versatility. It offers seating for up to nine passengers and ample cargo space. Chevrolet also offers compact SUVs like the Chevrolet Equinox and mid-size SUVs like the Chevrolet Traverse. These models typically feature modern designs, comfortable interiors, and a range of available features."
    desc=" Chevrolet  is a full-size SUV known for its spaciousness and versatility"
  />
  <Listitem name = "Jeep" src="/veh8.jpg" id="button5"  description="Dynamic and elegant.  3.6-liter V6 engine. Fuel efficiency of 18mpg in the suburbs and 25mpg on the highway" description2= "Jeep is an iconic American automotive brand known for its rugged and off-road capable vehicles. Jeep models typically feature a distinctive boxy design, high ground clearance, and four-wheel-drive systems. Jeep offers a range of vehicles, including SUVs and pickup trucks, such as the Wrangler, Grand Cherokee, and Gladiator. Jeep vehicles are popular choices for adventure enthusiasts and those who prioritize off-road capability." desc = "Jeep is an iconic American automotive brand known for its rugged and off-road capable vehicles."/>
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
