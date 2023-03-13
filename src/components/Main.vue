<script>
    export default{
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

</style>