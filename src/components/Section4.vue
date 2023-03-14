<script>
export default {
    data(){
        return{
          
        }
    }
}
</script>

<template>
<section>
    <div class="container-sm">
        <h1 class="title">Our Plans</h1>
        <p class="subtitle">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Labore temporibus asperiores rerum dolore!</p>
    </div>

    <div class="container">
        <div class="row">
            <div class="card">
                <h2 class="plans-type">Standart</h2>
                <div class="card-options">
                    <p class="price">19<span class="dollar">$</span><span class="cent">99</span><span class="monthly">monthly</span></p>
                    <p>5 Projects</p>
                    <p>5 GB Storage</p>
                    <p>Unlimited Users</p>
                    <a class="button" href="#">start today</a>
                </div>
            </div>

            <div class="card">
                <h2 class="plans-type">Premium</h2>
                <div class="card-options">
                    <p class="price">29<span class="dollar">$</span><span class="cent">99</span><span class="monthly">monthly</span></p>
                    <p>10 Projects</p>
                    <p>15 GB Storage</p>
                    <p>Unlimited Users</p>
                    <a class="button" href="#">start today</a>
                </div>
            </div>

            <div class="card">
                <h2 class="plans-type">Professional</h2>
                <div class="card-options">
                    <p class="price">39<span class="dollar">$</span><span class="cent">99</span><span class="monthly">monthly</span></p>
                    <p>15 Projects</p>
                    <p>30 GB Storage</p>
                    <p>Unlimited Users</p>
                    <a class="button" href="#">start today</a>
                </div>
            </div>

            <div class="card">
                <h2 class="plans-type">Extreme</h2>
                <div class="card-options">
                    <p class="price">59<span class="dollar">$</span><span class="cent">99</span><span class="monthly">monthly</span></p>
                    <p>Unlimited Projects</p>
                    <p>Unlimited Storage</p>
                    <p>Unlimited Users</p>
                    <a class="button" href="#">start today</a>
                </div>
            </div>

        </div>
    </div>

</section>

</template>

<style lang="scss" scoped>
@use '../style/partials/variables.scss';

section{
    background-image: url('/images/background1.jpg');
    background-size: cover;
    padding-bottom: 90px;

    .title{
        color: white;
    }
    .subtitle{
        color: white;
        padding-bottom: 50px;
    }

    .row{
        gap: 20px;
    }
    .card{
        background-color: white;
        text-align: center;
        padding: 25px 60px;
        flex-basis: calc(100% / 4);
    }

    .plans-type{
        font-size: 27px;
        margin-bottom: 35px;
        font-weight: 800;
    }
    .card-options{
        display: flex;
        flex-direction: column;
        gap: 35px;
        color: #606166;
    }
    .price{
        position: relative;
        font-size: 50px;
        font-weight: 700;
        color: #5F7AFB;
    }

    .cent{
        font-size:15px;
        position: absolute;
        left: 54%;
        top: 10px;
        color: #5F7AFB;
    }

    .monthly{
        font-size: 11px;
        color: #606166;
        font-weight: 400;
    }

    .dollar{
        position: absolute;
        font-size: 18px;
        top: 13px;
        right: 73%;
        color: black;
    }

    .button{
        text-transform: uppercase;
        padding: 10px 25px;
        border-radius: 999px;
        font-weight: bold;
        font-size: 13px;
        display: inline-block;
        border: 1px solid #606166;
        color: #606166;

        &:hover{
            color: white;
            background-color: #FFA837;
            border-color: currentColor;
        }
    }
}

</style>