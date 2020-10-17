<template>
  <v-card
    class="d-flex flex-column mx-auto"
    width="400"
    height="300"
    style="margin-top: 20vh"
  >
    <v-card-text class="text-center" style="font-size: 20px">
      Вход
    </v-card-text>
    <v-form class="d-flex flex-column align-center px-6">
      <v-text-field
        v-model="firstname"
        label="Логин"
        style="width: 100%"
      />
      <v-text-field
        v-model="firstname"
        label="Пароль"
        style="width: 100%"
      />
      <v-btn @click="$router.replace('/')" class="mt-3" width="120">Войти</v-btn>
    </v-form>
  </v-card>
</template>

<script>
export default {}
</script>

<style>
</style>