<template>
  <div>
    <header
      class="d-flex align-center"
      style="height: 56px; box-shadow: 0 2px 4px -1px rgba(0, 0, 0, 0.4)"
    >
    <v-icon large color="primary" class="ml-16">mdi-briefcase-check</v-icon>
      <v-avatar
        v-if="user"
        @click="user = !user"
        size="36"
        color="red"
        class="ml-auto mr-16"
        style="cursor: pointer"
      >
        <span class="white--text">CJ</span>
      </v-avatar>
      <v-avatar
        v-else
        @click="user = !user"
        size="36"
        color="indigo"
        class="ml-auto mr-16"
        style="cursor: pointer"
      >
        <span class="white--text">Am</span>
      </v-avatar>
    </header>
    <main class="d-flex">
      <aside
        class="d-flex flex-column"
        style="
          width: 400px;
          height: calc(100vh - 56px);
          font-size: 15px;
          border-right: 1px solid rgba(0, 0, 0, 0.05);
        "
      >
        <v-list shaped class="mt-1">
          <v-list-item-group v-model="selectedMenuOption" color="primary">
            <v-list-item :key="0">Документы на подпись</v-list-item>
            <v-list-item :key="1">Подписанные документы</v-list-item>
            <v-list-item :key="2"><template-form /></v-list-item>
          </v-list-item-group>
        </v-list>
      </aside>
      <aside
        class="d-flex flex-column ml-1"
        style="
          width: 220px;
          height: calc(100vh - 56px);
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
      <v-container class="d-flex">
        <!-- 
          https://www.npmjs.com/package/ngx-doc-viewer 
          https://www.npmjs.com/package/mammoth?activeTab=dependents
          https://mike.zwobble.org/projects/mammoth/
        -->
        <iframe
          src="https://view.officeapps.live.com/op/embed.aspx?src=http://www.learningaboutelectronics.com/Articles/NP-modernization-act-new-york-state.doc"
          width="80%"
          height="90%"
          frameborder="0"
        >
        </iframe>
        <v-btn @click="signed=true" :color="signed ? 'success' : 'primary'" class="mx-auto mt-5">{{
          signed ? 'Подписано' : 'Подписать'
        }}</v-btn>
      </v-container>
    </main>
  </div>
</template>

<script>
import TemplateForm from '../components/template-form'
export default {
  components: {
    TemplateForm,
  },
  data() {
    return {
      selectedMenuOption: 0,
      user: true,
      signed: false,
    }
  },
}
</script>
