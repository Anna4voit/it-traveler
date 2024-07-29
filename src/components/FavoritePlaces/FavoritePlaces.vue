<script setup>
import FavoritePlace from '../FavoritePlace/FavoritePlace.vue'
import IButton from '../IButton/IButton.vue'
import { ref } from 'vue'

const counter = ref(0)

const increment = () => {
  counter.value += 1
}
</script>

<template>
  <div class="px-6">
    <div class="text-gray mb-4">Додані маркери ({{ counter }})</div>
    <!-- <FavoritePlace v-for="n in 4" :key="n" /> -->
    <slot name="label"></slot>
    <slot name="list">
      <FavoritePlace v-for="n in 4" :key="n" />
    </slot>

    <slot></slot>

    <IButton class="w-full mt-10" variant="gradient" @click="increment">Додати маркер</IButton>
  </div>
</template>
