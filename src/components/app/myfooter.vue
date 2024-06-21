<template>
    <footer class="footer">
    <div class="footer__contacts container">
      <h3 class="footer__contacts-title">ELITE</h3>
      <div class="footer__contacts-social">
        <div class="footer__social">
          <img src="../../assets/img/la_telegram.png" alt="" />
        </div>
        <div class="footer__social">
          <img src="../../assets/img/dashicons_instagram.png" alt="" />
        </div>
        <div class="footer__social">
          <img src="../../assets/img/ant-design_facebook-outlined.png" alt="" />
        </div>
      </div>
      <p class="footer__contacts-num">+998 91 777 79 42</p>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  background: #313030;
  padding: 30px 0 20px 0;

  &__contacts {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  &__contacts-title {
    font-size: 48px;
    font-family: 700;
    line-height: 48px;
    color: #fff;
    padding-bottom: 10px;
  }

  &__contacts-social {
    display: flex;
    gap: 30px;
    cursor: pointer;
  }

  &__contacts-num {
    padding-top: 10px;
    font-family: 700;
    font-size: 20px;
    line-height: 30px;
    color: #fff;
    width: 170px;
  }
}
</style>