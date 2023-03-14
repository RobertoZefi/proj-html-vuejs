<script>
    export default{
        data(){
            return{

            }
        }
    }
</script>

<template>

<section>
    <div class="container-sm">
        <div class="card-consulation">
            <h1>Start Your Free Consulation</h1>
            <p class="description">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dignissimos sed <br> expedita eum quam?</p>
            <a class="button" href="">contact us now</a>
        </div>
    </div>
</section>

<footer>
    <div class="container-sm">
        <img class="logo" src="/images/logo_seo_1x.png" alt="">
        <ul class="links">
            <li>
                <a href="#">Home</a>
            </li>
            <li>
                <a href="#">Who We Are</a>
            </li>
            <li>
                <a href="#">What We Do</a>
            </li>
            <li>
                <a href="#">Where We Work</a>
            </li>
            <li>
                <a href="#">Carrees</a>
            </li>
            <li>
                <a href="#">News</a>
            </li>
            <li>
                <a href="#">Get In Touch Now</a>
            </li>
        </ul>
    </div>
</footer>

</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss';

section{
    background-image: url('/images/CTA-seo-1.jpg');
    background-position: center;
    background-size: cover;
    height: 450px;
    position: relative;

    .card-consulation{
        position: absolute;
        top: 0;
        right: 0;
        left: 0;
        bottom: 0;
        background-color: rgba($color: #000000, $alpha: 0.7);
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        gap: 30px;
        color: white;

        h1{
            font-size: 35px;
        }

        .description{
            font-size: 20px;
            line-height: 30px;
            text-align: center;
        }

        .button{
            text-transform: uppercase;
            background-color: #FFA837;
            padding: 10px 25px;
            border-radius: 999px;
            font-weight: bold;  
            font-size: 13px;
            color: white;
            display: inline-block;
            font-size: 15px;
        }
    }


}

footer{
    text-align: center;

    .logo{
        padding: 50px 0;
    }

    .links{
        display: flex;
        gap: 20px;
    }
}

</style>