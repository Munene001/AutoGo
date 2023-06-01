<script>
  import Icon from "@iconify/svelte";
</script>

<div class="uno">
  <div class = logo><img src = "logo3.jpg" alt = logo/></div>
  <div class="layer1">
    <div style="font-weight:bold; font-size:25px;color:black">Details</div>
    <div style="margin-top:3%;">785 Ronald Ngala street</div>
    <div style="margin-top:3%;">0715067768</div>
    <div style="margin-top:3%;">Info@Autogo.com</div>
  </div>
  <div class="layer2">
    <div style="font-weight:bold; font-size:25px;color:black">
      Informative Searches
    </div>
    <div style="margin-top:3%; color:white;">
      <a href="https://openroadodysseys.com/the-most-comfortable-car-to-rent/">Best Cars to rent</a>
    </div>
    <div style="margin-top:3%;">
      <a href="https://www.quora.com/If-you-had-to-choose-between-a-luxury-car-and-a-sports-car-which-would-be-it">Luxury vs Speed </a>
    </div>
    <div style="margin-top:3%;">
      <a href="https://www.edmunds.com/car-buying/10-steps-to-finding-the-right-car-for-you.html"
        >Tips on what to look for in a car</a
      >
    </div>
    <div  class = copy1 style = " font-size:17px;color:white"><i>@Copyright 2023</i></div>
  </div>
  <div class="layer3">
    <div style="font-weight:bold; font-size:25px;color:black">Engage Us</div>
    <div style="margin-top:3%;">Social Media platforms</div>
    <div class="layerz">
      <div style = "margin-left:3%;"><Icon icon="logos:facebook" /></div>
      <div style = "margin-left:3%;"><Icon icon="skill-icons:twitter" /></div>
      <div style = "margin-left:3%;"><Icon icon="skill-icons:linkedin" /></div>
    </div>

    
  
  </div>
  <div  class = copy style = " font-size:17px;color:white"><i>@Copyright 2023</i></div>
</div>

<style>
  .uno {
    background-color: chocolate;

    position: relative;
    display: flex;
    flex-direction: column;
    
  }

  .layer1 {
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    font-size: 16px;
    color: white;
    margin-top: 7%;
    margin-left: 7%;
  }
  .layer2 {
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    font-size: 16px;
    color: white;
    margin-top: 7%;
    margin-left: 7%;
  }
  .layer2 a {
    color: darkblue;
  }
  .layer3 {
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    font-size: 16px;
    color: white;
    margin-top: 7%;
    margin-left: 7%;
  }
  .logo{
   position: absolute;
   top:7%;
   left:79%;
   width: 35%;
   
  }
  .logo img{
    width: 50%;
  }

  .layerz{
    display:flex;
    flex-direction: row;
    align-items: center;
    margin-top: 3%;
   


  }
  .copy{
    align-items: center;
    display: flex;
    justify-content: center;
    margin-top: 3%;
    margin-bottom: 2%;
  }
  @media (max-width:768px){
  .copy1{
    display:none;
  }
}
    


  
  @media (min-width:768px){
    .uno{
     
      flex-direction: row;
      display: flex;
      justify-content: space-evenly;
      height: 31.5vh;


    }
    .logo{
      display: none;
    }
    .layer1{
      margin-top: 3%;
    }
    .layer2{
      margin-top: 3%;
    }
    .layer3{
      margin-top: 3%;
    }
    .copy{
      display:none;
    }
    .copy1{
      display: flex;
      margin-top: 8.5%;
    }
    .layerz{
      display: flex;
      font-size: 22px;
     
    }
  }
</style>
