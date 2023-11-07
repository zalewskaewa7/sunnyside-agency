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
        margin: 2%;
        padding: 6% 15%;
        display: flex;
        flex: 0 70%; 
        flex-flow: row wrap;
        justify-self: center;
        justify-content: flex-end;
        
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
                margin: 2%;
                padding: 15% 0;
                font-size: 1.1rem;
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
                }
        }
    }



}
</style>