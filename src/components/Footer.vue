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
   <img alt="logo" class="logoImg" src="../images/logo.svg"/> 
</div>
<ul class="footeMenu">
        <li>About</li>
        <li>Services</li>
        <li>Projects</li>
    </ul>

    <div class="mediaIconsDiv">
        <img alt="media icon" v-for="icon in icons" :src="icon.src"/>
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
            // filter: invert(68%) sepia(60%) saturate(6890%) hue-rotate(163deg) brightness(97%) contrast(101%);
            filter: invert(50%) sepia(19%) saturate(939%) hue-rotate(118deg) brightness(94%) contrast(84%);
            // filter: invert(25%) sepia(70%) saturate(332%) hue-rotate(116deg) brightness(93%) contrast(89%);
            // filter: invert(24%) sepia(73%) saturate(465%) hue-rotate(153deg) brightness(97%) contrast(94%);
            // filter: invert(45%) sepia(41%) saturate(419%) hue-rotate(118deg) brightness(100%) contrast(91%);
            // filter: invert(37%) sepia(11%) saturate(1560%) hue-rotate(116deg) brightness(93%) contrast(90%);
            // filter: invert(31%) sepia(48%) saturate(362%) hue-rotate(115deg) brightness(92%) contrast(96%);

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
            li:hover{
                cursor: pointer;
                color:  hsl(0, 0%, 100%);
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
                    //  filter: invert(68%) sepia(60%) saturate(6890%) hue-rotate(163deg) brightness(97%) contrast(101%);
                     filter: invert(50%) sepia(19%) saturate(939%) hue-rotate(118deg) brightness(94%) contrast(84%);

                }

                img:hover{
                    cursor: pointer;
                    // filter: invert(100%) sepia(60%) saturate(1469%) hue-rotate(204deg) brightness(111%) contrast(105%);
                    filter: invert(100%) sepia(100%) saturate(0%) hue-rotate(143deg) brightness(106%) contrast(101%);                }
        }
        
}

@media all and (max-width:  375px)  {
    .footerComponent{
        flex: 1 100%;
        .logoDiv{
            padding: 20%;
            flex: 1 100%;
            .logoImg{
            width: 85%;
            height: auto;
        }
    }

    .footeMenu{
        flex: 1 100%;
    }

    .mediaIconsDiv{
        padding: 10% 6% 15% 6%;
        flex: 0 60%;
        justify-content: space-evenly;

    }
    }
}
</style>