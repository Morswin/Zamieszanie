<template>
  <v-app>
    <v-main>
      <v-navigation-drawer rail>
        <v-avatar v-for="n in 5" :key="n" class="ma-2"><v-img src="https://picsum.photos/100/100?random"></v-img></v-avatar>
      </v-navigation-drawer>
      <v-navigation-drawer>Użytkownicy/kanały</v-navigation-drawer>
      <v-card class="h-screen">
        <v-app-bar>Podstawowe interakcje</v-app-bar>
        Czat
        <v-footer app>Input</v-footer>
        <v-navigation-drawer location="right">Info o osobie/aktywni użytkownicy serwera</v-navigation-drawer>
      </v-card>
    </v-main>
  </v-app>
</template>

<script lang="ts" setup>
</script>
