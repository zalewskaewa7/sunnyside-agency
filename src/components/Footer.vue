<script setup>
const icons=[
    { src: "../images/icon-facebook.svg"},
    { src: "../images/icon-instagram.svg"},
    { src: "../images/icon-twitter.svg"},
    { src: "../images/icon-pinterest.svg"}

]
</script>
<template>
<div class="footerComponent">

    <div class="logoDiv">
   <img class="logoImg" src="../images/logo.svg"/> 
</div>
<ul class="footeMenu">
        <li>About</li>
        <li>Services</li>
        <li>Projects</li>
    </ul>

    <div class="mediaIconsDiv">
        <img v-for="icon in icons" :src="icon.src"/>
    </div>
</div>


</template>
<style lang="scss" scoped>
.footerComponent{
    display:flex;
    justify-content: center;
    flex-flow: row wrap;
    flex: 0 50%;

    .logoDiv{
        padding: 10%;
        flex: 0 60%;
        display:flex;
        justify-content: center;
        .logoImg{
            width: 35%;
            height: auto;
            cursor:pointer;
            filter: invert(68%) sepia(60%) saturate(6890%) hue-rotate(163deg) brightness(97%) contrast(101%);
    }
        }

        .footeMenu{
            padding: 0% 6% 6% 6%;
            display: flex;
            justify-content: space-around;
            flex: 0 60%;
            flex-flow: row wrap;

            li{
                list-style-type:none;
                color:hsl(168, 34%, 41%);
                font-family: "Barlow";

            }
        }

        .mediaIconsDiv{
            padding: 4% 6% 10% 6%;
            display: flex;
            flex: 0 60%;
            flex-flow: row wrap;
            justify-content: center;

                img{
                    padding: 2%;
                    color:hsl(168, 34%, 41%);

                }
        }
        
}
</style>