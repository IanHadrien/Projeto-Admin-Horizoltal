<template>
<body>

  <div class="main-wrapper">

    <div class="preloader">
          <div class="lds-ripple">
              <div class="lds-pos"></div>
              <div class="lds-pos"></div>
          </div>
      </div>

      <div class="auth-wrapper d-flex no-block justify-content-center align-items-center" style="background: url(../assets/images/big/auth-bg.jpg) no-repeat center center;">

          <div class="auth-box">
              <div>

                  <div class="logo">
                      <span class="db">
                          <img alt="thumbnail" 
                              class="rounded-circle" 
                              width="100" 
                              src="../assets/images/users/1.jpg">
                      </span>
                      <h5 class="font-medium mb-3">Genelia</h5>
                  </div>

                          <!-- Form -->
                  <div class="row">
                      <div class="col-12">
                              
                          <form class="form-horizontal mt-3" action="index.html">
                              <div class="form-group row">
                                  <div class="col-12">
                                      <input class="form-control form-control-lg" 
                                              type="password" 
                                              required="" 
                                              placeholder="Password">
                                  </div>
                              </div>

                              <div class="form-group text-center">
                                  <div class="col-xs-12 pb-3">
                                      <button class="btn btn-block btn-lg btn-info" type="submit">LOGIN</button>
                                  </div>
                              </div>
                          </form>

                      </div>
                  </div>

              </div>
          </div>
                  
      </div>

  </div>
  
  <script src="../assets/libs/jquery/dist/jquery.min.js"></script>
      <!-- Bootstrap tether Core JavaScript -->
  <script src="../assets/libs/popper.js/dist/umd/popper.min.js"></script>
  <script src="../assets/libs/bootstrap/dist/js/bootstrap.min.js"></script>
      <!-- ============================================================== -->
      <!-- This page plugin js -->
      <!-- ============================================================== -->
  <script>
    $('[data-toggle="tooltip"]').tooltip();
    $(".preloader").fadeOut();
  </script>

</body>
</template>

<script>
export default {
    name: 'HelloWorld'
}
</script>