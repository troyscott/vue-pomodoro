<template>
  <div>
    <h3>{{ isworking ? workingtitle : restingtitle }}</h3>
  </div>
</template>

<script>
export default {
  data () {
    return {
      workingtitle: 'Work!',
      restingtitle: 'Rest!'
    }
  },
  props: ['isworking']
}
</script>

<style scoped>

</style>
