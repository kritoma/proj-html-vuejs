<template>
  <footer>
    <div class="copyrigth">
      <span>© Copyrigth 2012 - 2020 | AVADA THEME BY THEMEFUSION | ALL RIGHTS RESERVED | POWERED BY WORDPRESS</span>
    </div>
    <div class="social">
      <img src="../../assets/img/footer-facebook.png" alt="facebook">
      <img src="../../assets/img/footer-twitter.png" alt="twitter">
      <img src="../../assets/img/footer-pinterest.png" alt="pinterest">
      <img src="../../assets/img/footer-youtube.png" alt="youtube">
    </div>
  </footer>
</template>

<script>
export default {
    name: "BaseFooter",
}
</script>

<style lang="scss" scoped>
footer {
  background-color: #252a33;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.25rem;
  color: #747384;

  .social {
    display: flex;
    gap: .625rem;
  }
}
</style>