<script>
  import Footer from '../footer.svelte';
  import Con from "../con.svelte";
  import Header from '../Header.svelte';
</script>
<Header/>
<div class="uno">
  <div class="tree">
    <img src="/contact4.jpg" alt="tree" />
    <div class="con"><Con /></div>
  </div>
</div>
<div class="fin">
  <div class="fin1">
    <div style = "margin-top:16px;"> Address</div>
    <div style ="margin-top:7px; font-size:12px">785 Ronald Ngala street</div>
    <div style = "font-size:12px">Nairobi</div>
   

  </div>
  <div class="fin2">
    <div style = "margin-top:16px;">Contacts</div>
    <div style ="margin-top:7px; font-size:12px">0715067768</div>
    <div style = "font-size:12px"> infoAutogo@gmail.com</div>
    
  </div>
</div>



<style>
  .uno {
    display: flex;
    position: relative;
    flex-direction: row;
    border:1.5px solid transparent silver;
    object-fit: cover;
    
    
  }
  .tree {
    width: 100%;
    height: auto;
    position: relative;
  }
  .tree img {
    width: 100%;
    height: 76vh;
    object-fit: cover;
  }
  .con {
    position: absolute;
    top: 0%;
    right: 0%;
    width: 60%;
    opacity: 0.7;
    height: 100vh;
    overflow: hidden;
    display: flex;
    justify-content: flex-end;
    align-items:baseline;
  }
  .fin {
    background-color: black;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    color: chocolate;
    font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif ;
    height:140px;
    align-items: center;
    border:8px solid transparent;
    border-image: url(/tree.jpg) 10% round;
  
  }
  .fin1 {
    display: flex;
    flex-direction: column;
  }
  .fin2 {
    display: flex;
    flex-direction: column;
  }
 

  
</style>
