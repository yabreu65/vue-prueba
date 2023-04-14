<script setup>
import Header from "@/components/Header.vue";
import Usuario from "@/components/Usuario.vue";
import Grill from "@/components/Grill.vue";

const cards = [
  {
    image: "../assets/victoria.png",
    name: "John Doe",
    email: "johndoe@example.com",
    phone: "123-456-7890",

    address: "123 Main St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Maximo Gonzalez",
    phone: "123-456-7890",
    email: "johndoe@example.com",
    address: "123 Main St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Jane Smith",
    phone: "555-555-5555",
    email: "janesmith@example.com",
    address: "456 Park Ave, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Victoria Johnson",
    phone: "555-123-4567",
    email: "bob@example.com",
    address: "789 Oak St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Sarah Lee",
    phone: "555-987-6543",
    email: "sarah@example.com",
    address: "101 Elm St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Mark Davis",
    phone: "555-777-7777",
    email: "mark@example.com",
    address: "222 Maple St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Karen Smith",
    phone: "555-111-2222",
    email: "karen@example.com",
    address: "333 Pine St, Anytown",
  },
  {
    image: "../assets/victoria.png",
    name: "Tom Brown",
    phone: "555-444-4444",
    email: "tom@example.com",
    address: "444 Cedar St, Anytown",
  },
  {
    image: "../assets/victoria.png",
    name: "Laura Rodriguez",
    phone: "555-555-1234",
    email: "laura@example.com",
    address: "555 Oak St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Mike Johnson",
    phone: "555-222-3333",
    email: "mike@example.com",
    address: "666 Elm St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Tina Lee",
    phone: "555-444-5555",
    email: "tina@example.com",
    address: "777 Maple St, Anytown",
  },
  {
    image: "../assets/victoria.png",

    name: "Jason Brown",
    phone: "555-333-2222",
    email: "jason@example.com",
    address: "888 Pine St, Anytown",
  },
];
</script>

<template>
  <v-container>
    <v-row>
      <v-row
        ><v-col
          ><Header
            style="
              border-bottom: 1px solid #eeebf4;
              margin-left: 6px;
            " /><Usuario class="mt-4" /></v-col
      ></v-row>
      <v-row class="ml-6 mr-6">
        <v-col
          class="pa-8"
          v-for="(card, index) in cards"
          :key="card.id"
          xs="12"
          sm="6"
          md="4"
          lg="3"
        >
          <Grill
            :image="card.image"
            :name="card.name"
            :email="card.email"
            :phone="card.phone"
            :address="card.address"
          />
        </v-col>
      </v-row>
    </v-row>
  </v-container>
</template>
