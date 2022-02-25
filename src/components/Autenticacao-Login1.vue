<template>
<div class="main-wrapper" style="width: 100vw;
                                height: 100vh;
                                display: flex;
                                justify-content: center ;
                                align-items: center"
                                >

        <div class="auth-wrapper d-flex no-block justify-content-center align-items-center" 
             style="background-image: url(../assets/images/big/auth-bg.jpg) no-repeat center center;">

            <div class="auth-box">
                <div id="loginform"  style="display: block">

                    <div class="logo">
                        <span class="db">
                          <img src="../assets/images/logos/logo-icon.png" alt="logo" />
                        </span>
                        <h5 class="font-medium mb-3">Sign In to Admin</h5>
                    </div>

                    <!-- Form -->
                    <div class="row">
                        <div class="col-12">
                            <form class="form-horizontal mt-3" id="loginform" action="index.html">
                                <div class="input-group mb-3">
                                    <div class="input-group-prepend">
                                        <span class="input-group-text" id="basic-addon1">
                                          <i class="ti-user"></i>
                                        </span>
                                    </div>
                                    <input type="text" 
                                           class="form-control form-control-lg" 
                                           placeholder="Nome do usuário" 
                                           aria-label="Username" 
                                           aria-describedby="basic-addon1">
                                </div>

                                <div class="input-group mb-3">
                                    <div class="input-group-prepend">
                                        <span class="input-group-text" id="basic-addon2">
                                          <i class="ti-pencil"></i>
                                        </span>
                                    </div>
                                    <input type="text" 
                                           class="form-control form-control-lg" 
                                           placeholder="Senha" 
                                           aria-label="Password" 
                                           aria-describedby="basic-addon1">
                                </div>
                                <div class="form-group row">
                                    <div class="col-md-12">
                                        <div class="custom-control custom-checkbox">
                                            <input type="checkbox" class="custom-control-input" id="customCheck1">
                                            <label class="custom-control-label" for="customCheck1">Lembre de mim</label>
                                            <a href="javascript:void(0)" id="to-recover" class="text-dark float-right">
                                                <i class="fa fa-lock mr-1"></i> Esqueceu pwd?
                                            </a>
                                        </div>
                                    </div>
                                </div>
                                <div class="form-group text-center">
                                    <div class="col-xs-12 pb-3">
                                        <button class="btn btn-block btn-lg btn-info" type="submit">
                                          Conecte-se
                                        </button>
                                    </div>
                                </div>
                                <div class="row">
                                    <div class="col-xs-12 col-sm-12 col-md-12 mt-2 text-center">
                                        <div class="social">
                                            <a href="javascript:void(0)" class="btn  btn-facebook" 
                                              data-toggle="tooltip" title="" 
                                              data-original-title="Login with Facebook"> 
                                              <i aria-hidden="true" class="fab  fa-facebook"></i> 
                                            </a>
                                            <a href="javascript:void(0)" class="btn btn-googleplus" data-toggle="tooltip" title="" data-original-title="Login with Google"> <i aria-hidden="true" class="fab  fa-google-plus"></i> </a>
                                        </div>
                                    </div>
                                </div>
                                <div class="form-group mb-0 mt-2">
                                    <div class="col-sm-12 text-center">
                                        Não tem uma conta? 
                                        <a id="inscreva-se" class="text-info ml-1">
                                          <b>Inscrever-se</b>
                                        </a>
                                    </div>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>

                <div id="Registro1" style="display: none">
                    <Autenticacao_Registro1 />
                </div>
      
                <div id="recoverform" style="display: none">
                    <div class="logo">
                        <span class="db"><img src="../assets/images/logos/logo-icon.png" alt="logo" /></span>
                        <h5 class="font-medium mb-3">Recuperar Senha</h5>
                        <span>Digite seu email e as instruções serão enviadas para você!</span>
                    </div>
                    <div class="row mt-3">
                        <!-- Form -->
                        <form class="col-12" action="index.html">
                            <!-- email -->
                            <div class="form-group row">
                                <div class="col-12">
                                    <input class="form-control form-control-lg" type="email" required="" placeholder="Seu email">
                                </div>
                            </div>
                            <!-- pwd -->
                            <div class="row mt-3">
                                <div class="col-12">
                                    <button class="btn btn-block btn-lg btn-danger" type="submit" name="action">Redefinir</button>
                                </div>
                            </div>
                        </form>
                    </div>
                </div>

            </div>

        </div>
        
</div>

</template>

<script>
import Autenticacao_Registro1 from './Autenticacao-Registro1.vue'

export default {
  name: 'Autenticacao_Login1',

  components: {
    Autenticacao_Registro1
  },

  mounted() {
    document.querySelector('#to-recover').addEventListener("click", function() {
        document.querySelector("#loginform").style.display = "none";
        document.querySelector("#recoverform").style.display = "block";
    });

    document.querySelector('#inscreva-se').addEventListener("click", function() {
        document.querySelector("#Registro1").style.display = "block";
        document.querySelector("#loginform").style.display = "none";
    });

  },
}
</script>

<style>
@import url("https://cdn.jsdelivr.net/npm/bootstrap@4.6.1/dist/css/bootstrap.min.css");
</style>
