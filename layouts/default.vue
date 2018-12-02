<template lang="pug">
  div
    nuxt
    div(id="footer")
      b-container
        b-row(class="justify-content-md-center text-center")
          b-col
            h2 ShokuTaku
        b-row(class="justify-content-md-center text-center")
          b-col
            nuxt-link(class="link" to="/terms/privacy") privacy policy
</template>

<style lang="stylus">
#footer
  margin-top 40px
  padding 30px 0
  background-color #E7E7E7
  color #757575
  .link
    color #757575
</style>
