<script setup>

    const emit = defineEmits(['isOpenMobileMenu']);

</script>

<template>
<div @click= "$emit('isOpenMobileMenu', payload)" class="hamburgerIconComponent">
<img alt="hamburger icon" src="../images/icon-hamburger.svg"/>
</div>
</template>
<style lang="scss" scoped>
 .mobileMenuComponent{
        display: none;
    }

    .hamburgerIconComponent{
        display: none;
    }

@media all and (max-width:  375px)  {
   
    .hamburgerIconComponent{
    cursor:pointer;
    margin: 6% 4%;
    display: flex;
    flex: 0 8%;
    align-items: center;

    }    

        }

</style>
