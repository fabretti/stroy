<template>
    <section class="faq">
      <div class="container">
        <h2 class="container__title">Ответы на ваши вопросы</h2>
        <div class="faq_items">
          <div class="faq_item" @click="accordion1 = !accordion1">
            <div class="faq_item_head" :class="{ active: accordion1 }">
              <div class="head_title">Где я могу посмотреть образцы? <img src="/icons/arrow-slider.svg"></div>
            </div>
            <div class="faq_item_body" :class="{ show: accordion1 }">
              <div class="body_text">Для вас открыты шоу-рум в Москве и в Подмосковье. Также, есть представительство в Серпухове, Подольске и Солнечногорске. Подробнее на странице контакты.</div>
              
            </div>

          </div>
          <div class="faq_item" @click="accordion2 = !accordion2">
            <div class="faq_item_head" :class="{ active: accordion2 }">
              <div class="head_title">Что еще кроме пластиковых окон вы делаете? <img src="/icons/arrow-slider.svg"></div>
            </div>
            <div class="faq_item_body" :class="{ show: accordion2 }">
              <div class="body_text">Алюминиевые перегородки и двери, зимние сады, павильоны. Мебель на заказ. Деревянные и каркасные лестницы. Занимаемся индивидуальным дизайном и проектированием.</div>
              
            </div>

          </div>
          <div class="faq_item" @click="accordion3 = !accordion3">
            <div class="faq_item_head" :class="{ active: accordion3 }">
              <div class="head_title">Хотелось бы отделать балкон, можете помочь? <img src="/icons/arrow-slider.svg"></div>
            </div>
            <div class="faq_item_body" :class="{ show: accordion3 }">
              <div class="body_text">Да, конечно! Остеклим, утеплим, оформим стильными отделочными материалами из нашего каталога. Теплый пол, выключатели и розетки, жалюзи – все под ключ</div>
              
            </div>

          </div>
          <div class="faq_item" @click="accordion4 = !accordion4">
            <div class="faq_item_head" :class="{ active: accordion4 }">
              <div class="head_title">Зачем вызывать замерщика? Я могу дать размеры… <img src="/icons/arrow-slider.svg"></div>
            </div>
            <div class="faq_item_body" :class="{ show: accordion4 }">
              <div class="body_text">Точный замер – это обеспечение, что все четко встанет на место. Мы доверяем нашим клиентам, но рекомендуем обращаться к специалистам для замера и установки. Мы хотим обеспечить вас отличным результатом</div>
              
            </div>

          </div>
        </div>
      </div>
    </section>
</template>
<script>
export default {
  data: () => ({
    accordion1: false,
    accordion2: false,
    accordion3: false,
    accordion4: false,
  }),
}
</script>

<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';
.faq {
  margin-top: 64px;

  &_items {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;

    .faq_item {
      width: calc(50% - 8px);
      border-radius: 2px;
      box-shadow: 0 4px 15px 0 rgba(0, 0, 0, 0.05);
      border: solid 1px #e7e7e7;
      background-color: #ffffff;
      margin-bottom: 16px;

      &_head {
        padding: 4px 16px 4px 8px;
        font-size: 14px;
        font-weight: 600;
        line-height: 2;
        color: $black;
        cursor: pointer;

        .head_title {
          display: flex;
          justify-content: space-between;

          img {
            transform: rotate(90deg);
          }
        }

      }

      &_body {
        max-height: 0px;
        overflow: hidden;
        transition: max-height 0.3s ease-out;

        &.show {
          border-top: solid 1px #e7e7e7;
          max-height: 56px;
        }

        .body_text {
          width: 100%;
          height: 100%;
          padding: 8px 16px;
          font-size: 12px;
          line-height: 1.72;
          color: $black;
        }
      }
    }
  }
}
</style>