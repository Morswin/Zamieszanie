<script lang="ts" setup>
  import ServerIcon from './components/ServerIcon.vue';
  import UserShort from './components/UserShort.vue';
</script>

<template>
  <v-app>
    <v-main>
      <v-navigation-drawer rail>
        <ServerIcon v-for="n in 5" :key="n" />  
      </v-navigation-drawer>
      <v-navigation-drawer>
        <UserShort v-for="n in 5" :key="n" />
      </v-navigation-drawer>
      <v-card class="h-screen">
        <v-app-bar>
          <v-row>
            <v-col>
              <v-form>
                <v-text-field label="Szukaj"></v-text-field>
              </v-form>
            </v-col>
          </v-row>
        </v-app-bar>
        Czat
        <v-footer app>Input</v-footer>
        <v-navigation-drawer location="right">Info o osobie/aktywni użytkownicy serwera</v-navigation-drawer>
      </v-card>
    </v-main>
  </v-app>
</template>

