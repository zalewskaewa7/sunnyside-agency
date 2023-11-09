<script setup>

</script>

<template>
<div class="mobileMenuComponent">
    <div class="triangle"></div>
    <div class="mobileMenuDiv"> 
        <ul class="menu">
            <li>About</li>
            <li>Services</li>
            <li>Projects</li>
            <li class="contactListElement">CONTACT</li>
        </ul>
    </div>
    
</div>
</template>
<style lang="scss" scoped>

.mobileMenuComponent{
    display:none;
}
@media all and (max-width:  375px)  {
    .mobileMenuComponent{
        margin: 2% 0;
        padding: 2% 0%;
        text-align: center;
        display: none;
        flex-flow: row wrap;
        justify-content: flex-end;
        position: absolute;
        top: 7%;
        left: 3.5%;
        width: 92%;
        
        .triangle{
            
            justify-self: flex-end;
            width: 0; 
            height: 0; 

            border-left: 20px solid transparent;
            border-right: 0px solid transparent;         
            border-bottom: 20px solid hsl(0, 0%, 100%);
        }
        .mobileMenuDiv{
            background-color: hsl(0, 0%, 100%);
            padding: 5% 3% 1% 3%;
            display: flex;
            justify-content: center;
            flex: 1 100%;
        }
        .menu{
            display: flex;
            flex-flow: row wrap;
            flex: 0 30%;
            justify-content: center;
            padding: 0 2% 10% 2%;

            li{
                flex: 0 60%;
                list-style-type: none;
                color:  hsl(232, 10%, 55%);
                margin: 4%;
                padding: 15% 0;
                font-size: 1.2rem;
                font-family: "BarlowThin";
                text-align: center;
                cursor: pointer;

               
            } 
            .contactListElement{
                flex: 0 30%;
                padding: 10% 15% 10% 15%;
                background-color:  hsl(51, 100%, 49%);
                color:  hsl(212, 27%, 19%);
                border-radius: 25px;
                font-size: 1.1rem;

                }
        }
    }



}
</style>