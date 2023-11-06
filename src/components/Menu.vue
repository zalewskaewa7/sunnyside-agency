<template>
    <ul class="menu">
        <li>About</li>
        <li>Services</li>
        <li>Projects</li>
        <li class="contactListElement">CONTACT</li>
    </ul>
</template>
<style lang="scss" scoped>
.menu{
    display:flex;
    flex: 0 40%;
    justify-content: space-around;
    align-items: center;
    color:  hsl(0, 0%, 100%);
    margin: 0 2%;

        
        li{
        list-style-type: none;
        margin: 4%;
        font-size: 1.3rem;
        cursor:pointer;

    }
    .contactListElement{
        color: hsl(212, 27%, 19%);
        background-color:  hsl(0, 0%, 100%);
        border-radius: 25px;
        padding: 3% 6%;
        font-family:"BarlowThin";

        
    }

    .contactListElement:hover{
            color:hsl(0, 0%, 100%);
            background-color: rgba(240, 243, 245, 0.37);
        }
}

@media all and (max-width:  375px)  {
        .menu{
            display:none;
            }

        }


</style>