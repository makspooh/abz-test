<template>
  <div id="app">
    <app-header/>
    <banner/>
    <about/>
    <relationships/>
    <requirements/>
    <users/>
    <sign-up/>
    <app-footer/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader'
import Banner from './components/Banner'
import About from './components/About'
import Relationships from './components/Relationships'
import Requirements from './components/Requirements'
import Users from './components/Users'
import SignUp from './components/SignUp'
import AppFooter from './components/AppFooter'

export default {
  name: 'App',
  components: {
    AppHeader,
    Banner,
    About,
    Relationships,
    Requirements,
    Users,
    SignUp,
    AppFooter
  },
  data () {
    return {}
  }
}
</script>