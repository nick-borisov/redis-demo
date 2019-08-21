<template>
  <button
    class="button"
    :class="classes"
    v-bind="attributes"
    @click="onClick"
    >
    <span class="button__content">
      <span class="button__icon" v-if="icon">
        <img :src="icon" alt="">
      </span>
      <span class="button__text" v-if="text">
        {{ text }}
      </span>
    </span>
  </button>
</template>

<script>
  export default {
    name: 'VButton',
    props: {
      large: Boolean,
      rounded: Boolean,
      icon: String,
      text: String,
      type: {
        type: String,
        default: 'button'
      },
    },

    methods: {

      onClick() {
        this.$emit('click')
      },

    },

    computed: {

      attributes() {
        return {
          ...this.$attrs,
          type: this.type,
          disabled: this.disabled,
        }
      },

      classes() {
        return {
          'button--rounded': this.rounded,
          'button--large': this.large,
        }
      },

    }

  }
</script>
