<template>
<scroll-view class="scroll">
   <text class="heading">Ask a doctor</text>
  <view class="container"> 
    <text class="box-font">Patient Details</text>
    <view class="box1">
         <text-input class="input-text1" placeholder="First Name"> </text-input>
         <text-input class="input-text1" placeholder="Last Name"></text-input>
    </view>
        <view class="box1">
             <text-input class="input-text3" placeholder="Gender"></text-input>
             <text-input class="input-text3" placeholder="Age"></text-input>
              <text-input class="input-text1" placeholder="Contact No"></text-input>
        </view>
        <view class="box1">
         
          <text-input class="input-text2" placeholder="Email"></text-input>
        </view>
        <view class="box1">
           <text-input class="input-text1" placeholder="Address No 1"></text-input>
           <text-input class="input-text1" placeholder="Address No 2"></text-input>
       </view>
        </view>
        <view class="box1">
           <text-input class="input-text1" placeholder="City"></text-input>
           <text-input class="input-text1" placeholder="District"></text-input>
       </view>
        <view class="box1">
           <text-input class="input-text" placeholder="Pincode"></text-input>
            <text-input class="input-text" placeholder="State"></text-input>
             <text-input class="input-text" placeholder="Country"></text-input>
       </view>
       <text class="box-font">Patient Picture</text>
       <view class="box1">
             <text-input class="input-text2" type="image" placeholder="Age"></text-input>
        </view>  
       <view class="box1">
        <text-input class="input-text2" placeholder="Department"></text-input>
      </view> 
      <view class="box1">
             <text-input class="input-text2" placeholder="Patient Background"></text-input>
      </view> 
      <text class="box-font">Patient Question</text>
       <view class="box1">
             <text-input class="input-text2" placeholder="Patient Question"></text-input>
      </view> 
      <view class="box2">
      <touchable-opacity class="button">
        <text class="button-text">Submit</text>
     </touchable-opacity>
      </view> 
 </scroll-view>
</template>
<style>
.input-text{
  background-color: #fff;
  width: 30%;
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
.input-text3{
  background-color: #fff;
  width: 22%;
  padding: 10px;
  border-radius: 10px;
}
.heading{
  color: rgb(97, 13, 13);
  font-size: 30px;
  text-align: center;
   margin-top: 15px;
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
   name: "AskadoctorScreen",
      data: function() {
            return {
                text: ''
            };
        }
    }
 </script>