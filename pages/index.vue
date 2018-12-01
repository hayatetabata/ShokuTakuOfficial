<template lang="pug">
  v-layout(column justify-center align-center)
    v-flex(xs12 sm8 md6)
      div(class="text-xs-center") Show your first view
      v-card
        v-card-title(class="headline") Insert headline
        v-card-text
          p
            | Vuetify is a progressive Material Design component framework for Vue.js.
            | It was designed to empower developers to create amazing applications.
          p
            | Thank you for developing with Vuetify
            | and I look forward to bringing more exciting features in the future.
          hr(class="my-3")
        v-card-actions
          v-spacer
          v-btn(color="primary" flat nuxt to="/#inspire") Continue
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>
