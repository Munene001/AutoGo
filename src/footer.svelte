<script>
  import Icon from "@iconify/svelte";
</script>

<div class="uno">
  <div class="first">
    <div><img src="./logo3.jpg" alt="logo" /></div>
    <div style="font-size:16px; color:black;margin-top:5px;">Terms and Conditions apply</div>
    
    
  </div>
  <div class = second>
    <div style="color:white;">AutoGo</div>
    <div style="color:white;">Services </div>
    <div style = color:white;>Support</div>
  </div>
  <div class="third">
    <div
      style="font-size:17px; color:white; font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif; "
    >
      For inquiry
    </div>
    <div
      style="font-size:17px; color:white; font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif; margin-right:15px;"
    >
       Call<Icon icon="fluent:call-28-filled" />
    </div>
    <div style="font-size:20px; color:black;">0715067768</div>
    <div class="layerz">
    <div><Icon icon="logos:facebook" /></div>
    <div><Icon icon="skill-icons:twitter" /></div>
    <div><Icon icon="skill-icons:linkedin" /></div>
  </div>
  </div>
  <div class = free>@Copyright 2023</div>
</div>

<style>
  .uno {
    display: flex;
    flex-direction: row;
    background-color:#7b3f00;
    height: 25vh;
    align-items: center; /* Align items vertically in the center */
    position: relative;
    justify-content:space-around;
  
   
  }
  .first {
    display: flex;
    flex-direction: column;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  
  }
  .first img {
    width: 25%;
    height: auto;
  }
  .third {
    display: flex;
    flex-direction: column;

  }
  .layerz {
    display: flex;
    flex-flow: wrap-reverse;
    align-items: center; /* Align items vertically in the center */
    gap: 10px;
    margin-top: 14px;
  }
  .free{
    position:absolute;
    bottom: 5%;
    left:41%;
    color:silver;
    margin-top: 30px;
    display: flex;
    justify-content: center;
  }
  .second{
    display:none;
    
  }
  @media (min-width:768px){
    .second{
    display:none;
    
  }
  .uno{
    height:23vh;
  }
 
  

  }
</style>
