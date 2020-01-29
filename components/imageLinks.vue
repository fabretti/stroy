<template>
    <section class="windows">
        <div class="container">
            <div class="container__title">
                <h1>Окна</h1>
            </div>
            <div class="cards">
                <div class="card">
                    <div class="card__img">
                        <img src="/window.png" alt="window">
                    </div>
                    <h1 class="card__name">Пластиковые окна</h1>
                    <span class="price">От 3500 ₽</span>
                </div>
                <div class="card">
                    <div class="card__img">
                        <img src="/window.png" alt="">
                    </div>
                    <h1 class="card__name">Пластиковые окна</h1>
                    <span class="price">От 3500 ₽</span>
                </div>
                <div class="card">
                    <div class="card__img">
                        <img src="/window.png" alt="">
                    </div>
                    <h1 class="card__name">Пластиковые окна</h1>
                    <span class="price">От 3500 ₽</span>
                </div>
                <div class="card">
                    <div class="card__img">
                        <img src="/window.png" alt="">
                    </div>
                    <h1 class="card__name">Пластиковые окна</h1>
                    <span class="price">От 3500 ₽</span>
                </div>
            </div>
        </div>
    </section>
</template>
<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';

.windows {
  .container {
    margin-bottom: 64px;
  }

  .cards {
    @include cards;

    .card {
      text-align: center;

      &__img {
        width: 272px;
        height: 291px;

        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
        }
      }

      &__name {
        font-size: 18px;
        line-height: 24px;
        color: $green;
        padding: 16px 0 8px;
      }

      .price {
        font-size: 16px;
        line-height: 24px;
        font-weight: 700;
      }
    }
  }
}

</style>