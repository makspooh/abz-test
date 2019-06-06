<template>
  <div id="app">
    <app-header/>
    <sign-up/>
    <about/>
    <relationships/>
    <requirements/>
    <users/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader'
import SignUp from './components/SignUp'
import About from './components/About'
import Relationships from './components/Relationships'
import Requirements from './components/Requirements'
import Users from './components/Users'

export default {
  components: {
    AppHeader,
    SignUp,
    About,
    Relationships,
    Requirements,
    Users
  },
  data () {
    return {}
  }
}
</script>