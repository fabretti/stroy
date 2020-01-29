<template>
    <section class="news">
      <div class="container">
        <h2 class="container__title">Новости <a class="more" href="">Смотреть все</a></h2>
        <div class="news_items">
          <div class="item">
            <div class="item_img">
              <img src="window.png" alt="">

              <div class="date">07.11.2019</div>
            </div>
            <div class="item_info">
              <div class="title">Новость 1</div>
              <div class="text">Основной текст...</div>
              <a href="#" class="item_more">Подробнее</a>
            </div>
          </div>
          <div class="item">
            <div class="item_img">
              <img src="window.png" alt="">

              <div class="date">07.11.2019</div>
            </div>
            <div class="item_info">
              <div class="title">Новость 1</div>
              <div class="text">Основной текст...</div>
              <a href="#" class="item_more">Подробнее</a>
            </div>
          </div>
          <div class="item">
            <div class="item_img">
              <img src="window.png" alt="">

              <div class="date">07.11.2019</div>
            </div>
            <div class="item_info">
              <div class="title">Новость 1</div>
              <div class="text">Основной текст...</div>
              <a href="#" class="item_more">Подробнее</a>
            </div>
          </div>
          <div class="item">
            <div class="item_img">
              <img src="window.png" alt="">

              <div class="date">07.11.2019</div>
            </div>
            <div class="item_info">
              <div class="title">Новость 1</div>
              <div class="text">Основной текст...</div>
              <a href="#" class="item_more">Подробнее</a>
            </div>
          </div>
        </div>
      </div>
    </section>
</template>
<script>
export default {
  
}
</script>
<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';

.news {
  margin-top: 64px;

  .more {
    font-size: 12px;
    line-height: 2;
  }

  .more,
  .item_more {
    position: relative;
    color: $black;
    font-weight: 600;
    text-decoration: none;

    &:after {
      content: '';
      position: absolute;
      width: 7px;
      height: 8px;
      bottom: 4px;
      right: -15px;
      background: url('/icons/arrow.svg') no-repeat;
    }
  }

  .news_items {
    display: flex;
    justify-content: space-between;
    align-items: stretch;
    z-index: 3;
    margin-bottom: 100px;

    .item {
      width: calc(25% - 12px);
      border-radius: 2px;
      box-shadow: 0 4px 15px 0 rgba(0, 0, 0, 0.05);
      border: solid 1px #e7e7e7;
      margin-bottom: 16px;

      &_img {
        position: relative;
        height: 160px;
        overflow: hidden;
        width: 100%;
        z-index: 1;
        font-size: 0;

        img {
          object-fit: cover;
          height: 100%;
          width: 100%;
        }

        .date {
          position: absolute;
          z-index: 2;
          bottom: 0px;
          left: 15px;
          color: #fff;
          font-size: 12px;
          line-height: 2;
        }

        &:before {
          background-image: linear-gradient(to bottom, transparent, rgba(0, 0, 0, 0.5));
          position: absolute;
          top: 0;
          left: 0;
          height: 100%;
          width: 100%;
          content: '';
          z-index: 0;
        }
      }

      &_info {
        padding: 8px 16px;

        .title {
          font-size: 16px;
          font-weight: bold;
          line-height: 1.5;
          color: $black;
          margin-bottom: 8px;
        }

        .text {
          font-size: 14px;
          line-height: 1.71;
          color: $black;
          margin-bottom: 16px;
        }

        .item_more {
          font-size: 14px;
          font-weight: 600;
          line-height: 1.71;
          color: $black;
          text-decoration: none;
        }
      }
    }
  }
}
</style>