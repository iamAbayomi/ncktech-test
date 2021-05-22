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
              <img src="" alt="Credit Card image">
            </div>
            <div class="card-details">
                <div id="payment-type">
                    <img src="" alt="Visa">
                    <img src="" alt="Discover">
                    <img class="payment-logo" src="/paypal-logo.svg" alt="PayPal">
                </div>
                <div id="card-input-details">
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
                        <input type="submit" value="Add Card">
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
              <p class="subtotal-value figure"> 
                #2,497.00
              </p>
          </div>
          <div class="sub-total-div flex-row">
              <p id="estimated-tax-text"> 
                  Estimated TAX
              </p>
              <p class="estimated-tax-value figure"> 
                  #119.64
              </p>
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
              <p class="promotional-code-value figure"> 
                  #-60.00
              </p>
          </div>
        </div>
        
        <div class="menu-line"> ------ </div>
        
        <div class="payment-accept-section"> 
            <button class="blue-button"> Complete Payment</button>
            <div class="total-figure flex-row">
                <p id="payment-accept-button">TOTAL</p>
                <p id="payment-accept-text">#2556.64</p>
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
  font-weight: bold;
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

.flex-row{
  display: flex;
  justify-content: space-between;
}

.figure{
  float: right;
}

.payment-accept-section{
  display: flex;
  justify-content: space-between;
}

</style>
