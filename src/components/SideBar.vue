<template>
     <v-navigation-drawer
        expand-on-hover
        rail
      > 
      <v-list>
          <v-list-item
            prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
            title="Arockiaraj"
            subtitle="arajmsc@gmailcom"
          ></v-list-item>
        </v-list>
          <v-divider></v-divider>

        <v-list density="compact" nav>
          <v-list-item prepend-icon="mdi-folder" title="Color" value="Color View" @click="$emit('selectOption',true)"></v-list-item>
          <v-list-item prepend-icon="mdi-account-multiple" title="Grey" value="Grey"  @click="$emit('selectOption',false)"></v-list-item>
         
        </v-list>
      

      </v-navigation-drawer>
      
</template>

<script >
  // script setup logic
//  import {defineEmits} from 'vue';
  //defineEmits(['selectOption'])
//   export default {
//     setup(context)
//   {
//     function selectOption(iscolor){
//     context.emit("selectOption",iscolor)

//      }
//      return selectOption;
//   }

//   }
  
  
</script>


