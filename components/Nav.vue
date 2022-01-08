<template>
  <div class="z-10">
      <div class="top-bar w-full border-b border-grey"></div>
        <div class="nav-index">
            <button class="login-link float-right">Login</button>
        </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

.top-bar{
    height: 5px;
    background: transparent linear-gradient(91deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
    opacity: 1;
    padding: 1px;
}
.nav-index{
    top: 5px;
    left: 0px;
    width: 100%;
    height: 67px;
    background: #FFFFFF 0% 0% no-repeat padding-box;
    box-shadow: 0px 3px 6px #00000029;
    border-radius: 0px 0px 12px 12px;
    opacity: 1;
}
button.login-link{
    position: relative;
    top: 31px;
    width: 56px;
    height: 19px;
    text-align: left;
    text-decoration: underline;
    font: normal normal 600 14px/17px Lato;
    letter-spacing: 0.84px;
    color: #38B2AC;
    opacity: 1;
}
</style>