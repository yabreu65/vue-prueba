<script setup>
const props = defineProps({
  image: String,
  email: String,
  phone: Number,
  address: String,
  name: String,
});
</script>

<template>
  <v-card class="mx-auto w-100 overflow-visible card-shadow">
    <v-img
      class="w-100 transfor"
      style="z-index: 200; position: absolute; top: -42px"
      src="../assets/fabian.png"
      width="100"
      height="100"
    ></v-img>
    <div
      style="
        position: absolute;
        color: #ffffff;
        font-size: 15px;
        top: 98px;

        z-index: 100;
      "
      class="d-flex justify-center w-100"
    >
      <p class="text-center font-weight-medium">
        {{ name }}
      </p>
    </div>
    <div
      class="rounded-t-lg"
      style="
        height: 145px;
        width: 100%;
        overflow: hidden;
        position: relative;
        transition: 0.3s ease-in-out;
      "
    >
      <v-img
        src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
        height="145px"
        style="
          max-width: 100%;
          max-height: 100%;
          transition: transform 0.3s ease-in-out;
          transform-origin: center top;
        "
        class="transfor"
        cover
      ></v-img>
    </div>

    <div class="d-flex align-center">
      <v-avatar size="30">
        <v-img src="../assets/email1.svg" width="18" height="18"></v-img>
      </v-avatar>
      <v-card-title class="text-center pa-0 pt-2" style="margin-top: -8px">
        <span class="text-subtitle-2">{{ email }}</span>
      </v-card-title>
    </div>
    <div class="d-flex align-center">
      <v-avatar size="30">
        <v-img src="../assets/smartphone1.svg" width="18" height="18"></v-img>
      </v-avatar>
      <v-card-title class="text-center pa-0">
        <span class="text-subtitle-2">{{ phone }}</span>
      </v-card-title>
    </div>
    <div class="d-flex align-center">
      <v-avatar size="30">
        <v-img src="../assets/direccion1.svg" width="18" height="18"></v-img>
      </v-avatar>
      <v-card-title class="text-center pa-0 pb-2">
        <span class="text-subtitle-2">{{ address }}</span>
      </v-card-title>
    </div>
  </v-card>
</template>
<style scoped>
.card-shadow:hover {
  box-shadow: 0 0 30px #ddedff;
  transition-delay: 0.5s;
}
.card-shadow:hover .transfor {
  transform: scale(1.2);
}
</style>
