<script setup>
import Menu from './Menu.vue'

</script>
<template>
    <div class="headerComponent">
        <div class="divLogoImg">
                    <img alt="logo" class="logo" src="../images/logo.svg" />

        </div>
        <Menu />
        <div class="headerComponentBottom">
            <h1>We are creatives</h1>
        <img alt="Vue logo" class="arrowDown" src="../images/icon-arrow-down.svg" />

        </div>
        
    </div>
</template>
<style scoped>
.headerComponent{
    margin: 0;
    background-image: url("../images/desktop/image-header.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    display:flex;
    flex: 1 100%;
    justify-content: space-between;
    flex-flow: row wrap;
}

.divLogoImg{
    display:flex;
    flex: 0 15%;
    align-items: center;
    margin: 2%;
   
}
.logo{
    width: 70%;
    height: auto;
    cursor:pointer;
   
}
.headerComponentBottom{
    display:flex;
    justify-content: center;
    align-items: center;
    flex: 1 100%;
    flex-flow: row wrap;
    padding: 0 0 20% 0;
}
h1{
    flex: 1 100%;
    color:  hsl(0, 0%, 100%);
    font-size: 3.5rem;
    text-transform: uppercase;
    text-align: center;
    margin: 5%;
    font-family: Fraunces;
    letter-spacing: 8px;
     font-weight: 900;
}
.arrowDown{
    margin: 2%;
    flex: 0 2%;
    width: 10%;
    height:auto;
}

</style>