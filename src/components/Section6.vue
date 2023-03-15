<script>
export default{
    data(){
        return{
            currentSlide: 0,

            testimonials:[
                {
                    image: '/images/testimonials-2.jpg',
                    description: 'Ability proceeds from a fusion of skill, knowfedge, understanding and imagination, consolidated by experience.',
                    name: 'Luis Desalvo',
                    task: 'cred tech',
                },

                {
                    image: '/images/testimonials-1.jpg',
                    description: 'Beauty is when you can appreciate yourself. When you love yourself, that’s when you’re most beautiful.',
                    name: 'Shelia McCourtney',
                    task: 'architect',
                },
            ]
        }
    },

    methods:{
        nextSlide(){
            this.currentSlide = 1
        },

        prevSlide(){
            this.currentSlide = 0
        }
    }
}
</script>

<template>

<section>
    <div class="container-sm">
        <h1 class="title">What Our Clients Say</h1>

        <div class="card-testimonial" :class="currentSlide === index ? 'slide-active' : ''" v-for="(el, index) in testimonials">
            <img class="testimonial-img" :src="el.image" alt="">
            <p class="description">{{ el.description }}</p>
            <p class="info"><span class="name">{{el.name}}, </span> <span class="task"> {{ el.task }}</span></p>
        </div>
        <span @click="prevSlide" :class="currentSlide === 0 ? 'active' : ''" class="circle"></span> <span @click="nextSlide" :class="currentSlide === 1 ? 'active' : ''" class="circle"></span>
    </div>

        <div class="card-client">
            <img src="/images/clients_partner_5-200x202.png" alt="">
            <img src="/images/clients_partner_6-200x202.png" alt="">
            <img src="/images/clients_partner_1-200x202.png" alt="">
            <img src="/images/clients_partner_2-200x202.png" alt="">
        </div>
   
</section>

</template>

<style lang="scss" scoped>
@use '../style/partials/variables.scss';

section{
    text-align: center;
}

.title{
    padding-bottom: 50px;
}
.card-testimonial{
    display: none;
    animation-name: card;
    animation-duration: 1s;

    @keyframes card {
        0%{opacity: 0;}
        100%{opacity: 1;}
    }

    .testimonial-img{
        border-radius: 999px;
        margin-bottom: 30px;
        width: 150px;
    }

    .description{
        font-style: italic;
        margin-bottom: 25px;
        line-height: 30px;
        font-size: 18px;
    }

    
    .info{
        margin-bottom: 25px;
        .name{
            font-weight: bold;
            font-size: 19px;
        }
        .task{
            text-transform: uppercase;
            font-size: 19px;
        }
    }

}
.circle{
    width: 13px;
    aspect-ratio: 1;
    border: 1px solid black;
    border-radius: 999px;
    display: inline-block;
    margin-right: 5px;
}

.active{
    background-color: black;
}

.card-testimonial.slide-active{
    display: block;
}

.card-client{
    display: flex;
    justify-content: center;
    gap: 200px;
    padding: 50px 0;
    margin-top: 80px;
    border-top: 1px solid #F7F8FA;

    img{
        width: 120px;
    }
}

</style>