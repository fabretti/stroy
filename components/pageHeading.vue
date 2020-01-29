<template>
    <section class="main-header">
        <div class="container">
            <h1>Пластиковые окна в Москве</h1>
            <p>Изготавливаем на собственном производстве от 7 дней <span>со скидкой 65%</span></p>
        </div>
    </section>
</template>
<style   lang="scss">
@import '~/assets/css/styleComp'; 
@import '~/assets/css/colors';

.main-header {
  .container {
    margin: 64px auto;
  }

  h1 {
    font-size: 40px;
    line-height: 32px;
    font-weight: 700;
    padding-bottom: 8px;
  }

  p {
    font-size: 16px;
    line-height: 24px;

    span {
      font-weight: 700;
      color: $green;
    }
  }
}
</style>