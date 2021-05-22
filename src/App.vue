<template>
  <div id="app" class="app">
    <div class="container">
      <link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Fira+Sans&display=swap" rel="stylesheet">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
       
        <div class="division">  </div>
       
        <div class="payment-information-section">
            <div class="card-type">
              <p class="payment-title">
                Payment Information
              </p>
              <p class="payment-subtitle">
                Choose your method of payment
              </p>
              <img class="credit-card-image" src="/card_image.jpg" alt="Credit Card image">
            </div>
            <div class="card-details">
                <div class="payment-type">
                    <img class="payment-logo visa-image" src="/visa-icon.png" alt="Visa">
                    <img class="payment-logo discover-image" src="/discover-logo.png" alt="Discover">
                  <div class="paypal-selector">  
                    <input type="radio" id="paypal-radio-button" class="block-display paypal-radio-button" name="gender" value="paypal">
                    <img class="payment-logo paypal-image" src="/paypal-logo.png" alt="PayPal">
                  </div>
                </div>
                <div class="card-input-details">
                    <form action="/card-details">
                      <div class="first-input-field flex-row">
                          <div class="input-field">
                            <label class="light-label" for="credit-card-no">Credit card number</label>
                            <input type="text" id="credit-card-no" class="text-input-field" value="4324 5433 9382 1030">
                          </div>  
                          <div class="input-field">
                            <label class="light-label" for="expiration-date">Expiration date</label>
                            <input type="text" id="expiration-date" class="text-input-field" value="03/24"><br><br>
                          </div>
                      </div>    
                      <div class="second-input-field flex-row">
                          <div class="input-field">
                            <label class="light-label" for="security-code">Security code</label>
                            <input type="text" id="security-code" class="text-input-field" value="420">
                          </div>
                          <div class="input-field">
                            <label class="light-label" for="postal-code">Postal Code</label>
                            <input type="text" id="Postal Code" class="text-input-field" value="10119"><br><br>
                          </div>
                      </div>
                      <div class="flex-only">
                          <input type="radio" id="card-radio-button" class="block-display" name="gender" value="card" checked="checked">
                          <p class="card-info">Use this card for next time purchase </p>
                        </div> 
                         
                       <input type="submit" class="long-blue-button blue-button" value="Add Card">
                      
                    </form>
                </div>
            </div>
        </div>
        
        <div class="division">  </div>
        
        <div class="payment-details-section">
          <div class="sub-total-div flex-row">
              <p class="subtotal-text bold-payment-information"> 
                Subtotal
              </p>
              <div class="price"> 
                  <p class="subtotal-value figure"> 
                    <span>&#8358;</span>2,497.00
                  </p>
              </div> 
          </div>
          <div class="sub-total-div flex-row">
              <p class="estimated-tax-text bold-payment-information"> 
                  Estimated TAX
              </p>
              <div class="price"> 
                  
                  <p class="estimated-tax-value figure"> 
                    <span>&#8358;</span>119.64
                  </p>
              </div> 
          </div>
          <div class="sub-total-div flex-row">
              <div class="promotional-code flex-row">
                <p class="promotional-code-text bold-payment-information"> 
                    Promotional Code: 
                </p>
                <p class="promotional-code-subttilte-text light-text"> 
                     Z4KXLM94
                </p>
              </div>
              <div class="price"> 
                  <p class="promotional-code-value figure"> 
                     <span>&#8358;</span>-60.00
                  </p>
              </div> 
          </div>
        </div>
        
        <div class="division">  </div>
        
        <div class="payment-accept-section"> 
            <input type="submit" class="blue-button" value="Complete payment">
            <div class="total-figure flex-row">
                <p id="payment-accept-total">TOTAL:</p>
                <div class="price payment-section"> 
                  <p class="payment-accept-text"> <span>&#8358;</span>2556.64</p>
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
}

p{
  font-family: 'Fira Sans', sans-serif;
}

/* Text Fields Style*/
input:focus, textarea:focus, select:focus, button:focus{
    outline: #2762BC;
    border:1px solid #2762BC;
    box-shadow: 0 0 4px #719ECE;
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
  margin: 0px 0px 80px 0px;
}

.sub-menu p{
  margin: 20px;
  font-size: 17px;
  font-family: 'Fira Sans', sans-serif;
  font-weight: 550;
  color:#052a75fd;
}

.profile-image{
  width: 50px ;
  margin: 0px 0px 0px 50px;
}

.main-details{
  clear: both;
}

.payment-information-section{
  display: flex;
  justify-content: space-between;
  margin: 20px 0px;
}

.credit-card-image{
  width: 400px;
}

.payment-title{
  font-size: 18px;
  font-weight: 550;
}

.payment-subtitle{
  font-size: 14px;
  color: lightgray;
}

.payment-type{
  display: flex;
  align-items: center;
  justify-content: space-between;
  float: right;
}

.payment-logo{
  /* height: 50px; */
  margin: 10px;
  width: 40px;
  /* border:1px solid; */
}

.visa-image{
  margin: 0px 0px 20px 0px;
}
.discover-image{
  /* border:1px solid; */
  width: 50px;
  margin: 0px 0px 30px 10px;
}

.paypal-selector{
  /* border:1px solid; */
  display: flex;
  margin: 0px 0px 30px 60px;
}

.paypal-radio-button{
  margin: 26px 0px 0px 0px;  
}

.paypal-image{
  /* border:1px solid; */
  width: 70px;
  margin: 00px 0px -10px 20px;
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

.light-label{
  display: block;
  font-size: 14px;
  font-weight: 500;
  margin: 0px 0px 5px 0px;
  font-family: 'Fira Sans', sans-serif;
  color: hsl(227, 71%, 11%);
}

.text-input-field{
  height: 38px;
  padding-left: 10px;
  font-family: 'Fira Sans', sans-serif;
  color: hsl(227, 71%, 11%);
  background-color: #f0f1f3;
  border-color:#c7d3e6;
  border-radius: 4px;
  border-style: solid;
  margin: 10px 0px 10px 0px;
  width: 250px;
}

.flex-only{
  display: flex;
}

.card-radio-button{

}

.card-info{
  margin: 2px 0px 10px 10px;
}

.first-input-field{
  /* margin: 20px 0px 15px 0px; */
}

.second-input-field{
  /* margin: 20px 0px 15px 0px; */
}

.flex-row{
  display: flex;
  justify-content: space-between;
}

.figure{
  float: right;
  /* color:#424859; */
  font-weight: 700;
}

.division{
  border: solid #d3d3d3;
  border-width: 0px 0px 0.1px 0px ;
}

.payment-details-section{
  margin: 30px 0px 60px 0px;
}

.bold-payment-information{
   font-size: 16px;
   font-weight: 550;
   font-family: 'Fira Sans', sans-serif;
}

.light-text{
  color: hsla(0, 1%, 63%, 0.836);
  margin-left: 5px;
}

.payment-accept-section{
  display: flex;
  justify-content: space-between;
  margin: 30px 0px;
}

.payment-accept-section p{
  font-weight: 700;
  font-size: 18px;
}


.blue-button{
  color: white;
  width: 200px;
  height: 44px;
  font-family: 'Fira Sans', sans-serif;
  font-size: 16px;
  font-weight: 500;
  background: hsl(226, 76%, 48%);
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

@media screen and (max-width: 450px){

}

@media screen and (max-width: 1150px){

}
</style>
