<template>
  <div class="about">
    <v-app>
      <v-container>
        <v-col
          :style="{ border: '1px solid' }"
          v-for="n in 3"
          :key="n"
          sm="6"
          md="4"
        >
          {{ n }}
        </v-col>
      </v-container>
      <h1>
        This is an about page123
        <v-btn>
          <v-icon left>mdi-minus-circle</v-icon>
          Accept
        </v-btn>
        {{ test }}
      </h1>
    </v-app>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'

const test = ref('')
</script>
