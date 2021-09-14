<template>
  <app-navigator></app-navigator>
</template>

<script>
import { createAppContainer } from "react-navigation";
import { createBottomTabNavigator } from "react-navigation-tabs";
// import {  createMaterialTopTabNavigator } from "react-navigation-tabs";
import { createStackNavigator } from "react-navigation-stack";
import * as React from 'react';
import Icon from 'react-native-vector-icons/FontAwesome5';

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
const TabNavigator = createBottomTabNavigator(
  {
   Home: {
        screen: HomeScreen, 
        navigationOptions: {
            tabBarLabel: 'Home', 
            tabBarIcon: <Icon name="home" size={25} color=""/>,
        }
    }, 
    Login: {
        screen: LoginScreen, 
        navigationOptions: {
            tabBarLabel: 'Login', 
            tabBarIcon: <Icon name="sign-in-alt" size={25} color=""/>,
        }
    }, 
    Register: {
        screen: RegisterScreen, 
        navigationOptions: {
            tabBarLabel: 'Register' ,
            tabBarIcon: <Icon name="user" size={25} color=""/>, 
           
        }
    },
    Askadoctor: {
        screen: AskadoctorScreen, 
        navigationOptions: {
            tabBarLabel: 'Ask A Doctor', 
            tabBarIcon: <Icon name="user-shield" size={25} color=""/>, 
        }
    }
  }
);
const StackNavigator = createStackNavigator(
  {
    TabNavigator,
    IOSTabs
  }
);
const AppNavigator = createAppContainer(StackNavigator);
export default {
  components: {
     AppNavigator,
     
    
   }
}
</script>