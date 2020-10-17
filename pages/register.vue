<template>
  <v-card
    class="d-flex flex-column mx-auto"
    width="400"
    style="margin-top: 20vh"
  >
    <v-card-text class="text-center" style="font-size: 20px">
      Регистрация
    </v-card-text>
    <v-form class="d-flex flex-column align-center px-6">
      <v-text-field label="Имя" style="width: 100%" />
      <v-text-field label="Фамилия" style="width: 100%" />
      <v-text-field label="Отчество" style="width: 100%" />
      <v-text-field label="Почта" style="width: 100%" />
      <v-btn @click="$router.replace('/')" class="mt-3 my-6" width="120"
        >Вперед!</v-btn
      >
    </v-form>
  </v-card>
</template>

<script>
export default {}
</script>

<style>
</style>