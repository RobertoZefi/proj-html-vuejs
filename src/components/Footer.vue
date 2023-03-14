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
    <div class="container">
        <img class="logo" src="/images/logo_seo_1x.png" alt="">
        <ul class="links">
            <li>
                <a class="active" href="#">Home</a>
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


        <ul class="licenses">
            <li>@Copywrite 2017</li>
            <li>|</li>
            <li>Avada Theme by <a href="#" class="license-link">ThemeFusion</a></li>
            <li>|</li>
            <li>All Right Reserved</li>
            <li>|</li>
            <li>Powered by <a href="#" class="license-link">WordPress</a></li>
        </ul> 
        
        <ul class="social">
            <li><i class="fa-brands fa-facebook-f"></i></li>
            <li><i class="fa-brands fa-instagram"></i></li>
            <li><i class="fa-brands fa-twitter"></i></li>
            <li><i class="fa-brands fa-youtube"></i></li>
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
    height: 480px;
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
        width: 200px;
    }

    .links{
        display: flex;
        gap: 40px;
        justify-content: center;
        padding-bottom: 40px;
        font-size: 16px;

        li:hover{
            color: #FFA837;
        }

        .active{
            color: #FFA837;
        }
    }

    .licenses{
        display: flex;
        gap: 15px;
        justify-content: center;
        font-size: 14px;
        color: #5d5c5d;
        margin-bottom: 25px;
        .license-link{
            color: #FFA837;
        }
    }

    .social{
        display: flex;
        gap: 20px;
        justify-content: center;
        color: #5d5c5d;
        font-size: 22px;
        margin-bottom: 60px;
    }
}

</style>