<template>
    <section class="about">
        <div class="container">
            <div class="container__title">
                <h1>Почему именно мы?</h1>
            </div>
            <div class="about__cards">
                <div class="card">
                    <div class="card__icon"><img src="/icons/a1.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">1</div>
                </div>
                <div class="card">
                <div class="card__icon"><img src="/icons/a2.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">2</div>
                </div>
                <div class="card">
                    <div class="card__icon"><img src="/icons/a3.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">3</div>
                </div>
                <div class="card">
                    <div class="card__icon"><img src="/icons/a4.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">4</div>
                </div>
                <div class="card">
                    <div class="card__icon"><img src="/icons/a5.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">5</div>
                </div>
                <div class="card">
                    <div class="card__icon"><img src="/icons/a6.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">6</div>
                </div>
                <div class="card">
                    <div class="card__icon"><img src="/icons/a7.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">7</div>
                </div>
                <div class="card">
                    <div class="card__icon"><img src="/icons/a8.svg"></div>
                    <div class="card__title">Бесплатный выезд замерщика</div>
                    <div class="card__text">
                        <ul>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                            <li>Lorem ipsum dolor sit.</li>
                        </ul>
                    </div>
                    <div class="number">8</div>
                </div>
            </div>
        </div>
    </section>
</template>

<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';

.about {
  .container {
    margin-bottom: 64px;
  }

  .about__cards {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(363px, 1fr));
    grid-column-gap: 15px;
    grid-row-gap: 30px;

    .card {
      min-height: 168px;
      position: relative;
      border-radius: 2px;
      box-shadow: 0 4px 15px 0 rgba(0, 0, 0, 0.05);
      border: solid 1px #e7e7e7;
      background-color: #ffffff;
      line-height: 24px;
      padding: 16px 46px 16px 56px;

      &:nth-child(2n) {
        border: solid 1px #4c9a2a;
      }

      &__icon {
        position: absolute;
        left: 15px;
        user-select: none;
      }

      &__title {
        font-size: 16px;
        font-weight: 700;
        padding-bottom: 8px;
      }

      &__text {
        ul {
          li {
            font-size: 12px;
          }
        }
      }

      .number {
        position: absolute;
        right: 10px;
        bottom: 34px;
        font-size: 96px;
        font-weight: 700;
        color: #ebfee2;
        user-select: none;
      }
    }
  }
}
</style>