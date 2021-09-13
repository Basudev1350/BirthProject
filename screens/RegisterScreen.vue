<template>
<scroll-view class="scroll">
   <text class="heading">Register</text>
  <view class="container"> 
    <view class="box1">
         <text-input class="input-text1" placeholder="First Name"> </text-input>
         <text-input class="input-text1" placeholder="Last Name"></text-input>
    </view>
        <view class="box1">
               <text-input class="input-text1" placeholder="Mobile No"> </text-input>
               <text-input class="input-text1" placeholder="Landline No"></text-input>
        </view>
        <view class="box1">
          <text-input class="input-text2" placeholder="Email"></text-input>
        </view>
        <view class="box1">
          <text-input class="input-text2" placeholder="Password"></text-input>
         </view>
        <view class="box1">
          <text-input class="input-text2" placeholder="Confirm Password"></text-input>
        </view>
         <view class="box1">
          <switch 
            :on-value-change = "handleChange"
            :value = "value"/>
            <text class="switch"> I Agree with Terms of Services</text>
        </view>
          
      <view class="box2">
      <touchable-opacity class="button">
        <text class="button-text">Submit</text>
     </touchable-opacity>
      </view> 
  </view>
 </scroll-view>
</template>
<style>
.switch{
  color: rgb(97, 13, 13);
  font-size: 18px;
  margin-right: 80px;
}
.input-text{
  background-color: #fff;
  width: 120px;
  padding: 10px;
  border-radius: 5px;
}
.box2{
   align-items: center;
  justify-content: center;
}
.input-text1{
  background-color: #fff;
  width: 47%;
  padding: 10px;
  border-radius: 5px;
}
.input-text2{
  background-color: #fff;
  width: 100%;
  padding: 10px;
  border-radius: 10px;
}
.heading{
  color: rgb(97, 13, 13);
  font-size: 30px;
  text-align: center;
   margin-top: 15px;
   font-weight: bold;
}
.button{
  background-color:rgb(97, 13, 13); 
  padding: 10px;
  width: 200px;
  height: 50px;
  border-radius: 30px;
  margin-top: 15px;
  margin-bottom: 20px;
}
.button-text{
   color: white;
  font-weight: bold;
  font-size: 18px;
  text-align: center;
}
.scroll{
   background-color: rgb(242, 170, 168);
}
.box1{
  padding: 15px; 
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  }
  
.box-font{
  font-size: 20px;
  margin-top: 20px;
  margin-left: 20px;
  color:rgb(97, 13, 13);;
}
.box-sub-font{
  font-size: 16px;
  color: #fff;
  text-align: left;
  margin-top: 10px;
}
.text-color-primary {
  color:rgb(97, 13, 13);
  font-size: 40px;
  margin-top: 15px;
}
.text-color{
  color:rgb(97, 13, 13);
  font-size: 20px;
  margin-top: 15px;
  text-align: center;
}
</style>
 <script>
 export default {
      name:'RegisterScreen',
      data: function() {
            return {
                value: false,
            };
        },
        methods: {
    handleChange: function(val) {
                this.value = val;
                if(this.value==true){
                 alert('Welcome to BIRTH eclinic online. The content of the app (web/mobile), pertains to BIRTH eclinic, is the property of Bengal Infertility & Reproductive Therapy Hospital Pvt. Ltd. (" BIRTH eclinic", the "Company", "we" or "us"), having its registered office at 36B Elgin Road, Kolkata , West Bengal, India, PIN 700020. BIRTH eclinic, is an online web-application channel facilitating healthcare consultation (“services”) with Birth Specialists and Team doctors. It facilities, booking video appointments, clinic appointments or simply asking questions to Birth India doctors.');
                }
                 
            },
        }
    }
 </script>