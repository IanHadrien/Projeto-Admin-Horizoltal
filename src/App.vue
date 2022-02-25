<template>
<div>
  <Autenticacao_Login1 />
</div>
</template>

<script>
import Autenticacao_Login1 from './components/Autenticacao-Login1.vue'
//import Autenticacao_Registro1 from './components/Autenticacao-Registro1.vue'
//import Autenticacao_Recuperar_Senha from './components/Autenticacao-Recuperar-Senha.vue'

export default {
  name: 'App',
  components: {
    Autenticacao_Login1,
    //Autenticacao_Registro1, <Autenticacao_Registro1 />
    //Autenticacao_Recuperar_Senha <Autenticacao_Recuperar_Senha />
  }
}
</script>

<style>
</style>
