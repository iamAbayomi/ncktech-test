<template>
  <div id="app">
      <div id ="menu-bar"> 
          <div class="sub-menu">
            TRIPS
          </div>
          <div class="sub-menu">
            RECENTLY VIEWED
          </div>
          <div class="sub-menu">
            BOOKINGS
          </div>
          <div class="sub-menu">
            profile-image
          </div>
      </div>
      <div id="main-details">
        <div id="payment-information">
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
                    <img src="" alt="PayPal">
                </div>
                <div id="card-input-details">
                    <form action="/card-details">
                        <label for="credit-card-no">Credit Card Number</label>
                        <input type="text" id="credit-card-no" name=""><br><br>
                        <label for="expiration-date">Expiration Date</label>
                        <input type="text" id="expiration-date" name=""><br><br>
                        <label for="security-code">Security Code</label>
                        <input type="text" id="security-code" name=""><br><br>
                        <label for="postal-code">Postal Code</label>
                        <input type="text" id="Postal Code" name=""><br><br>
                        <p>Use this card for next time purchase </p>
                        <input type="submit" value="Add Card">
                    </form>
                </div>
            </div>
        </div>

        <div id="payment-details">
          <div id="sub-total-div">
              <p id="subtotal-text"> 
                Subtotal
              </p>
              <p id="subtotal-value"> 
                #2,497.00
              </p>
          </div>
          <div id="sub-total-div">
              <p id="estimated-tax-text"> 
                  Estimated TAX
              </p>
              <p id="estimated-tax-value"> 
                  #119.64
              </p>
          </div>
          <div id="sub-total-div">
              <p id="promotional-code-text"> 
                  Promotional Code
              </p>
              <p id="promotional-code-subttilte-text"> 
                  :Z4KXLM94
              </p>
              <p id="promotional-code-value"> 
                  #-60.00
              </p>
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

</style>
