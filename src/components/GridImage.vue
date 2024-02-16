<template>
<v-card class="mt-5 pa-3">
     <v-row >
   <v-col
      v-for="n in 200"
      :key="n"
      xs="4"
      cols="4"
      md="1"
    >
    <v-card>
    <v-img
        :src="`https://picsum.photos/500/300?image=${n * 5 + 10}${props.isWithColor?'':'&grayscale'}`"
        :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}${props.isWithColor?'':'$grayscale'}`"
        aspect-ratio="1"
        cover >
        <template v-slot:placeholder>
          <v-row
            class="fill-height ma-0"
            align="center"
            justify="center"
          >
            <v-progress-circular
              indeterminate
              color="grey-lighten-5"
            ></v-progress-circular>
          </v-row>
        </template>
        
      </v-img>
    </v-card>
   </v-col>
    </v-row>
</v-card>
</template>
<script setup>
import {defineProps} from 'vue'
//eslint-disable-next-line no-unused-vars
const props=defineProps(['isWithColor'])
// eslint-disable-next-line no-unused-vars
// const props = defineProps({
//   isWithColor: Boolean
// })

</script>
