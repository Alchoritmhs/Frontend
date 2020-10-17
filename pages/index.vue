<template>
  <div>
    <header
      style="height: 56px; box-shadow: 0 2px 4px -1px rgba(0, 0, 0, 0.4)"
    ></header>
    <main class="d-flex">
      <aside
        class="d-flex flex-column"
        style="
          width: 400px;
          height: 100vh;
          font-size: 15px;
          border-right: 1px solid rgba(0, 0, 0, 0.05);
        "
      >
        <v-list shaped class="mt-1">
          <v-list-item-group v-model="selectedMenuOption" color="primary">
            <v-list-item :key="0">Документы на подпись</v-list-item>
            <v-list-item :key="1">Подписанные документы</v-list-item>
          </v-list-item-group>
        </v-list>
      </aside>
      <aside
        class="d-flex flex-column ml-1"
        style="
          width: 220px;
          height: 100vh;
          font-size: 14px;
          box-shadow: 10px 0px 10px -10px rgba(0, 0, 0, 0.1);
        "
      >
        <v-list shaped class="mt-1">
          <v-list-item-group color="primary">
            <v-list-item>Документ 1</v-list-item>
            <v-list-item>Документ 2</v-list-item>
          </v-list-item-group>
        </v-list>
      </aside>
      <v-container>
        <!-- <iframe
          src="https://view.officeapps.live.com/op/embed.aspx?src=http://remote.url.tld/path/to/document.doc"
          width="1366px"
          height="623px"
          frameborder="0"
        ></iframe> -->
        <iframe src='https://view.officeapps.live.com/op/embed.aspx?src=http://www.learningaboutelectronics.com/Articles/NP-modernization-act-new-york-state.doc' width='80%' height='565px' frameborder='0'> </iframe>
      </v-container>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedMenuOption: 0,
    }
  },
}
</script>
