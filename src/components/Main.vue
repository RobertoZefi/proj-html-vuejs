<script>
    import Section4 from './Section4.vue';
    import Section5 from './Section5.vue';
    import Section6 from './Section6.vue';
    export default{
        components:{
            Section4,
            Section5,
            Section6,
        },

        data(){
            return{
                
            }
        }
    }
</script>

<template>
    <main>
        <section class="section-1">
            <div class="container-sm">
                <h1 class="title">Meet The Bew Agency SEO Template From The Avada Team</h1>
                <p class="subtitle">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolor mollitia ipsa eveniet excepturi!</p>
            </div>
            <div class="container">
                <div class="row">
                    <div class="card">
                        <i class="fa-solid fa-road"></i>
                        <h2>Establish Goal</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quaerat pariatur doloribus laborum fuga labore iusto sequi dicta ea id quae?</p>
                    </div>
                    <div class="card">
                        <i class="fa-solid fa-video"></i>
                        <h2>Work With A Team</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quaerat pariatur doloribus laborum fuga labore iusto sequi dicta ea id quae?</p>
                    </div>
                    <div class="card">
                        <i class="fa-solid fa-droplet"></i>
                        <h2>Get Result</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quaerat pariatur doloribus laborum fuga labore iusto sequi dicta ea id quae?</p>
                    </div>
                </div>
                <img src="/images/agency-seo-desk-front-1200x570.jpg" alt="">
            </div>
        </section>

        <section class="section-2">
            <div class="container-sm">
                <h1 class="title">See Our Top Notch Services</h1>
                <p class="subtitle">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Libero provident sint impedit harum.</p>
            </div>
            <div class="container">
                <div class="row">
                    <div class="card">
                        <i class="fa-brands fa-google"></i>
                        <h2>Google SEO</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam asperiores non eius incidunt nam pariatur adipisci placeat explicabo libero perspiciatis? </p>
                        <p class="info">Read more ></p>
                    </div>
                    <div class="card">
                        <i class="fa-solid fa-gear"></i>
                        <h2>Brand Strategy</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam asperiores non eius incidunt nam pariatur adipisci placeat explicabo libero perspiciatis? </p>
                        <p class="info">Read more ></p>
                    </div>
                    <div class="card">
                        <i class="fa-solid fa-building"></i>
                        <h2>Local SEO</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam asperiores non eius incidunt nam pariatur adipisci placeat explicabo libero perspiciatis? </p>
                        <p class="info">Read more ></p>
                    </div>
                    <div class="card">
                        <i class="fa-solid fa-chart-column"></i>
                        <h2>SEO Analysis</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ullam asperiores non eius incidunt nam pariatur adipisci placeat explicabo libero perspiciatis? </p>
                        <p class="info">Read more ></p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section-3">
            <div class="container-sm">
                <h1 class="title">Our Work</h1>
                <p class="subtitle">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptas obcaecati eum explicabo hic.</p>
            </div>
            <div class="container">
                <div class="row">
                    <img src="/images/case-study-gallery-3-1-400x300.jpg" alt="">
                    <img src="/images/case-study-gallery-2-400x300.jpg" alt="">
                    <img src="/images/case-study-gallery-1-1-400x300.jpg" alt="">
                    <img src="/images/case-study-gallery-4-1-400x300.jpg" alt="">
                    <img src="/images/case-study-gallery-5-1-400x300.jpg" alt="">
                    <img src="/images/case-study-gallery-6-1-400x300.jpg" alt="">
                </div>
                <a class="button" href="#">view our work</a>
            </div>
        </section>

        <Section4 />
        <Section5 />
        <Section6 />
    </main>
</template>

<style scoped lang="scss">
@use '../style/partials/variables.scss';

.section-1{
    background-color: #F7F8FA;

    .row{
        gap: 25px;
    }
    .card{
        text-align: center;
        background-color: white;
        padding: 40px 25px;
        display: flex;
        flex-direction: column;
        gap: 25px;

        p{
            line-height: 30px;
        }

        i{
            font-size: 30px;
            color: #FFA837;
        }

    }

    img{
        display: block;
        margin: 0 auto;
    }
}


.section-2{
    background-color: #051642;
    background-image: url('/images/pattern_background.png');
    background-size: cover;
    color: white;
    padding-bottom: 130px;
    .subtitle{
        color: white;
    }
    .row{
        gap: 25px;
    }
    .card{
        text-align: center;
        background-color: #071B50;
        padding: 40px 25px;
        display: flex;
        flex-direction: column;
        gap: 25px;

        p{
            line-height: 30px;
        }

        i{
            font-size: 30px;
            color: #FFA837;
        }

        .info{
            color: #FFA837;
        }
    }

    img{
        display: block;
        margin: 0 auto;
    }
}

.section-3{

    padding-bottom: 80px;
    .container{
        text-align: center;
    }
    .row{
        flex-wrap: wrap;
        gap: 20px;
        justify-content: center;
    }
    .img{
        flex-basis: calc(100% / 3);
        width: 100%;
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
        margin-top: 50px;
        font-size: 15px;
    }
}
</style>