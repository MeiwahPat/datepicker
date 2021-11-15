<template>
  <div>
    <date-picker v-model="time" :format="customFormatter"></date-picker>
  </div>
</template>

<script>
  import DatePicker from 'vuejs-datepicker'
  // JavaScript 日期处理类库
  import moment from 'moment'

  export default {
    name: "VuejsDatepicker",
    components: {
      DatePicker
    },
    data() {
      return {
        time: Date.now()
      }
    },
    methods: {
      customFormatter(date) {
        console.log(date)
        return moment(date).format('YYYY-MM-DD H:mm');
      }
    },
  }
</script>

<style scoped>

</style>
