<template>
  <article class="event-card">
    <header class="event-card__header">
      <h2 class="event-card__title text-h2">
        {{ title }}
      </h2>
      <button class="event-card__control" type="button">
        <img src="../../assets/img/icon/uil-ellipsis.svg" alt="">
      </button>
    </header>
    <div class="event-card__description" v-if="description">
      {{ description }}
    </div>
    <footer class="event-card__footer">
      <time class="event-card__date" v-if="date">
        {{ date }}
      </time>
      <div class="event-card__users">
        <div class="event-card__users-item" v-for="(item, index) in users" :key="index">
          <img :src="item.photo" :alt="item.name"/>
        </div>
      </div>
    </footer>
  </article>
</template>

<script>
  export default {
    props: {
      title: String,
      description: String,
      date: String,
      users: Array,
    }
  }
</script>
