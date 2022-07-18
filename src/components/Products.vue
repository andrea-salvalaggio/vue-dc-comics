<template>
    <div class="products-bg">
        <div class="jumbo-container">
            <img src="../assets/img/jumbotron.jpg" alt="DC Banner Image">
        </div>
        <div class="title-container">
            <h3>Current Series</h3>
        </div>
        <div class="container d-flex justify-content-center flex-wrap">
            <ProductCard  class="product-card" v-for="(product, index) in products" :key="index" :imgUrl="product.thumb" :title="product.series"/>

            <!-- <div class="product-card" v-for="(product, index) in products" :key="index">
                <div class="img-container">
                    <img :src="product.thumb" :alt="product.series">
                </div>
                <h6 class="mb-0"> {{ product.series }}</h6>
            </div> -->
            <button class="btn-load">Load More</button>
        </div>
    </div>
</template>

<script>
import ProductCard from './ProductCard.vue'

export default {

    name: 'Products',
    components: {
        ProductCard,
    },

    data: function(){
        return{
            products:[
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    .products-bg{
        width: 100%;
        background-color: #1c1c1c;

        .product-card{
            width: calc((100% / 6) - 20px);
            margin: 20px 10px;
        }
    }

    .jumbo-container{
        width: 100%;
        height: 300px;

        img{
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: top;
        }
    }

    .title-container{
        width: 220px;
        position: relative;
        bottom: 30px;

        h3{
            text-align: center;
            text-transform: uppercase;
            color: white;
            background-color: #0282f9;
            padding: 10px 10px;
        }
    }

    .btn-load{
        border: none;
        color: white;
        text-transform: uppercase;
        font-size: 13px;
        letter-spacing: .5px;
        background-color: #0282f9;
        padding: 5px 50px;
        margin-top: 40px;
        margin-bottom: 20px;
    }

</style>