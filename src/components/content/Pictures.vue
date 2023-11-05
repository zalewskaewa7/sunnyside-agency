<script setup>
const pictures = [
    {src: "./images/desktop/image-gallery-milkbottles.jpg"},
    {src: "./images/desktop/image-gallery-orange.jpg"},
    {src: "./images/desktop/image-gallery-cone.jpg"},
    {src: "./images/desktop/image-gallery-sugarcubes.jpg"}

]
</script>
<template>
    <div class="picturesComponent">
        <img class="image" v-for="picture in pictures" :src="picture.src" alt="some sweets"/>
    </div>
</template>
<style lang="scss" scoped>
.picturesComponent{
    display:flex;
    flex-flow: row wrap;
    flex: 1 100%;

        .image{
            flex: 0 25%;
            width: 25%;
            height: auto;
        }
}
</style>