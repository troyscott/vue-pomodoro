<template>
  <div class="container">
    <h2>
      <span>Pomodoro</span>
      // Looks like the Conrotls Compoent
      <button>
        <i class="glyphicon glyphicon-play"></i>
      </button>
      <button>
        <i class="glyhpicon glyphicon-pause"></i>
      </button>
      <button>
        <i class="glyphicon glyphicon-stop"></i>
      </button>
    </h2>
    // Looks lie our StateTitleComponent
    <h3>{{ title }}</h3>
    // Looks like our CountdownComponent
    <div class="well">
      <div class="pomodoro-timer">
        <span>{{ min }}</span>:<span>{{ sec }}</span>
      </div>
    </div>
    // Looks like our KittensComponent
    <div class="well">
      <img :src="catImgSrc" />
    </div>
  </div>
</template>

<script>
import ControlComponent from './components/ControlComponent'
import CountdownComponent from './components/CountdownComponent'
import KittensComponent from './components/KittensComponent'
import StateTitleComponent from './components/StateTitleComponent'

export default {
  name: 'App',
  components: {
    ControlComponent,
    CountdownComponent,
    KittensComponent,
    StateTitleComponent
  }
}
</script>

<style>
</style>
