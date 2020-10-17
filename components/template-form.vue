<template>
  <v-dialog v-model="dialog" persistent max-width="600px">
    <template v-slot:activator="{ on, attrs }">
      <span v-bind="attrs" v-on="on"> Создать документ по шаблону </span>
    </template>
    <v-card>
      <v-card-title>
        <span class="headline">Поля шаблона</span>
      </v-card-title>
      <v-card-text>
        <v-container>
          <v-text-field label="Поле" />
          <v-text-field label="Поле" />
          <v-text-field label="Поле" />
          <v-text-field label="Поле" />
          <v-text-field label="Поле" />
          <v-text-field label="Поле" />
        </v-container>
      </v-card-text>
      <v-card-actions>
        <v-spacer></v-spacer>
        <v-btn color="blue darken-1" text @click="dialog = false">
          Закрыть
        </v-btn>
        <v-btn color="blue darken-1" text @click="dialog = false">
          Создать
        </v-btn>
      </v-card-actions>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
    }
  },
}
</script>

<style>
</style>