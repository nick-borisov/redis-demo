<template>
  <div class="event-list">
    <ul class="event-list__content">
      <li class="event-list__content-item" v-for="(item, index) in list" :key="index">
        <EventCard
          :title="item.title"
          :description="item.description"
          :date="item.date"
          :users="item.users"
          />
      </li>
    </ul>
    <Pagination/>
  </div>
</template>

<script>
  import EventCard from '../EventCard'
  import Pagination from '../Pagination'

  export default {
    components: {
      EventCard,
      Pagination,
    },
    data() {
      return {
        list: [
          {
            title: 'Task 01',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit...',
            date: 'AUG 16, 2019 20:00',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
              {
                name: 'Alex 2',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              }
            ]
          },
          {
            title: 'Task 02',
            description: '',
            date: 'AUG 16, 2019 20:00',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
            ]
          },
          {
            title: 'Task 03',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit...',
            date: '',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
              {
                name: 'Alex 2',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              }
            ]
          },
          {
            title: 'Task 04',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit...',
            date: 'AUG 16, 2019 20:00',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
              {
                name: 'Alex 2',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              }
            ]
          },
          {
            title: 'Task 05',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit...',
            date: 'AUG 16, 2019 20:00',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
              {
                name: 'Alex 2',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              }
            ]
          },
          {
            title: 'Task 06',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit...',
            date: 'AUG 16, 2019 20:00',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
              {
                name: 'Alex 2',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              }
            ]
          },
          {
            title: 'Task 07',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit...',
            date: 'AUG 16, 2019 20:00',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
              {
                name: 'Alex 2',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              }
            ]
          },
          {
            title: 'Task 08',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit...',
            date: 'AUG 16, 2019 20:00',
            users: [
              {
                name: 'Alex',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              },
              {
                name: 'Alex 2',
                photo: 'https://images.pexels.com/photos/614810/pexels-photo-614810.jpeg?auto=compress&cs=tinysrgb&dpr=3&h=750&w=1260'
              }
            ]
          },
        ]
      }
    }
  }
</script>
