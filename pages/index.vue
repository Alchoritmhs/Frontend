<template>
  <div>
    <header
      style="height: 56px; box-shadow: 0 2px 4px -1px rgba(0, 0, 0, 0.4)"
    ></header>
    <main class="d-flex">
      <aside
        class="d-flex flex-column pl-3 pr-5"
        style="
          width: 370px;
          height: 100vh;
          font-size: 15.5px;
          box-shadow: 10px 0 10px -10px rgba(0, 0, 0, 0.2);
        "
      >
        <div class="py-2" style="color: rgba(0, 0, 0, 0.6)">
          Документы на подпись
        </div>
        <div class="py-2 indigo--text text--lighten-1" style="">
          Подписанные документы
        </div>
      </aside>
      <aside
        class="d-flex flex-column pl-3 pr-5"
        style="
          width: 200px;
          height: 100vh;
          font-size: 14px;
          box-shadow: 10px 0px 10px -10px rgba(0, 0, 0, 0.2);
        "
      >
        <div class="py-2 indigo--text text--lighten-1" style="">Документ 1</div>
        <div class="py-2" style="color: rgba(0, 0, 0, 0.6)">Документ 2</div>
      </aside>
      <v-container> Документ 1... </v-container>
    </main>
  </div>
</template>

<script>
export default {}
</script>
