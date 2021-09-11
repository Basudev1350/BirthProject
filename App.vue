<template>
  <app-navigator></app-navigator>
</template>

<script>
import { createAppContainer } from "react-navigation";
import { createStackNavigator } from "react-navigation-stack";

import HomeScreen from "./screens/HomeScreen.vue";
import LoginScreen from "./screens/LoginScreen.vue";
import RegisterScreen from "./screens/RegisterScreen.vue";
import AskadoctorScreen from "./screens/AskadoctorScreen.vue";
const StackNavigator = createStackNavigator(
  {
    Home:     HomeScreen,
    Login:    LoginScreen,
    Register: RegisterScreen,
    Askadoctor: AskadoctorScreen
  },
  {
    initialRouteName: 'Home',
  }
);

const AppNavigator = createAppContainer(StackNavigator);

export default {
  components: { AppNavigator },
}
</script>