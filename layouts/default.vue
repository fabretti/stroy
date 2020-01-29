<template>
  <div>
    <header>
        <div class="container">
            <div class="logo">
                <img src="/logo.svg" alt="">
            </div>
            <div class="nav-menu">
                <ul>
                    <li>
                      <a href="#">Окна</a>
                      <div class="subnav">
                        <a href="#">Пластиковые окна</a>
                        <a href="#">Ламинированные окна</a>
                        <a href="#">Остекление балконов</a>
                        <a href="#">Пластиковые двери</a>
                        <a href="#">Подоконники</a>
                        <a href="#">Рольставни</a>
                        <a href="#">Жалюзи  </a>
                      </div>
                    </li>
                    <li>
                      <a href="#">Двери</a>
                      <div class="subnav">
                        <a href="#">Межкомнатные двери</a>
                        <a href="#">Раздвижные двери</a>
                        <a href="#">Комбинированные двери</a>
                        <a href="#">Раздвижные перегородки</a>
                        <a href="#">Алюминивые перегородки</a>
                        <a href="#">Стеклянные двери</a>
                      </div>
                    </li>
                    <li>
                      <a href="#">Корпусная мебель</a>
                      <div class="subnav">
                        <a href="#">Стандартные кухни</a>
                        <a href="#">Кухни на заказ</a>
                        <a href="#">Каркасные кухни</a>
                        <a href="#">Шкафы купе</a>
                        <a href="#">Комоды</a>
                        <a href="#">Книжные полки</a>
                      </div>
                    </li>
                    <li>
                      <a href="#">Другая продукция</a>
                      <div class="subnav">
                        <a href="#">Металичиские лестницы</a>
                        <a href="#">Деревянные лестницы</a>
                        <a href="#">Модульные лестницы</a>
                        <a href="#">Комбинированные лестницы</a>
                        <a href="#">Торговые перегородки</a>
                        <a href="#">Стеновые панели</a>
                        <a href="#">Декоративные заборы</a>
                      </div>
                    </li>
                    <li>
                      <a href="#">Услуги</a>
                      <div class="subnav">
                        <a href="#">Мастер на час</a>
                        <a href="#">Проектирование и дизайн</a>
                        <a href="#">Доставка материалов</a>
                        <a href="#">Складирование и хранение.</a>
                        <a href="#">Выезд замерщика</a>
                        <a href="#">Подбор материалов</a>
                        <a href="#">Уборка помещений</a>
                      </div>
                    </li>
                    <li><a href="#">Контакты</a></li>
                </ul>
            </div>
            <div class="request">
                <button>Оставить заявку</button>
            </div>
            <div class="tel">
                <p>+7 495 968 01 50</p>
                <p>+7 903 968 01 50</p>
            </div>
        </div>
    </header>
    <nuxt/>
    <footer>
        <div class="container">
            <div class="title">В доме строй</div>
            <div class="footer__bot">
                <div class="contacts">
                    <div class="bot__title">
                        <h1>Контакты</h1>
                    </div>
                    <div class="contacts__info">
                        <p>+7 495 968 01 50</p>
                        <p>+7 903 968 01 50</p>
                        <p>vdome-stroy@mail.ru</p>
                    </div>
                </div>
                <div class="nav-menu">
                    <div class="bot__title">
                        <h1>Меню</h1>
                    </div>
                    <div class="nav-menu__list">
                        <ul>
                            <li><a href="#">Окна</a></li>
                            <li><a href="#">Перегородки</a></li>
                            <li><a href="#">Лестницы</a></li>
                            <li><a href="#">Корпусная мебель</a></li>
                        </ul>
                        <ul>
                            <li><a href="#">Новости</a></li>
                            <li><a href="#">Услуги</a></li>
                            <li><a href="#">Галерея</a></li>
                            <li><a href="#">Контакты</a></li>
                        </ul>
                    </div>
                </div>
                <div class="extra">
                    <div class="bot__title">
                        <h1>Дополнительно</h1>
                    </div>
                    <div class="extra__btn">
                        <button>Выезд замерщика</button>
                        <button>Оставить заявку</button>
                    </div>
                </div>
            </div>
            <div class="footer__dev">
                Разработано в
                <a href="https://sevenreasons.ru">sevenreasons.ru</a>
            </div>
        </div>
    </footer>
  </div>
</template>
<style  scoped lang="scss">
@import '~/assets/css/styleComp';
@import '~/assets/css/colors';
header {
  box-shadow: 0 4px 5px 0 rgba(0, 0, 0, 0.05);

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 16px 15px;
  }

  .nav-menu {
    color: $black;

    ul {
      display: flex;

      li {
        position: relative;
        list-style-type: none;
        .subnav {
          position: absolute;
          z-index: 5;
          background-color: #fff;
          top: calc(50% + 10px);
          left: 50%;
          transform: translate(-50%, 0);
          padding: 8px 16px;
          border-radius: 2px;
          border: solid 1px #e7e7e7;
          display: none;
          a {
            font-size: 14px;
            padding: 2px;
            font-weight: 600;
            line-height: 1.71;
            color: #1e1d26;
            display: block;
            padding: 8px 0px;
            border-bottom: 1px solid #e7e7e7;
            text-decoration: none;
            white-space: nowrap;
            &:last-child {
              border-bottom: none;
            }
          }
        }
        &:hover {
          .subnav {
            display: block;
          }
        }
        a {
          color: $black;
          font-size: 14px;
          line-height: 24px;
          font-weight: 600;
          text-transform: uppercase;
          text-decoration: none;
        }

        &:not(:last-of-type) a {
          padding-right: 16px;
        }
      }
    }
  }

  .request {
    button {
      @include btn;
    }
  }

  .tel {
    p {
      font-size: 14px;
      line-height: 24px;
      font-weight: 600;

      &:first-child {
        padding-bottom: 8px;
      }
    }
  }
}

footer {
  background: $black;

  .container {
    padding: 24px 15px;
    flex-direction: column;
    color: #fff;
    font-size: 12px;
    line-height: 24px;
  }

  .title {
    font-size: 18px;
    line-height: 16px;
    font-weight: 700;
    text-transform: uppercase;
    margin-bottom: 16px;
  }

  .footer__bot {
    display: flex;
    justify-content: space-between;

    .bot__title {
      padding-bottom: 8px;

      h1 {
        font-size: 16px;
        line-height: 24px;
        font-weight: 700;
      }
    }

    .contacts__info {
      p {
        font-size: 12px;
      }
    }

    .nav-menu {
      &__list {
        display: flex;

        ul:first-child {
          padding-right: 32px;
        }

        a {
          color: #fff;
          text-decoration: none;
        }
      }
    }

    .extra {
      .extra__btn {
        display: flex;
        flex-direction: column;

        button {
          @include btn;
          font-size: 14px;
          height: 32px;
          font-weight: 600;
          line-height: 32px;
          color: #fff;

          &:first-child {
            margin-bottom: 8px;
          }
        }
      }
    }
  }

  .footer__dev {
    color: #434152;

    a {
      font-size: 14px;
      color: #434152;
      text-decoration: none;
      transition: .2s;

      &:hover {
        color: #636170;
      }
    }
  }
}
</style>