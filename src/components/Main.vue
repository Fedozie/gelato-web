<template>
    <main class="main">
        <div class="main-description">
            <div class="main-description-lettering">
                <p>
                    The <span>creamiest</span> gelato you will ever lick.
                </p>
                <p>
                    One cone is never enough, never settle. Always go for more.
                </p>
                <button class="btn">Place an order</button>
            </div>
            <div class="main-description-image">
                <svg>
                    <use xlink:href="assets/Main Image.svg"></use>
                </svg>
            </div>
        </div>
        <div class="main-galleria">
            <div class="main-galleria-lettering">
                <div>
                    <p>Our Favourite Gelato</p>
                    <p>One lick, and you love it!</p>
                </div>
                <button class="btn">View Full Menu</button>
            </div>
            <div class="main-galleria-grid">
                <div>
                    <img :src="image1" alt="Ice Cream">
                </div>
                <div>
                    <img :src="image2" alt="Ice Cream">
                </div>
                <div>
                    <img :src="image3" alt="Ice Cream">
                </div>
                <div>
                    <img :src="image4" alt="Ice Cream">
                </div>
                <div>
                    <img :src="image5" alt="Ice Cream">
                </div>
                <div>
                    <img :src="image6" alt="Ice Cream">
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import image1 from "../assets/Rectangle11.jpg"

export default {
    name: 'Main',
    data(){
        return {
            image1: '../assets/Rectangle11.jpg',
            image2: '../assets/Rectangle10.jpg',
            image3: '../assets/Rectangle8.jpg',
            image4: '../assets/Rectangle14.jpg',
            image5: '../assets/Rectangle12.jpg',
            image6: '../assets/Rectangle15.jpg'
        }
    }
}
</script>

<style scoped>
    .main-description{
        display: flex;
        justify-content: space-between;
        padding: 0 5rem;
    }

    .main-description-lettering{
        text-align: left;
        width: 50%;
    }

    .main-description-lettering p{
        margin: 0;
    }

    .main-description-lettering p:first-of-type{
        font-size: 5rem;
    }

    .main-description-lettering p span{
        background: url("/src/assets/Scribble.png") no-repeat;
        
    }

    .main-description-lettering button{
        margin-top: 4rem;
    }

    .main-galleria{
        width: 100%;
        
    }

    .main-galleria-lettering{
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 5rem;
    }

    .main-galleria-lettering p:first-of-type{

    }

    .main-galleria-lettering p:last-of-type{

    }

    .main-galleria-grid{
        display: grid;
        grid-template-columns: repeat(3, 30%);
        grid-template-rows: repeat(3, 30%);
        grid-gap: 3rem;
    }
</style>