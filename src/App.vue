<template>
  <div id="app">
    <h3>Element: </h3>
    <el-date-picker v-model="value1" type="datetime" placeholder="选择日期时间" time-arrow-control></el-date-picker>
    <h3>vue2-datepicker: </h3>
    <vue2-datepicker v-model="value2"></vue2-datepicker>
    <H3>laydate: </H3>
    <lay-date></lay-date>
    <h3>vue-datepicker-ui: </h3>
<!--    <vue-datepicker-ui></vue-datepicker-ui>-->
    <h3>vuejs-datepicker: </h3>
    <vuejs-datepicker ></vuejs-datepicker>
  </div>
</template>

<script>

import Vue2Datepicker from "@/components/Vue2Datepicker";
import VueDatepickerUi from "@/components/VueDatepickerUi";
import LayDate from "@/components/LayDate";
import VuejsDatepicker from "@/components/VuejsDatepicker";

export default {
  name: 'App',
  components: {
    VuejsDatepicker,
    LayDate,
    VueDatepickerUi,
    Vue2Datepicker,
  },
  data() {
    return {
      value1: '',
      value2: '',
    }
  },
  created() {

  },
  methods: {

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
