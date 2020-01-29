<template>
    <section class="gallery">
        <div class="container">
            <div class="container__title"><h1>Примеры наших работ</h1></div>
            <client-only>
                <carousel
                :paginationEnabled="false"
                :navigationEnabled="true"
                :perPageCustom="[[0, 1], [890, 2], [1120, 4]]"
                navigationNextLabel="<div class='slider-btn slider-next'><img src='/icons/arrow-slider.svg'></div>"
                navigationPrevLabel="<div class='slider-btn slider-prev'><img src='/icons/arrow-slider.svg'></div>"
                >
                <slide>
                    <div class="slider-img"><img src="/window.png"></div>
                </slide>
                <slide>
                    <div class="slider-img"><img src="/window.png"></div>
                </slide>
                <slide>
                    <div class="slider-img"><img src="/window.png"></div>
                </slide>
                <slide>
                    <div class="slider-img"><img src="/window.png"></div>
                </slide>
                <slide>
                    <div class="slider-img"><img src="/window.png"></div>
                </slide>
                </carousel>
            </client-only>
        </div>
    </section>
</template>
<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';

.gallery {
  .VueCarousel-navigation-prev[data-v-453ad8cd] {
    left: 60px;

    img {
      transform: rotate(180deg);
    }
  }

  .VueCarousel-navigation-next[data-v-453ad8cd] {
    right: 60px;
  }

  .slider-btn {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: #fff;

    img {
      width: 10px;
      height: 10px;
    }
  }

  .slider-img img {
    height: 264px;
    width: 272px;
  }
}
</style>