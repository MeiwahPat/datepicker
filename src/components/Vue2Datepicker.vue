<template>
  <DatePicker v-model="time" type="datetime"></DatePicker>
</template>

<script>
  import DatePicker from 'vue2-datepicker';
  import 'vue2-datepicker/index.css';

  export default {
    name: "Vue2Datepicker",
    components: {
      DatePicker
    },
    props: {
      value: {
        type: [Number, String],
        default: 0
      },
    },
    data() {
      return {
        time: null
      }
    },
    watch: {
      value(newValue, oldValue) {
        this.time = newValue
      }
    },
    created() {
      this.time = this.value
    }
  }
</script>

<style scoped>

</style>
