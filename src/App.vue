<script setup>
// import HomepageView from './views/HomepageView.vue'
// import FavoritePlace from './components/FavoritePlace/FavoritePlace.vue'
import FavoritePlaces from './components/FavoritePlaces/FavoritePlaces.vue'
</script>

<template>
  <div class="bg-white h-screen w-[400px]"></div>
  <!-- <FavoritePlaces /> -->
  <!-- <HomepageView /> -->
  <FavoritePlaces>
    <div>THis is super slot</div>
    <template v-slot:label>This is label</template>
    <template #list>This is list</template>
  </FavoritePlaces>
</template>
