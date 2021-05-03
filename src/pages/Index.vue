<template lang='pug'>
q-page.flex.flex-center
  date-picker(v-model="date" is-expanded :rows="2" :attributes="attrs")
</template>

<script>
import Calendar from "v-calendar/lib/components/calendar.umd";
import DatePicker from "v-calendar/lib/components/date-picker.umd";

// Vue.component("calendar", Calendar);
// Vue.component("date-picker", DatePicker);

export default {
  components: {
    Calendar,
    DatePicker,
  },
  data() {
    return {
      date: new Date(),
      attrs: [
        {
          key: 'today',
          highlight: true,
          dates: new Date(),
        }
      ]
    }
  },
}
</script>

<style lang='sass' scoped>
</style>