<template>
    <footer>
        <div class="container-img">
            <div class="container">
                <div class="d-flex justify-content-between">
                    <div class="d-flex flex-column">
                        <h4 class="pt-5">Dc Comics</h4>
                        <ul class="p-0">
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>

                        <h4>Shop</h4>
                        <ul class="p-0">
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                    <div class="d-flex flex-column">
                        <h4 class="pt-5">Dc</h4>
                        <ul class="p-0">
                            <li>Term of use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choises</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact us</li>
                        </ul>
                    </div>
                    <div class="d-flex flex-column">
                        <h4 class="pt-5">Sites</h4>
                        <ul class="p-0">
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                    <div class="wrapper">
                        <img src="../assets/img/dc-logo-bg.png" alt="Logo DC Banner">
                    </div>           
                </div>
            </div>
        </div>
        <div class="container py-5">
            <div class="d-flex justify-content-between align-items-center">
                <div>
                    <a href="#" class="btn-footer">Sign-up now!</a>
                </div>
                
                <div class="icon-footer d-flex align-items-center">
                    <h4 class="text-footer">Follow Us</h4>
                    <div v-for="(social, index) in socials" :key="index">
                        <img :src="require(`../assets/img/${social.imgUrl}`)" :alt="social.text">
                    </div>
                </div>
            </div>
        </div>
    </footer>
    
</template>

<script>
export default {

    data: function(){
        return{
            socials:[
                {
                    imgUrl: "footer-facebook.png",
                    text: "Facebook",
                },
                {
                    imgUrl: "footer-twitter.png",
                    text: "Twitter",
                },
                {
                    imgUrl: "footer-youtube.png",
                    text: "Youtube",
                },
                {
                    imgUrl: "footer-pinterest.png",
                    text: "Pinterest",
                },
                {
                    imgUrl: "footer-periscope.png",
                    text: "Periscope",
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

    footer{
        background-color: #303030;
    }

    h4{
        color:#ffff;
        font-size: 18px;
        text-transform: uppercase;
    }

    li{
        color: #959595;
        list-style: none;
        font-weight: 300;
        letter-spacing: 1px;
    }
    .container-img{
        background-image: url("../assets/img/footer-bg.jpg");
        background-size: cover;
    }

    .wrapper {
        height: 430px;
        overflow: hidden;
    }

    .wrapper img {
        position: relative;     
        top: -50px;
    }

    .icon-footer img{
        padding: 0 10px;
    }

    .text-footer{
        color: #0282f9;
        padding-right: 15px;
    }

    .btn-footer{
        border: 2px solid #0282f9;
        padding: 13px;
    }

    a {
        text-decoration: none;
        color: #ffff;
        text-transform: uppercase;

        &:hover{
            color: #ffff;
        }
    }

</style>