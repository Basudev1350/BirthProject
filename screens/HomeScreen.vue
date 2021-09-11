<template>
<scroll-view class="scroll">
         <view class="box1">
          <view class="box12">
          <text class="box-font">Ask a doctor</text>
           <touchableOpacity class="btn" @press="goToHomeScreen">
           <text class="text" @press="goToHomeScreen">Book Now1</text>
          </touchableOpacity>
       </view>
       <view class="box2">
          <text class="box-font">Rs: 250</text>
          <text class="box-sub-font">Submit Patient Details Upload Reports & Prescriptions Fees: Rs.100.00</text>
       </view>
        </view>
          <view class="box1">
          <view class="box12">
          <text class="box-font">Video Appointment</text>
          <touchableOpacity class="btn" >
           <text class="text">Book Now</text>
           </touchableOpacity>
          </view>
          <view class="box2">
          <text class="box-font">Rs: 250</text>
          <text class="box-sub-font">Currently On-line Booking Not Available. Please Whatsapp to 9830037217 to Book Video Appointment</text>
          </view>
        </view>
        <view class="box1">
         <view class="box12">
          <text class="box-font">Clinic Appointment</text>
          <touchableOpacity class="btn">
           <text class="text">Book Now</text>
           </touchableOpacity>
           </view>
          <view class="box2">
          <text class="box-font">Rs: 250</text>
          <text class="box-sub-font">Submit Patient Details Book Clinic Appointment Fees: Dr Khastgir Rs.2000.00 Team Doctor Rs.2000.00</text>
        </view>
        </view>
 </scroll-view>
</template>
<style>
.btn{
  background-color:#fff;
  border-radius: 25px;
  padding: 10px;
  color: #fff;
}
.text{
  color: #000;
   font-weight: bold;
}
.scroll{
   padding: 5px;
   background-color: rgb(242, 170, 168);
}
.box1{
  border-radius: 20px;
  margin-top: 10px;
  width:400px ;
  height: 200px;
  background-color: rgb(97, 13, 13);
  padding: 30px; 
  }
  .box2{
    margin-top: 10px;
  }
.box-font{
  font-size: 20px;
  color: #fff;
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
 .box12{
     display: flex;
   flex-direction: row;
  justify-content: space-between;
 }
 
 </style>
 <script>
 export default {
     name:"HomeScreen",
      props: {
    navigation: {
      type: Object
    }
  },
  methods: {
    goToHomeScreen() {
      this.navigation.navigate("Login");
    }
  }
    }
 </script>