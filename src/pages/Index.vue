<template lang='pug'>
q-page.flex.flex-center
  q-date.full-width(v-model="date" square flat today-btn)
  q-date.full-width(v-model="date" square flat today-btn minimal)
</template>

<script>
export default {
  data() {
    return {
      date: '2019/02/01'
    }
  },
}
</script>

<style lang='sass' scoped>
</style>