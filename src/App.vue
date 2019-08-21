<template>
  <div id="app">
    <SiteHeader
      logoImage="https://www.qbrobotics.com/wp-content/uploads/2018/03/sample-logo-170x150.png"
      logoTitle="Organizer"
      logoSubtitle="Home"
      userEmail="gregory.murphy@example.com"
      userName="Gregory Murphy"
      userPhoto="https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260"
    />
  </div>
</template>

<script>
import './assets/scss/general.scss'
import SiteHeader from './components/SiteHeader'

export default {
  name: 'app',
  components: {
    SiteHeader,
  }
}
</script>
