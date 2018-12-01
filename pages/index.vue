<template lang="pug">
  div
    b-container(class="first-view" fluid)
      b-row(class="text-center first-view-row" align-v="center")
        b-col
          div(class="caption")
            h2 ShokuTaku
            p
              | We provide you and your community with amusement
            a(class="discover" href="#product") discover
    b-container(id="product" fluid)
      b-row(class="text-center first-view-row" align-v="center")
        b-col
          div(class="headline") Products
          div(class="line-shape")
      b-row(class="text-center first-view-row section")
        b-col(align-celf="center")
          b-img(src="/img/screenshot1.png")
        b-col(align-celf="center")
          b-row(class="detail")
            h3(class="title") NumberBlockBreaker
            p(class="description")
              | 指一本で簡単操作！自分の数字を増やしつつ、行く手を阻むブロックを壊し続けよう！
              | 君はどれだけ生き延びることができるか？
            div(class="store-link")
              a(href="#")
                img(src="/img/app_store_badge.svg")
              a(href="#")
                img(src="/img/google-play-badge.png")
</template>

<style lang="stylus">
*
  font-family roboto


.first-view
  background-image url('/img/pc/background.png')
  height 900px
  background-size cover
  background-position bottom center
  .first-view-row
    height 100%

.caption
  align-items center
  margin-top -150px
  h2
    font-size 150px
    color white
    margin-bottom -20px

  p
    font-size 40px
    color white

  .discover
    display block
    margin 150px auto 0
    border solid white 2px
    border-radius 60px
    width 400px
    transition all  0.3s ease
    text-decoration none
    font-size 60px
    color white
    &hover
      background-color white
      color #F39B97

#product
  .section
    padding-top 80px
    .title
      font-size 50px

    .description
      padding-top 10px
      width 80%
      font-size 20px
      text-align left

    .store-link
      text-align left
      img
        height 50px
        padding-right 10px

  .headline
    font-size 100px

  .line-shape
    width 15%
    height 5px
    background-color #F0955E
    margin 0 auto

@media screen and (max-width: 400px)
  .first-view
    height 350px

  .caption
    margin-top 0px
    h2
      font-size 45px
      margin-bottom 0

    p
      font-size 13px
      margin-bottom 40px

    .discover
      margin 0 auto
      width 40%
      font-size 20px

  #product
    .headline
      font-size 40px

    .section
      .title
        font-size 25px

    .detail
      padding-top 10px
      .title
        margin 10px auto 0

      .description
        font-size 15px
        margin 10px auto 0
        line-height 25px

      .store-link
        margin-top 15px
        text-align center
        margin 10px auto 0

        a
          display block
          margin-bottom 15px
          img
            height auto
            width 65%

    .line-shape
      width 23%
</style>
