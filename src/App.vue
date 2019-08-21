<template>
  <main id="app" class="page">
    <div class="page__header">
      <SiteHeader
        logoImage="https://www.qbrobotics.com/wp-content/uploads/2018/03/sample-logo-170x150.png"
        logoTitle="Organizer"
        logoSubtitle="Home"
        userEmail="gregory.murphy@example.com"
        userName="Gregory Murphy"
        userPhoto="https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260"
      />
    </div>

    <div class="page__sidebar">
      <div class="page__sidebar-item">
        <SiteMenu/>
      </div>
      <div class="page__sidebar-footer">
        <div class="page__sidebar-item">
          <Button
            text="new task"
            />
        </div>
        <div class="text-h4 color-gray">
          &copy; 2019 Organaizer Home.<br>
          All rights reserved.
        </div>
      </div>
    </div>

    <div class="page__content">

      <div class="page__toolbar">
        <div class="page__toolbar-title">
          <h1>Hi, Gregory Murphy</h1>
        </div>
        <div class="page__toolbar-sort">

        </div>
        <div class="page__toolbar-add">
          <Button
            rounded
            large
            text="+"
            />
        </div>
      </div>

      <EventList/>

    </div>

    <div class="page__sidebar page__sidebar--right">

    </div>

  </main>
</template>

<script>
import SiteHeader from './components/SiteHeader'
import SiteMenu from './components/SiteMenu'
import EventList from './components/EventList'

import Button from './widgets/Button'

import './assets/scss/general.scss'

export default {
  name: 'app',
  components: {
    SiteHeader,
    SiteMenu,
    Button,
    EventList
  }
}
</script>
