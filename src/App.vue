<template>
  <v-app> 
    <sideBar  @selectOption="selectOne"/>
    <v-main>
      <GridImage :isWithColor="isWithColor"/>
    </v-main>
  </v-app>
</template>

<script setup>

import sideBar from './components/SideBar.vue'
import GridImage from './components/GridImage.vue'
import {ref} from 'vue'
const isWithColor=ref(true)
function selectOne(iscolor)
{
    isWithColor.value=iscolor;
    //alert(isWithColor.value)
}
</script>