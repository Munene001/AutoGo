<script>
</script>

<div class = uno>
  <div>
    <h1 style = "justify-content:center;" >Contact Us</h1>
  </div>
      <div>
        <p>
          Feel free to contact us any time. We will get to you as soon as we
          can.
        </p>
      </div>
      
    <div>
      <form method="post">
        <label>Name</label>
        <input type="text" />
        <label>Email</label>
        <input type="text" />
        <label>Car brand</label>
        <select name="car">
          <option value="Mazda Atenza">Mazda Atenza</option>
          <option value="Bentley 360">Bentley 360</option>
          <option value="Mercedes Maybach">Mercedes Maybach</option>
          <option value="Chevrolet Suv">Chevrolet SUV</option>
          <option value="Mercedes GLS">Mercedes GLS</option>
        </select>
        <label>Hours</label>
        <input type="number" />
      <br>
      <button style = "border:1px solid black; padding:5px;" >submit</button>
    </form>
  </div>
</div>

<style>
    .uno{
        position:relative;
        display: flex;
        
        background-color: white;
        padding:15px;
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
        justify-content: start;
        border: 2px solid black;
        
    
        flex-direction: column;

    }
    
      @media (min-width:768px){
        .uno{
          width:400px;
          
        }

      }

    
    </style>