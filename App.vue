<template>
  <app-navigator></app-navigator>
</template>

<script>
import { createAppContainer } from "react-navigation";
import { createBottomTabNavigator } from "react-navigation-tabs";
// import {  createMaterialTopTabNavigator } from "react-navigation-tabs";
import { createStackNavigator } from "react-navigation-stack";

import HomeScreen from "./screens/HomeScreen.vue";
import LoginScreen from "./screens/LoginScreen.vue";
import RegisterScreen from "./screens/RegisterScreen.vue";
import AskadoctorScreen from "./screens/AskadoctorScreen.vue";
const IOSTabs = createBottomTabNavigator(
  {
    Home:     HomeScreen,
    Login:    LoginScreen,
    Register: RegisterScreen,
    Askadoctor: AskadoctorScreen
  }
);
const AndroidTabs = createBottomTabNavigator(
  {
   Home:     HomeScreen,
    Login:    LoginScreen,
    Register: RegisterScreen,
    Askadoctor: AskadoctorScreen
  }
);
const StackNavigator = createStackNavigator(
  {
    AndroidTabs,
    IOSTabs
  }
);
const AppNavigator = createAppContainer(StackNavigator);
export default {
  components: { AppNavigator }
}
</script>
<style>

</style>