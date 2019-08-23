<template>
  <div>
    <header>{{title}}</header>
    <div>{{content}}</div>
  </div>
</template>

<script>
export default {
  name: 'NewComponent',
  data () {
    return {
      title: 'New Component',
      content: 'Creating Components in Vue is easy'
    }
  }
}
</script>

<style lang="scss">



</style>