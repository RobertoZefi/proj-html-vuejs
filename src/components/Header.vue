<script>
    export default{
        data(){
            return{
                headerOptions: [
                    'Home',
                    'Who We Are',
                    'What We Do',
                    'Where We Work',
                    'Careers',
                    'News'
                ],

                slideIndex: 0,

                slides:[
                    {
                        title: 'SEM Campaigns Made Simple With Avada',
                        text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis amet velit error inventore officia iure.',
                        image: '/images/best-sem-seo-services-slide-2.png'
                    },{
                        title: 'Rank Your Local Business With SEO',
                        text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis amet velit error inventore officia iure.',
                        image: '/images/best-seo-services-slide-3.png'
                    },{
                        title: 'We Provide The Best SEO Service',
                        text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis amet velit error inventore officia iure.',
                        image: '/images/best-seo-services-slide-1.png'
                    }
                ]
            }
        },

        methods:{
            nextSlide(){
                this.slideIndex++
                if(this.slideIndex === this.slides.length){
                    this.slideIndex = 0
                }
            },

            prevSlide(){
                this.slideIndex--
                if(this.slideIndex < 0){
                    this.slideIndex = this.slides.length - 1
                }
            }
        },

        mounted(){
            setInterval(this.nextSlide, 10000)
        }
    }
</script>

<template>
    <header>
        <nav class="container">
            <div class="nav-options">
                <img class="logo" src="/images/logo_seo_w_1x.png" alt="">
                <ul class="options">
                    <li v-for="el in headerOptions">
                        <a href="#">{{ el }}</a>
                    </li> 
                </ul>
            </div>
            <a class="button" href="#">get in touch now</a>
        </nav>

        <div class="container hero" :class="slideIndex === index ? 'active' : ''" v-for="(el, index) in slides">
            <div class="hero-description">
                <h1>{{ el.title }}</h1>
                <p>{{el.text}}</p>
                <div class="hero-links">
                    <a class="hero-button" href="">buy avada now</a>
                    <a class="hero-button" href="">contact us</a>
                </div>
            </div>
            <img :src="el.image" alt="">
        </div>

        <i @click="prevSlide" class="arrow arrow-left fa-solid fa-chevron-left"></i>
        <i @click="nextSlide" class="arrow arrow-right fa-solid fa-chevron-right"></i>
    </header>
    
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss';

header{
    position: relative;
    color: white;
    height: 880px;
    background-image: url('/images/pattern_background.png'), linear-gradient(to bottom right, #361E5C,#9B3A59, #FC9946);
}

nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-bottom: 130px;
    padding-top: 30px;
    .nav-options{
        display: flex;
        align-items: center;
        gap: 40px;
    }
    .options{
        display: flex;
        gap: 35px;
    }
    
    .button{
        text-transform: uppercase;
        background-color: #FFA837;
        padding: 12px 35px;
        border-radius: 999px;
        font-weight: 700;
        font-size: 14px;
    }
}

/*****************************/
.hero{
    display: flex;
    align-items: center;
    display: none;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    .hero-description{
        display: flex;
        flex-direction: column;
        gap: 30px;
    
        h1{
            font-size: 60px;
        }
    
        p{
            font-size: 21px;
            font-weight: 400;
            width: 500px;
            line-height: 35px;
        }
    
        .hero-links{
            display: flex;
            gap: 20px;
        }
    }
    
    .hero-button{
        text-transform: uppercase;
        padding: 15px 50px;
        border-radius: 999px;
        font-weight: bold;
        font-size: 14px;
    }
    
    .hero-button:first-child{
        background-color: #FFA837;
    }
    
    .hero-button:last-child{
        background-color: #556EED;
    }
}

.hero.active{
    display: flex;
}

.arrow{
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background-color: rgba($color: #000000, $alpha: 0.4);
    padding: 15px;
}

.arrow-left{
    left: 0;
}

.arrow-right{
    right: 0;
}

.hero{
    img{
        animation-name: img-seo;
        animation-duration: 2s;
    }

    @keyframes img-seo {
        0% {opacity: 0;}
        100% {opacity: 1;}
    }
    
    h1{
        animation-name: title-seo;
        animation-duration: 1s;
    }

    @keyframes title-seo {
        0% {
            opacity: 0;
            transform: translateX(-10%);
        }
        100% {
            opacity: 1;
        }
    }

    p{
        animation-name: text-seo;
        animation-duration: 1s;
    }

    @keyframes text-seo {
        0% {
            opacity: 0;
            transform: translateX(-10%);
        }
        100% {
            opacity: 1;
        }
    }

    .hero-button{
        animation-name: button-seo;
        animation-duration: 1s;
    }

    @keyframes button-seo {
        0% {
            opacity: 0;
            transform: translatey(100%);
        }
        100% {
            opacity: 1;
        }
    }
}


</style>