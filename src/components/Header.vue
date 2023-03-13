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
                ]
            }
        }
    }
</script>

<template>
    <header>
        <nav class="container">
            <img src="/images/logo_seo_w_1x.png" alt="">
            <div class="nav-options">
                <ul class="options">
                    <li v-for="el in headerOptions">{{ el }}</li> 
                </ul>
                <a class="button" href="#">get in touch now</a>
            </div>
        </nav>

        <div class="container hero">
            <div class="hero-description">
                <h1>SEM Campaigns Made Simple With Avada</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis amet velit error inventore officia iure.</p>
                <div class="hero-links">
                    <a class="hero-button" href="">buy avada now</a>
                    <a class="hero-button" href="">contact us</a>
                </div>
            </div>
            <img src="/images/best-sem-seo-services-slide-2.png" alt="">
        </div>
    </header>
    
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss';

header{
    background-image: url('/images/pattern_background.png');
    background-color: #361E5C;
    background-size: contain;
    color: white;
    height: 850px;
}

nav{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-bottom: 130px;
    padding-top: 30px;
}

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
    padding: 10px 18px;
    border-radius: 999px;
    font-weight: bold;
    font-size: 13px;
}

.hero{
    display: flex;
    align-items: center;

    img{
        flex-basis: 70%;
    }
}
.hero-description{
    display: flex;
    flex-direction: column;
    gap: 30px;

    h1{
        font-size: 60px;
    }

    p{
        font-size: 20px;
        font-weight: 300;
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
    font-size: 13px;
}

.hero-button:first-child{
    background-color: #FFA837;
}

.hero-button:last-child{
    background-color: #556EED;
}

</style>