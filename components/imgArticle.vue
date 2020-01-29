<template>
    <section class="info">
        <div class="container">
            <div class="info__left">
                <img src="/imageArticle.svg" alt="">
            </div>
            <div class="info__right">
                <div class="container__title">
                    <h1>Преимущество окон из ПВХ</h1>
                </div>
                <div class="info__content">
                    <div class="topic">
                        <div class="topic__content">
                            <p>1.	Небольшой вес в сравнении с изделиями из алюминия или дерева.
                            <br>
                            2.	Долгий срок эксплуатации при сохранении технических характеристик.
                            <br>
                            3.	Различные варианты открывания: поворотное, откидное, раздвижное или их комбинации.
                            <br>
                            4.	Простота ухода и налаженный сервис.
                            <br>
                            5.	Доступная цена.
                            <br>
                            Качественный ПВХ - профиль, это безопасный продукт,  не выделяющий вредные вещества. Он отвечает высокому классу экологической безопасности, подтвержденной сертификатом. Важно и то,  что все изделия из ПВХ пластика проходят обязательное декларирование о безвредности объекта при пожаре в центре сертификации, после чего продукция получает Сертификат пожарной безопасности, Помимо всего, пластик остается стабильным при нагреве лучами солнца, со временем он не становится хрупким от ультрафиолета, Характеристики климатического применения остаются стабильными от -30 до +40С.
                        </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';

.info {
  display: flex;
  align-items: center;
  height: 616px;
  margin-bottom: 64px;
  background: url("/background-strang.svg") -150px;

  .container {
    display: flex;
    justify-content: space-between;
    padding: 30px 15px;
  }

  .info__right {
    display: flex;
    flex-direction: column;
    padding: 32px;
    margin-left: 48px;
    border-radius: 2px;
    box-shadow: 0 4px 15px 0 rgba(0, 0, 0, 0.05);
    border: solid 1px #e7e7e7;
    background-color: #ffffff;

    .contacts__info {
      margin-bottom: 16px;
    }

    .info__content {
      display: flex;
      flex-direction: row;

      .topic {
        line-height: 24px;

        &__title {
          font-size: 16px;
          font-weight: 700;
          padding-bottom: 8px;
        }

        &__content {
          font-size: 14px;
          line-height: 1.71;
        }

        &:first-child {
          padding-right: 36px;
        }
      }
    }
  }

}
</style>