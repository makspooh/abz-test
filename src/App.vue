<template>
  <div id="app">
    <app-header/>
    <sign-up/>
    <lets-get/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader'
import SignUp from './components/SignUp'
import LetsGet from './components/LetsGet'

export default {
  components: {
    AppHeader,
    SignUp,
    LetsGet
  },
  data () {
    return {}
  }
}
</script>