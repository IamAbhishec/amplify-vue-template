<script setup lang="ts">
import Todos from './components/Todos.vue';
import { Authenticator } from "@aws-amplify/ui-vue";
import "@aws-amplify/ui-vue/styles.css";
</script>

<template>
  <Authenticator v-slot="{ signOut }">
    <main>
      <Todos />
      <button @click="signOut">Sign Out</button>
    </main>
  </Authenticator>
</template>
