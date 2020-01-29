<template>
    <section class="product">
        <div class="container">
            <div class="container__title">
                <h1>Товары</h1>
            </div>
            <div class="cards">
                <div class="card">
                    <div class="card__main">
                        <div class="card__img">
                            <img src="/window.png" alt="">
                        </div>
                        <div class="card__content">
                            <h1 class="card__name">Пластиковые окна</h1>
                            <p class="card__sub">Основной текст</p>
                            <div class="card__spec">
                                <p>Характеристики:</p>
                                <div class="param">
                                    <span class="param__prop">Ширина створки</span>
                                    <span class="param__value">60 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Ширина стеклопакета</span>
                                    <span class="param__value">24/32 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Воздушные камеры</span>
                                    <span class="param__value">3</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Теплосопротивление</span>
                                    <span class="param__value">0,64 м2 С/Вт</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <button class="cost">Рассчитать стоимость</button>
                </div>
                <div class="card">
                    <div class="card__main">
                        <div class="card__img">
                            <img src="/window.png" alt="">
                        </div>
                        <div class="card__content">
                            <h1 class="card__name">Пластиковые окна</h1>
                            <p class="card__sub">Основной текст</p>
                            <div class="card__spec">
                                <p>Характеристики:</p>
                                <div class="param">
                                    <span class="param__prop">Ширина створки</span>
                                    <span class="param__value">60 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Ширина стеклопакета</span>
                                    <span class="param__value">24/32 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Воздушные камеры</span>
                                    <span class="param__value">3</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Теплосопротивление</span>
                                    <span class="param__value">0,64 м2 С/Вт</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <button class="cost">Рассчитать стоимость</button>
                </div>
                <div class="card">
                    <div class="card__main">
                        <div class="card__img">
                            <img src="/window.png" alt="">
                        </div>
                        <div class="card__content">
                            <h1 class="card__name">Пластиковые окна</h1>
                            <p class="card__sub">Основной текст</p>
                            <div class="card__spec">
                                <p>Характеристики:</p>
                                <div class="param">
                                    <span class="param__prop">Ширина створки</span>
                                    <span class="param__value">60 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Ширина стеклопакета</span>
                                    <span class="param__value">24/32 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Воздушные камеры</span>
                                    <span class="param__value">3</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Теплосопротивление</span>
                                    <span class="param__value">0,64 м2 С/Вт</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <button class="cost">Рассчитать стоимость</button>
                </div>
                <div class="card">
                    <div class="card__main">
                        <div class="card__img">
                            <img src="/window.png" alt="">
                        </div>
                        <div class="card__content">
                            <h1 class="card__name">Пластиковые окна</h1>
                            <p class="card__sub">Основной текст</p>
                            <div class="card__spec">
                                <p>Характеристики:</p>
                                <div class="param">
                                    <span class="param__prop">Ширина створки</span>
                                    <span class="param__value">60 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Ширина стеклопакета</span>
                                    <span class="param__value">24/32 мм</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Воздушные камеры</span>
                                    <span class="param__value">3</span>
                                </div>
                                <div class="param">
                                    <span class="param__prop">Теплосопротивление</span>
                                    <span class="param__value">0,64 м2 С/Вт</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <button class="cost">Рассчитать стоимость</button>
                </div>
            </div>
        </div>
    </section>
</template>
<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';

.product {
  .container {
    margin-bottom: 64px;
  }

  .cards {
    @include cards;

    .card {
      max-width: 272px;
      line-height: 24px;

      &__main {
        border-radius: 2px;
        box-shadow: 0 4px 15px 0 rgba(0, 0, 0, 0.05);
        border: solid 1px #e7e7e7;
        background-color: #ffffff;
      }

      &__content {
        padding: 8px 16px;
      }

      &__name {
        font-size: 16px;
        font-weight: 700;
        padding-bottom: 8px;
      }

      &__sub {
        font-size: 14px;
        padding-bottom: 8px;
      }

      &__spec {
        font-size: 12px;

        .param {
          width: 100%;

          &__prop {
            float: left;
            color: #afafaf;
          }

          &__value {
            font-weight: 700;
            float: right;
          }

          &:after {
            content: '  . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . ';
            display: block;
            white-space: nowrap;
            overflow: hidden;
          }
        }
      }
    }
  }

  button {
    @include btn;
    width: 100%;
    margin-top: 16px;
  }
}
</style>