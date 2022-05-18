<template>
  <div class="footer__wrapper">
      <div class="footer__top">

      </div>
      <div class="footer__bottom">
          <div class="container">
            <div class="footer-button">
                <a href="">SIGN-UP NOW!</a>
            </div>
            <div class="footer-social">

            </div>

        </div>
      </div>
    </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.footer {
    &__bottom {
        height: 100px;
        background-color: #303030;
        display: flex;
        justify-content: space-between;
        align-items: center;

        a {
            border: 1px solid #0282f9;
            padding: .3rem .5rem;
            color: white;
        }
    }
}
</style>
