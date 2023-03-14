<script>
export default{
    data(){
        return[

        ]
    }
}
</script>

<template>
<section>
    <div class="container-sm">
        <h1 class="title">Our News</h1>
        <p class="subtitle">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nemo magni quas rem delectus!</p>
    </div>

    <div class="container">
        <div class="row">
            <div class="card">
                <img src="/images/related-service-2-700x441.jpg" alt="">
                <h2 class="card-title">Why You Need a SEO Agency Now</h2>
                <p class="date">November 1st, 2017</p>
                <article>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perferendis veniam explicabo quod harum praesentium cum necessitatibus. Facilis sapiente nemo ipsum.</article>
            </div>

            <div class="card">
                <img src="/images/related-service-4-700x441.jpg" alt="">
                <h2 class="card-title">SEO Tips For Your Startup</h2>
                <p class="date">November 1st, 2017</p>
                <article>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perferendis veniam explicabo quod harum praesentium cum necessitatibus. Facilis sapiente nemo ipsum.</article>
            </div>

            <div class="card">
                <img src="/images/blog-post-6-700x441.jpg" alt="">
                <h2 class="card-title">Image Optimization For Your Site</h2>
                <p class="date">November 1st, 2017</p>
                <article>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Perferendis veniam explicabo quod harum praesentium cum necessitatibus. Facilis sapiente nemo ipsum.</article>
            </div>
        </div>
        <a class="button" href="#">go to news</a>
    </div>
</section>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables.scss';

section{
    background-color: #F7F8FA;
}
.container{
    text-align: center;
}
.row{
    gap: 20px;
}
.card{
    text-align: center;
    display: flex;
    flex-direction: column;
    color: #606166;

    img{
        margin-bottom: 15px;
    }
    .card-title{
        color: #FFA837;
        margin-bottom: 6px;
    }

    .date{
        font-size: 13px;
        margin-bottom: 15px;
    }

    article{
        line-height: 30px;
        font-size: 17px;
    }
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
    margin-top: 70px;
    margin-bottom: 80px;
    font-size: 15px;
}

</style>