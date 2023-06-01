<script>
  import Icon from "@iconify/svelte";
  import Footer from "../footer.svelte";
  import Header from "../Header.svelte";
</script>

<div class="uno">
  <Header />
  <div class="layer1">
    <div style="color:silver; margin-left:15px;"><h1>About Us</h1></div>
    <div class="layer11">
      <p>
        AutoGo has a foundation built on trust and reputation.We know how to
        make our customers love us by our high quality products.
      </p>
      <p>
        Whether you're traveling for business or pleasure, we strive to make
        your car rental experience convenient, efficient, and enjoyable and
        become your go-to choice for car rentals.
      </p>
      <p>AutoGo was founded in 2005 by a bunch of carlovers in a bid to fuse travel with luxurious transportation.Our company is managed by a board of directors</p>
    </div>
  </div>
  <div class="layer15">
    <img src="carl2.jpg" alt="aboutus" />
  </div>
  <div class="layer17">
    <div><Icon icon="twemoji:vertical-traffic-light" /></div>
    <div style="color:goldenrod"><Icon icon="entypo:traffic-cone" /></div>
    <div style="color:lightblack;"><Icon icon="fa6-solid:road" /></div>
  </div>
  <div class="layer2">
    <div class="layer22">
      <div class="shadow17">
        <div><Icon icon="twemoji:vertical-traffic-light" /></div>
        <div style="color:goldenrod"><Icon icon="entypo:traffic-cone" /></div>
        <div style="color:lightblack;"><Icon icon="fa6-solid:road" /></div>
      </div>
      <h1>Terms And Conditions</h1>

      <p>
        Please read these terms and conditions carefully before using our
        services.
      </p>
      <ol>
        <li>
          By using our services, you agree to comply with these terms and
          conditions.
        </li>
        <li>All rental bookings are subject to availability.</li>
        <li>
          Drivers must possess a valid driver's license and meet the minimum age
          requirement.
        </li>
        <li>
          Customers are responsible for returning the rental vehicle in the same
          condition as received.
        </li>
        <li>
          Any damages to the vehicle during the rental period will be the
          responsibility of the customer.
        </li>
        <li>
          Additional charges may apply for late returns, fuel refills, or other
          optional services.
        </li>
        <li>
          Reservations can be modified or canceled based on our cancellation
          policy.
        </li>
        <li>
          We reserve the right to refuse service to anyone for any reason.
        </li>
        <li>
          All personal information provided will be handled in accordance with
          our privacy policy.
        </li>
        <li>
          AutoGo shall not be held liable for any loss, damage, or inconvenience
          arising from the use of our services.
        </li>
      </ol>
      <p>
        Please contact us if you have any questions regarding these terms and
        conditions.
      </p>
    </div>
  </div>
  <div />
</div>
<Footer />

<style>
  .uno {
    display: flex;
    flex-direction: column;
    position: relative;
    font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
      "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
    border: 2px solid #7b3f00;
  }
  .layer1 {
    width: 100%;
    background-color: #7b3f00;
    height: 65vh;
  }
  .layer2 {
    width: 100%;
    background-color: white;
    height: auto;
  }
  .layer11 {
    color: white;
    margin: 0 0 1.5em; /* Adjust the margin as per your preference */
    line-height: 1.3;
    margin-left: 15px;
    margin-right: 15px;
  }
  .layer15 {
    position: absolute;
    width: 35%;
    top: 34.5%;
    right: 8%;
    z-index: 1;
  }
  .layer15 img {
    width: 100%;
  }
  .layer22 {
    line-height: 1.7;
    margin-left: 15px;
    margin-right: 15px;
    margin-top: 65px;
    color: #7b3f00;
    position: relative;
  }
  .layer17 {
    position: absolute;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    width: 37%;
    top: 38%;
    left: 4%;
    font-size: 26px;
  }
  .shadow17 {
    display: none;
  }
  @media (min-width: 768px) {
    .layer17 {
      display: none;
    }

    .shadow17 {
      position: absolute;
      display: flex;
      top: 35%;
      right: -10%;
      flex-direction: column;
      width: 35%;
      font-size: 40px;
    }
  }
</style>
