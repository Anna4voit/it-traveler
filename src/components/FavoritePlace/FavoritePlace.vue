<script setup>
import FavoritePlaceIconButton from './FavoritePlaceIconButton.vue'
import DeleteIcon from './DeleteIcon.vue'
import EditIcon from './EditIcon.vue'
</script>

<template>
  <section class="text-gray mb-6 last:mb-0">
    <div class="flex gap-4">
      <img class="w-[76px] h-[76px] shrink-0 rounded-md" src="" alt="" />
      <div class="w-full">
        <div class="flex justify-between items-center mb-2">
          <h2 class="font-bold text-sm text-[#2C2C2C]">Палац спорту</h2>
          <div class="flex gap-2">
            <FavoritePlaceIconButton>
              <EditIcon />
            </FavoritePlaceIconButton>
            <FavoritePlaceIconButton>
              <DeleteIcon />
            </FavoritePlaceIconButton>
          </div>
        </div>
        <p class="text-xs line-clamp-3">текст про палац спорту</p>
      </div>
    </div>

    <div class="h-[1px] w-full bg-[#ececec] mt-4"></div>
  </section>
</template>
