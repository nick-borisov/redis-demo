<template>
  <nav class="site-menu">
    <div class="site-menu__title">
      Dashboard
    </div>
    <ul class="site-menu__list">
      <li class="site-menu__item">
        <button class="site-menu__link color-danger" href="#">
          <span class="site-menu__link-icon">
            <img src="../../assets/img/icon/uil-home.svg" alt=""/>
          </span>
          <span class="site-menu__link-text">
            My Categories
          </span>
          <span class="site-menu__link-arrow">
            <img src="../../assets/img/icon/uil-arrow.svg" alt=""/>
          </span>
        </button>

        <ul class="site-menu__list site-menu__list--level-2">

          <li class="site-menu__item" v-for="(item, index) in menu" :key="index">
            <a
              class="site-menu__link site-menu__link--level-2"
              :style="{color: item.color}"
              :href="item.url"
              >
              <span class="site-menu__link-icon">
                <img src="../../assets/img/icon/uil-tag.svg" alt=""/>
              </span>
              <span class="site-menu__link-text">
                {{ item.name }}
              </span>
              <span class="site-menu__link-count">
                {{ item.count }}
              </span>
            </a>
          </li>

          <li class="site-menu__item">
            <button class="site-menu__link" type="button">
              <span class="site-menu__link-icon">
                <img src="../../assets/img/icon/uil-edit.svg" alt=""/>
              </span>
              <span class="site-menu__link-text">
                Edit Categories
              </span>
            </button>
          </li>
        </ul>

      </li>

      <li class="site-menu__item">
        <a class="site-menu__link" href="#">
          <span class="site-menu__link-icon">
            <img src="../../assets/img/icon/uil-users.svg" alt=""/>
          </span>
          <span class="site-menu__link-text">
            Shared with me
          </span>
          <span class="site-menu__link-count">8</span>
        </a>
      </li>

      <li class="site-menu__item">
        <a class="site-menu__link" href="#">
          <span class="site-menu__link-icon">
            <img src="../../assets/img/icon/uil-trash.svg" alt=""/>
          </span>
          <span class="site-menu__link-text">
            Trash
          </span>
          <span class="site-menu__link-count">1</span>
        </a>
      </li>

    </ul>
  </nav>

</template>

<script>
  export default {
    data() {
      return {
        menu: [
          {
            name: 'Home',
            url: '#',
            count: 8,
            color: '#8E43E7',
          },
          {
            name: 'Personal',
            url: '#',
            count: 25,
            color: '#5FC9F8',
          },
          {
            name: 'Assignments',
            url: '#',
            count: 16,
            color: '#53D769',
          },
        ]
      }
    }
  }
</script>
