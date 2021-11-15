<template>
  <div>
      <Calendar
        v-model="example.value"
        :range="example.range"
        :lang="example.lang"
        :firstDayOfWeek="example.firstDayOfWeek"
        :input-class="example.inputClass"
        :position="example.position"
        :disabled-start-date="example.disabledStartDate"
        :text-format="example.textFormat"
        :date-format="example.dateFormat"
        :disabled-end-date="example.disabledEndDate"/>

<!--    <calendar :calendar="example" :current-date="example"-->
<!--              selected-date="" :format-date="test"-->
<!--              text-format=""-->
<!--    />-->
  </div>
</template>

<script>
  import Calendar from 'vue-datepicker-ui';

  export default {
    name: "VueDatepickerUi",
    components: {
      Calendar
    },
    data() {
      return {
        example: {
          "title": "First Day Of Week",
          "inputClass": "exampleDatePicker",
          "lang": "en",
          "position": "left",
          "range": true,
          "value": [
            "2020-05-20T01:34:41.250Z",
            "2020-05-29T01:34:41.250Z"
          ],
          "firstDayOfWeek": "sunday"
        }
      }
    },
    created() {

    },
    methods: {
      test() {

      }
    },
  }
</script>

<style scoped>

</style>
