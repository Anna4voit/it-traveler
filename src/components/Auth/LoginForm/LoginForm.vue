<script setup>
import { reactive } from 'vue'
import IInput from '../../IInput/IInput.vue'
import FormContainer from '../FormContainer.vue'
import IButton from '../../IButton/IButton.vue'
const emit = defineEmits(['submit'])
const userData = reactive({
  email: '',
  password: ''
})
</script>

<template>
  <FormContainer @submit.prevent="emit('submit', userData)">
    <IInput
      class="mb-4"
      label="Електронна пошта"
      placeholder="email@gmail.com"
      v-model="userData.email"
    />
    <IInput type="password" label="Пароль" v-model="userData.password" />
    <IButton class="mt-10 w-full" variant="gradient" type="submit">Увійти </IButton>
  </FormContainer>
</template>
