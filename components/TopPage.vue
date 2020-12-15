<template lang="pug">
  div
    header
      .header-title
        .header-title__img
          img(src="/imgs/header-tree.svg")
        .header-title__text
          p.first-companyname
            | 秩父・荒川の「森の窓口」
            br
          p.companyname
            | 秩父木材協会組合
      .header-body
        a
          span 組合について
        a
          span  木材利用について
        a
          span  活用事例
        a
          span  秩父木材について
        a
          span  組合員紹介
        a
          span  お知らせ
        a
          span  Q&A
      .header-contact
        a(href="#")
          img(src="/imgs/header-mail.svg")
          br
          span  お問い合わせ
    main
      section.top-mv
        .top-mv__contents
          img(src="/imgs/top-mv-text.svg")
          button.button-primary
            span  木材を使いたいと思ったら、まずはこちら
          br
          a
            span  秩父木材共同組合について
        .top-mv__balloon
          .balloon.balloon--1
            .balloon-img
              img(src="/imgs/top-mv-bubble.svg")
            .balloon-text
              p 学校を木造にしたい！
      section.top-case_study
        .container
          .title
            .title__img
              img(src="/imgs/title-bg.svg")
              .title__text
                h2 木材の活用事例
          .top-case_study__body
            .card-list
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎
              .card
                .card__img
                  a(href="#")
                    img(src="/imgs/noimage.svg")
                .card__text
                  a(href="#")
                    span 秩父市役所合同庁舎

          .top-case_study__button
            button.button-primary
              span  すべての事例を見る　>
      section.top-info
        .container




</template>
<script lang="ts">
  import {Component, Vue} from "~/node_modules/nuxt-property-decorator";

  @Component({
    components: {}
  })
  export default class TopPage extends Vue {
    mounted() {
    }
  }
</script>
<style lang="scss">
  .card-body {
    display: flex;

    .card {
      width: 25%;

      img {
        width: 150px;
        height: auto;
      }
    }
  }

  .button-primary {
    background-color: #000000;
    border-radius: 5px;
    color: #ffffff;
    width: 500px;
    height: 80px;
    font-size: 20px;
    margin-top: 2rem;
    margin-bottom: 2rem;
    display: inline-block;
    transition: all 0.6s;


    &:hover {
      transform: scale(1.1);
      background-color: #d8c24b;
      border: #d8c24b;
      span {
        color: white;
      }
    }
  }

  .title {
    text-align: center;
    padding-top: 3rem;
    padding-bottom: 3rem;
    &__img{
      position: relative;
    }
    &__text{
      position: absolute;
      width: 100%;
      top: 35%;
    }
  }

  header {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .header-title {
      display: flex;
      align-items: center;

      img {
        width: 50px;
        height: auto;
      }

      &__text {
        line-height: 20px;

        .first-companyname {
          font-size: 15px;
          color: #98938E; //$color-gray-600
        }

        .companyname {
          font-size: 22px;
        }
      }
    }

    .header-body {
      a {
        padding-left: 0.5rem;
        padding-right: 0.5rem;
      }
    }

    .header-contact {
      width: 120px;
      text-align: center;
      background-color: #000000;
      padding-top: 10px;
      padding-bottom: 10px;

      span {
        text-decoration: none;
        color: white; //$color-white
      }
    }
  }

  main {
    .top-mv {
      height: 30rem;
      background-color: #d8c24b;
      background-image: url("/imgs/top-mv-bg.svg");
      display: flex;
      justify-content: center;
      position: relative;

      &__contents {
        padding-top: 6rem;
        background-color: #ffffff;
        width: 672px;
        height: 420px;
        margin: auto;
        text-align: center;

        h2 {
          font-size: 30px;
        }

        span {
          position: relative;

          &:hover {
            color: #d8c24b;
          }
        }
      }

      &__balloon {
        .balloon {
          position: absolute;
          top: 0;
          left: 0;
          transform: translate(-50%, -50%);

          .balloon-img {

          }

          .balloon-text {
            display: block;
            width: 160px;
          }
        }

        .balloon--1 {
          top: 230px;
          left: 105px;
        }

        .balloon--2 {
          top: -10px;
          right: 100px;

          .balloon-img {
            transform: scale(-1, 1);
          }

        }
      }
    }

    .top-case_study {
      &__body {
        .card-list {
          display: flex;
          justify-content: flex-start;
          flex-wrap: wrap;
          .card{
            padding-top: 1rem;
            padding-bottom: 2rem;
            padding-right: 1rem;
            padding-left: 1rem;
            span{
              text-decoration: none;
              color: #403B36;//$color-gray-700
              &:hover{
                color: #789529;//$color-green
                text-decoration: underline;
              }
            }
          }
        }
      }
      &__button{
        text-align: center;
      }
    }

    .top-info{
      background-color: #EBE8E4;//$color-gray-200
    }
  }
</style>
