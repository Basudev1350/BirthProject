<template>
<scroll-view class="scroll">
   <text class="heading">Login</text>
  <view class="container"> 
       <view class="box1">
             <text-input class="input-text2" placeholder="Email or Mobile No"></text-input>
              <text-input class="input-text2" placeholder="Password"></text-input>
      </view> 
      <view class="box2">
      <touchable-opacity class="button" @press="goToAskadoctorScreen">
        <text class="button-text" @press="goToAskadoctorScreen">Submit</text>
     </touchable-opacity>
      </view> 
       <text class="forgot-user">Forgot your password?</text>
        <touchableOpacity class="btn" @press="goToRegisterScreen">
       <text class="forgot-user" @press="goToRegisterScreen">New User?</text>
        </touchableOpacity>
  </view>
 </scroll-view>
</template>
<style>
.box2{
   align-items: center;
  justify-content: center;
}
.input-text2{
  background-color: #fff;
  margin-top: 25px;
  width: 380px;
  padding: 10px;
  border-radius: 10px;
}
.heading{
  color: rgb(97, 13, 13);
  font-size: 30px;
  text-align: center;
  margin-top: 25px;
  font-weight: bold;
}
.forgot-user{
  color: #3490dc;
  font-size: 15px;
  text-align: center;
  margin-top: 10px;
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
  }
</style>
 <script>
 export default {
    name:"LoginScreen",
    props: {
    navigation: {
      type: Object
    }
    },
    methods: {
    goToRegisterScreen() {
      this.navigation.navigate("Register");
    },
    goToAskadoctorScreen(){
        this.navigation.navigate("Askadoctor");
    }
  },
      data: function() {
            return {
                text: ''
            };
        }
    }
 </script>