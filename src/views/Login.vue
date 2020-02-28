<template>
  <div id="Login">
    <Header></Header>
    <FormLogin></FormLogin>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from '@/components/templates/Header.vue'
import Footer from '@/components/templates/Footer.vue'
import FormLogin from '@/components/FormLogin.vue'

export default {
  name: 'Login',
  components: {
    Header,
    Footer,
    FormLogin
  }
}
</script>

<style lang="scss">
  #Login {
    height: 100vh;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
  }
</style>
