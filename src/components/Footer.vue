<template>
    <footer>
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
    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

    footer{
        background-image: url("../assets/img/footer-bg.jpg");
        background-size: cover;
    }

    h4, li{
        color:#ffff; 
    }

    ul{
        list-style: none;
    }

    .wrapper {
        height: 430px;
        overflow: hidden;
    }

    .wrapper img {
        position: relative;     
        top: -50px;
    }

</style>