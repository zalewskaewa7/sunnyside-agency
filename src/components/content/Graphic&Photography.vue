<script setup>
    import { ref } from 'vue'
  const graphic = ref(
    { title: "Graphic design",
      text: "  Great design makes you memorable. We deliver artwork that underscores your brand message and captures potential clients’ attention."
    }
);

const photography = ref(
    {
        title: "Photography",
        text: "  Increase your credibility by getting the most stunning, high-quality photos that improve your business image."
    }
)


</script>

<template>
    
    <div class="graphicPhotographyComponent">    
    <div class="graphicPhtography graphic" >
        <h2>{{ graphic.title }}</h2>
        <p>{{ graphic.text }}</p>
    </div>
    <div class="graphicPhtography photography">
        <h2>{{ photography.title }}</h2>
        <p>{{ photography.text }}</p>

    </div>
    </div>
    
    </template>
    <style lang="scss" scoped>

    .graphicPhotographyComponent{
        display: flex;
        justify-content: center;
        flex: 1 100%;
        flex-flow: row wrap;
        
        .graphic{
            background-image: url("../../images/desktop/image-graphic-design.jpg");
        }
        .photography{
            background-image: url("../../images/desktop/image-photography.jpg"),
        }

    .graphicPhtography{
        padding: 2.5%;
        display:flex;
        flex: 0 45%;
        flex-flow: row wrap;
        align-items: flex-end;

        text-transform: capitalize;

        h2{
            flex:1 100%;
             padding: 10%;
        }
        p{
            flex:1 100%;

            padding: 10%; 
        }

    }
    }
    
    </style>