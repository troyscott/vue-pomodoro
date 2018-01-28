<template>
  <div class="container">
    <h2>
      <span>Pomodoro</span>
      <control-component></control-component>
    </h2>
    <state-title-component></state-title-component>
    <countdown-component></countdown-component>
    <transition name="fade">
      <kittens-component v-if="kittens"></kittens-component>
    </transition>
  </div>
</template>

<script>
import ControlComponent from './components/ControlComponent'
import CountdownComponent from './components/CountdownComponent'
import KittensComponent from './components/KittensComponent'
import StateTitleComponent from './components/StateTitleComponent'

window.data = {
  kittens: true
}

export default {
  name: 'App',
  data () {
    return window.data
  },
  components: {
    ControlComponent,
    CountdownComponent,
    KittensComponent,
    StateTitleComponent
  }
}
</script>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s
}
.fade-enter, .fade-leave-active {
  opacity: 0
}

</style>
