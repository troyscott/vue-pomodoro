<template>
<div>
  <div class="well">
    <div class="pomodoro-timer">
      <span>{{ min | leftpad }}:{{ sec | leftpad }}</span>
    </div>
  </div>
</div>
</template>

<script>
export default {
  data () {
    return {
      min: 0,
      sec: 59
    }
  }
}
</script>

<style scoped>

</style>
