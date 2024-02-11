<template>
    <v-card>
        <v-card-subtitle>
            {{ title }}
        </v-card-subtitle>
        <v-card-title>
            {{ amount }}
        </v-card-title>
    </v-card>
  </template>

<style></style>

<script setup>
import { defineProps } from "vue";

defineProps({
  title: String,
  amount: String,
  color: String,
});
</script>
