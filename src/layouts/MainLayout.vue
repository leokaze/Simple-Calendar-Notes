<template lang='pug'>
q-layout(view="hHh lpR fFf")
  q-header.bg-primary.text-white(bordered)
    q-toolbar
      q-btn(dense flat round icon="menu" @click="left = !left")
      q-toolbar-title Simple Calendar Notes

  q-drawer(v-model="left" side="left" behavior="mobile" bordered)
  q-page-container
    router-view
  q-footer.bg-grey-8.text-white(bordered)
    q-toolbar
      q-toolbar-title Herramientas


</template>

<script>
export default {
  data() {
    return {
      left: false,
    }
  },
}
</script>

<style lang='sass' scoped>
</style>