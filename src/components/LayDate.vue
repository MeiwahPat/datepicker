<template>
  <div>
    <input :id="id" type="text"/>
  </div>
</template>

<script>
  export default {
    name: "LayDate",
    props: {
      id: {
        type: [Number, String],
        default: () => 'lay-date-' + new Date().getTime()
      },
    },
    data() {
      return {
        time: ''
      }
    },
    created() {
      console.log(laydate)
      laydate.render({
        elem: '#'  + this.id,
        type: 'datetime',
        format: 'yyyy-MM-dd HH:mm',
        done: value => {
          console.log(value)
          this.time = value;
        }
      })
    }
  }
</script>

<style scoped>

</style>
