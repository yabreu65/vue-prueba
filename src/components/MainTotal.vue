<script setup>
import SideBar from "@/components/SideBar.vue";
import Contenedor from "@/components/Contenedor.vue";
</script>

<template>
  <v-container class="d-flex h-100 ml-0 w-100 pa-0">
    <v-row
      class="d-none d-sm-flex h-75 pb-8"
      style="
        align-self: flex-start;
        border-bottom: 1px solid #eeebf4;
        flex: 0;
        border-right: 1px solid #eeebf4;
      "
    >
      <v-col style="width: 110px; heigth: 96%"><SideBar /></v-col>
    </v-row>
    <v-row class="w-100 mt-0">
      <v-col> <Contenedor /> </v-col>
    </v-row>
  </v-container>
</template>
