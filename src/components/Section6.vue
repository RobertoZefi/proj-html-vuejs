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
        <h1 class="title">What Our Clients Say</h1>

        <div class="card-testimonial">
            <img class="testimonial-img" src="/images/testimonials-2.jpg" alt="">
            <p class="description">Ability proceeds from a fusion of skill, knowfedge, understanding and imagination, consolidated by experience.</p>
            <p class="info"><span class="name">Luis Desalvo, </span> <span class="task"> cred tech</span></p>
            <span class="circle active"></span> <span class="circle"></span>
        </div>
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
    
    .testimonial-img{
        border-radius: 999px;
        margin-bottom: 30px;
    }

    .description{
        font-style: italic;
        margin-bottom: 25px;
        line-height: 30px;
        font-size: 17px;
    }

    
    .info{
        margin-bottom: 25px;
        .name{
            font-weight: bold;
            font-size: 17px;
        }
        .task{
            text-transform: uppercase;
            font-size: 17px;
        }
    }

    .circle{
        width: 10px;
        aspect-ratio: 1;
        border: 1px solid black;
        border-radius: 999px;
        display: inline-block;
        margin-right: 5px;
    }

    .active{
        background-color: black;
    }
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