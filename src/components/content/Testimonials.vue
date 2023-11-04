<script setup>
    import { ref } from 'vue'

const testimonials = [
{ imgSrc: "../../images/image-emily.jpg", text: "We put our trust in Sunnyside and they delivered, making sure our needs were met and deadlines were always hit.", author: "Emily R.", job: "Marketing Director" }, 
{ imgSrc: "../../images/image-thomas.jpg", text: "  Sunnyside’s enthusiasm coupled with their keen interest in our brand’s success made it a satisfying and enjoyable experience.", author: "Thomas S.", job: " Chief Operating Officer" },
{ imgSrc: "../../images/image-jennie.jpg", text: "Incredible end result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!", author: "Jennie F.", job: "Business Owner" }
]
  
</script>
<template>
    <div class="testimonialsComponent">
            <h3>Client testimonials</h3>
            <div class="testimonialsDiv">
                <div class="clientTestimonial" v-for="testimonial in testimonials"> 
                 <img  :src="testimonial.imgSrc"  alt="testimonial author"/>
                <p> {{ testimonial.text }}</p>
                <div>{{ testimonial.author }}</div>
                <div class="clientJob">{{ testimonial.job }}</div>
                </div>
            </div>
                
    </div>
</template>
<style lang="scss" scoped>
.testimonialsComponent{
    display:flex;
    flex-flow: row wrap;
    justify-content: center;
    padding: 10% 0 0 0;

    

    h3{
        text-transform: uppercase;
        font-family: "Fraunces";
        font-size: 1.3rem;
        color:  hsl(210, 4%, 67%);
        letter-spacing: 3px;
    }
    .testimonialsDiv{
        display:flex;
    flex-flow: row wrap;
    flex: 1 100%;
    justify-content: center;
    text-align: center;

        .clientTestimonial{
            flex: 0 25%;
            margin: 2%;
            padding: 10% 0;
            font-family: "BarlowThin";
            line-height: 1.5;


                img{
                    border-radius: 50%;
                    width: 25%;
                    height: auto;
                }
                p{
                    padding: 15% 2%;
                    color: hsl(213, 9%, 39%, .8);
                    font-size: 1.1rem;

                }
                div{
                    padding: 2%;
                    color:  hsl(212, 27%, 19%);
                    font-family: "Fraunces";

                }
                .clientJob{
                    color:  hsl(210, 4%, 67%, .8);
                    font-size: 0.9rem;
                    font-family: "BarlowThin";

                }
        }
    }
}
</style>