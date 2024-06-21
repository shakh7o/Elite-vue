<script setup>
const images = ["bmw-1", "img-4", "img-3", "img-4", "img-1", "img-6"];
</script>

<template>
  <div class="main">
    <div class="main__info container">
      <h2 class="main__info-title">BMW</h2>
      <div class="main__info-galery">
        <div class="main__galery" v-for="(img, idx) of images" :key="idx">
          <img
            :src="`/src/assets/img/${img}.png`"
            alt=""
            class="main__images-pic"
          />
          <p class="main__info-text">Detail...</p>
        </div>
      </div>
    </div>
    <div class="main__history container">
      <div class="main__history-inf">
        <h3 class="main__history-title">HISTORY</h3>
        <p class="main__history-text">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Arcu pretium
          proin rutrum nam sed nibh condimentum id libero. Etiam non luctus
          scelerisque nec dignissim lobortis. Auctor feugiat scelerisque
          eleifend arcu sed id donec dui eget. Elit elementum nam risus
          dignissim. Arcu fermentum pharetra sed nunc.
        </p>
      </div>
      <img src="@/assets/img/img-7.png" alt="" class="main__history-image" />
    </div>
    <div class="main__content-map container">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d568931.2621017206!2d9.472515906305999!3d51.30108056446076!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sru!2s!4v1718800003127!5m2!1sru!2s"
        width="1190"
        height="600"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.main {
  background: #625451;
  padding: 30px 0;

  &__info {
    &-title {
      text-align: center;
      font-weight: 500;
      font-size: 48px;
      color: #ffffff;
      margin-bottom: 40px;
    }
  }

  &__info-galery {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    row-gap: 30px;
  }

  &__galery {
    width: 370px;
    position: relative;
  }

  &__images-pic {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  &__info-text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 24px;
    color: #fff;
    font-weight: 500;
    cursor: pointer;
    background: #00000040;
    backdrop-filter: blur(15px);
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: 0.3s;

    &:hover {
      opacity: 1;
    }
  }

  &__history {
    display: flex;
    padding: 50px 0;
    gap: 60px;
    justify-content: center;
    align-items: center;
  }

  &__history-title {
    font-size: 48px;
    font-weight: 500;
    text-align: center;
    color: #ffffff;
    margin-bottom: 30px;
  }

  &__history-text {
    font-weight: 400;
    font-size: 24px;
    line-height: 30px;
    text-align: center;
    color: #ffffff;
    max-width: 653px;
  }

  &__history-image {
    width: 450px;
  }
}


</style>
