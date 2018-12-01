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
          div(class="headline") Product
          div(class="line-shape")
      b-row(class="text-center first-view-row section")
        b-col(align-celf="center")
          b-img(src="/img/screenshot1.png")
        b-col(align-celf="center")
          b-row
            h3(class="title") NumberBlockBreaker
          b-row
            p(class="description")
              | 指一本で簡単操作！自分の数字を増やしつつ、行く手を阻むブロックを壊し続けよう！
              | 君はどれだけ生き延びることができるか？
          b-row(class="store-link")
            b-col
              a(href="#")
                img(src="/img/app_store_badge.svg" style="width: 35%;")
              a(href="#")
                img(src="/img/google-play-badge.png" style="width:45%;")
</template>

<style lang="stylus">
.first-view
  background-image: url('/img/pc/background.png')
  height: 900px
  background-size: cover
  background-position: bottom center
  .first-view-row
    height: 100%

.caption
  align-items: center
  font-family: roboto
  margin-top: -150px
  h2
    font-size: 150px
    color: white
    margin-bottom: -20px

  p
    font-size: 40px
    color: white

  .discover
    display: block
    margin: 150px auto 0
    border: solid white 2px
    border-radius: 60px
    width: 400px
    transition: all  0.3s ease
    text-decoration: none
    font-size: 60px
    color: white
    &:hover
      background-color: white
      color: #F39B97

#product
  .section
    padding-top: 80px
    .title
      font-size: 50px

    .description
      padding-top: 10px
      width: 80%
      font-size: 20px
      text-align: left

    .store-link
      text-align: left

  .headline
    font-size: 100px

  .line-shape
    width: 80px
    height: 5px
    background-color: #F0955E
    margin: 0 auto
</style>
