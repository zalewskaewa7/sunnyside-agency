<script setup>
import Menu from './Menu.vue'
import HamburgerIcon from './HamburgerIcon.vue';
import MobileMenu from './MobileMenu.vue';
import { ref } from 'vue';

const openMenu = ref(false);
 function openMobileMenu(){
    openMenu.value=!openMenu.value;
 }

</script>
<template>
    <div class="headerComponent">
        <div class="divLogoImg">
                    <img alt="logo" class="logo" src="../images/logo.svg" />

        </div>
        <Menu />
        <HamburgerIcon  v-on:is-open-Mobile-Menu="openMobileMenu" title="Hello Ewunia"/>
        <MobileMenu :ifOpenMenu="openMenu"/>
        <div class="headerComponentBottom">
            <h1>We are creatives</h1>
        <img alt="arrow down" class="arrowDown" src="../images/icon-arrow-down.svg" />

        </div>
        
    </div>
</template>
<style lang="scss" scoped>
.headerComponent{
    margin: 0;
    background-image: url("../images/desktop/image-header.jpg");
    background-position: center; 
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
    font-size: 3.2rem;
    text-transform: uppercase;
    text-align: center;
    margin: 5%;
    font-family: "Fraunces";
    letter-spacing: 8px;
     font-weight: 900;
}
.arrowDown{
    margin: 2%;
    flex: 0 2%;
    width: 10%;
    height:auto;
}

@media all and (max-width:  375px)  {

    .headerComponent{
        padding: 6% 0 20% 0;
        background-image: url("../images/mobile/image-header.jpg");
        background-position: center; 
        background-repeat: no-repeat;
        background-size: cover;
.headerComponentBottom{

        h1{
             padding: 12% 0% 0% 0%;
            font-size: 2.5rem;  
        }

        .arrowDown{
            margin: 15% 0 0 0;
            flex: 0 10%;
            width: 15%;
            height:auto;
        }

}
    .divLogoImg{
    display:flex;
    flex: 0 45%;
    align-items: center;
    margin: 4%;
   
    }
}
}


</style>