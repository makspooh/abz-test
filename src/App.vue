<template>
  <v-app>
    <v-content>
      <app-header/>
      <banner/>
      <about/>
      <relationships/>
      <requirements/>
      <users/>
      <sign-up/>
    </v-content>
  </v-app>
</template>

<script>
import AppHeader from './components/AppHeader'
import Banner from './components/Banner'
import About from './components/About'
import Relationships from './components/Relationships'
import Requirements from './components/Requirements'
import Users from './components/Users'
import SignUp from './components/SignUp'

export default {
  name: 'App',
  components: {
    AppHeader,
    Banner,
    About,
    Relationships,
    Requirements,
    Users,
    SignUp
  },
  data () {
    return {}
  }
}
</script>