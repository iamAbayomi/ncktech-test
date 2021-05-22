<template>
  <div id="app" class="app">
    <div class="container">
      <div id ="menu-bar" class="menu-bar"> 
          <div class="sub-menu">
            <p>TRIPS </p>
          </div>
          <div class="sub-menu">
            <p>RECENTLY VIEWED</p>
          </div>
          <div class="sub-menu">
            <p>BOOKINGS </p>
          </div>
          <div class="sub-menu">
            <img class="profile-image" src="/cardi-profile-image.png" alt="profile-image">
          </div>
      </div>


      <div id="main-details" class="main-details">
       
        <div class="menu-line"> ------ </div>
       
        <div class="payment-information-section">
            <div class="card-type">
              <p id="payment-title">
                Payment Information
              </p>
              <p id="payment-subtitle">
                Choose your method of payment
              </p>
              <img class="credit-card-image" src="/card_image.jpg" alt="Credit Card image">
            </div>
            <div class="card-details">
                <div class="payment-type">
                    <img class="payment-logo" src="/visa-icon.png" alt="Visa">
                    <img class="payment-logo" src="/discover-logo.png" alt="Discover">
                    <img class="payment-logo" src="/paypal-logo.png" alt="PayPal">
                </div>
                <div class="card-input-details">
                    <form action="/card-details">
                      <div>
                        <label for="credit-card-no">Credit Card Number</label>
                        <input type="text" id="credit-card-no" name="">
                        
                        <label for="expiration-date">Expiration Date</label>
                        <input type="text" id="expiration-date" name=""><br><br>
                      </div>
                      <div>
                        <label for="security-code">Security Code</label>
                        <input type="text" id="security-code" name="">
      
                        <label for="postal-code">Postal Code</label>
                        <input type="text" id="Postal Code" name=""><br><br>
                      </div>
                        <p>Use this card for next time purchase </p>
                        <input type="submit" class="long-blue-button blue-button" value="Add Card">
                    </form>
                </div>
            </div>
        </div>
        
        <div class="menu-line"> ------ </div>
        
        <div class="payment-details-section">
          <div class="sub-total-div flex-row">
              <p id="subtotal-text"> 
                Subtotal
              </p>
              <div class="price"> 
                  <img class="naira-image" src="/naira-image.jpg">
                  <p class="subtotal-value figure"> 
                    2,497.00
                  </p>
              </div> 
          </div>
          <div class="sub-total-div flex-row">
              <p id="estimated-tax-text"> 
                  Estimated TAX
              </p>
              <div class="price"> 
                  <img class="naira-image" src="/naira-image.jpg">
                  <p class="estimated-tax-value figure"> 
                    119.64
                  </p>
              </div> 
          </div>
          <div class="sub-total-div flex-row">
              <div class="promotional-code flex-row">
                <p id="promotional-code-text"> 
                    Promotional Code
                </p>
                <p id="promotional-code-subttilte-text"> 
                    :Z4KXLM94
                </p>
              </div>
              <div class="price"> 
                  <img class="naira-image" src="/naira-image.jpg">    
                  <p class="promotional-code-value figure"> 
                      -60.00
                  </p>
              </div> 
          </div>
        </div>
        
        <div class="menu-line"> ------ </div>
        
        <div class="payment-accept-section"> 
            <input type="submit" class="blue-button" value="Complete payment">
            <div class="total-figure flex-row">
                <p id="payment-accept-total">TOTAL:</p>
                <div class="price payment-section"> 
                  <img class="naira-image" src="/naira-image.jpg">    
                  <p class="payment-accept-text">2556.64</p>
              </div> 
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App'
}
</script>

<style>
.body{
  font-family: Arial, Helvetica, sans-serif;
}

.app{
  margin: auto;
  max-width: 1300px;
}

.container{
  margin: 30px;
}

.menu-bar{
 display: flex;
 float: right;
 font-family: Arial, Helvetica, sans-serif;
}

.sub-menu p{
  margin: 20px;
  font-size: 14px;
  color:darkgray;
  font-family: Helvetica;
  font-weight: 800;
}

.profile-image{
  width: 40px;
}

.main-details{
  clear: both;
}

.payment-information-section{
  display: flex;
  justify-content: space-between;
}

.credit-card-image{
  width: 400px;
}

.payment-type{
  float: right;
}

.payment-logo{
  /* height: 50px; */
  margin: 10px;
  width: 40px;
  /* border:1px solid; */
}

.card-type{
  clear: both;
}

.card-details{
  width: 600px;
}

.card-input-details{
  clear: both;
}

.flex-row{
  display: flex;
  justify-content: space-between;
}

.figure{
  float: right;
  color:#424859;
  font-weight: bold;
}

.payment-accept-section{
  display: flex;
  justify-content: space-between;
}

.blue-button{
  color: white;
  width: 200px;
  height: 44px;
  font-size: 16px;
  background: hsl(226, 78%, 42%);
  border-color:#1A48E2;
  border-width: 0px;
  border-radius: 0px;
}

.long-blue-button{
  color: white;
  width: 600px;
}

.price{
  /* border: 1px solid;
  border-width: 1px; */
  display: flex;
  align-items: center;
}

.naira-image{
  /* border: 1px solid;
  border-width: 1px; */
  margin: 18px 1px 18px 0px;
  width: 11px;
}


.total-figure{
  /* border: 1px solid;
  border-width: 1px; */
}

.payment-section{
  /* display: flex; */
}

</style>
