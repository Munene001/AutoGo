<script>
  import Icon from "@iconify/svelte";
  import { navigate } from "svelte-routing";
  let popOpen = false;
  const links = [
    { label: "Home", url: "/" },
    { label: "About", url: "/about" },
    { label: "CarListing", url: "/carlisting" },
    { label: "Contact", url: "/contact" },
  ];
  $: {
    console.log("Pops", popOpen);
  }
  /**@param {string} url */
  const navigateTo = (url) => {
    navigate(url);
  };
</script>

<div class="uno">
  <div class="logo"><img src="/logo3.jpg" alt="logo" /></div>
  <div class = developerwidth>
    <div class = subzero>{#each links as link}
      <button class = button0 on:click={(e)=> navigateTo(link.url)}>
      {link.label}</button>
    {/each}</div>
  </div>
  <div  class = clientwidth style="color:chocolate;">
    <button class="button1" on:click={(e) => (popOpen = true)}
      ><Icon icon="majesticons:menu" /></button
    >
    {#if popOpen}
      <div class="pops">
        <div class="pops1">
          {#each links as link}
            <button class="button2" on:click={(e) => navigateTo(link.url)}
              >{link.label}</button
            >
          {/each}
        </div>
        <button class = button3 on:click={(e) => (popOpen=false)}><Icon icon="zondicons:close" /></button>
      </div>
    {/if}
  </div>
</div>

<style>
  .uno {
    padding: 10px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    background-color: #4B3832 ;
    background-color: brown;
    background-color:#4B3621 ;
    background-color:  #7B5C3A;
  }
  .logo img {
    width: 60px;
  }
  .button1 {
    padding: 1px;
    background-color: chocolate;
    font-size: 25px;
    color: whitesmoke;
  }
  .pops {
    position: fixed;
    background-color: beige;
    z-index: 20;
    top: 1.7rem;
    right: 1rem;
  }
  .pops1 {
    display: flex;
    flex-direction: column;
    cursor: pointer;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    padding-top: 8px;
    padding-bottom: 10px;
    align-items: flex-start;
    background-color:burlywood;
    width:250px;
    
  }
  .button2 {
    padding-left: 0.5rem /* 8px */;
    padding-right: 0.5rem /* 8px */;
    margin: 1.2px;

    color: chocolate;
    font-weight: bold;
    font-size: 16px;
    width: 80%;
    text-align: left;
    background-color: white;
    border: 0px;
    border-radius: 20px;
  }
  .button2:hover {
    background-color: black; /* Add your desired background color *
  /* Add any additional styles for the hover effect */
  }
  .button3{
    position:absolute;
    font-size: 17x;
    top:1%;
    right:1%;
    border-radius: 10px;
  }
  @media (max-width:768px){
  .developerwidth{
    display: none;
    
  }
  .subzero{
    display: none;
  }
  .button0{
    display:none;
  }
}
  
  @media (min-width:768px){
    .clientwidth{
      display: none;
    }
  }


   .developerwidth{
    display: flex;
    flex-direction: row;
    justify-content: end;

   }
   .subzero{
    font-size: 17px;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    margin-left: 5px;
    border:0px;
  
   }
   .button0{
    color:#FFFFFF;
    background-color: #4B3832;
    margin-right: 35px;
    border:0px;
   }
     /* Home Page */
 
</style>
