<template>
  <div id="app">
    <main>
      <project-header :menuData="mainMenuData"></project-header>
    <!-- <ul>
      <li v-for="(person, index) in projectData.people" :key="index">{{ person.name }} {{index}}</li>
    </ul> -->
    <router-view/>
    </main>
    <project-footer :menuData="mainMenuData"></project-footer>
  </div>
</template>

<script>

import ProjectHeader from './components/shared/project-header.vue';
import ProjectFooter from './components/shared/project-footer.vue';
import {someData, mainMenuData} from './projectData.js';

export default {
  data () {
    return {
      projectData: someData,
      mainMenuData
    }
  },
  components: {
    ProjectHeader: ProjectHeader,
    ProjectFooter: ProjectFooter
  }
}
</script>

<style lang="scss">
  main {
    padding-top: 80px;
    min-height: 50vh;
  }
</style>
