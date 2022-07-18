<template>
    <header class="container d-flex justify-content-between align-items-center">
        <div class="py-3">
            <img src="../assets/img/dc-logo.png" alt="DC logo">
        </div>
        <nav>
            <ul class="m-0 p-0">
                <li v-for="(link, index) in links" :key="index"> <a href="link.url"> {{ link.text }} </a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {

    data: function(){
        return{
            links: [
                {
                    text: "Characters",
                    url: "#",
                },
                {
                    text: "Comics",
                    url: "#",
                },
                {
                    text: "Movies",
                    url: "#",
                },
                {
                    text: "Tv",
                    url: "#",
                },
                {
                    text: "Games",
                    url: "#",
                },
                {
                    text: "Collectibles",
                    url: "#",
                },
                {
                    text: "Videos",
                    url: "#",
                },
                {
                    text: "Fans",
                    url: "#",
                },
                {
                    text: "News",
                    url: "#",
                },
                {
                    text: "Shop",
                    url: "#",
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>

    header{
        background-color: #ffff;
    }

    ul{
        list-style: none;
    }

    li{
        display: inline-block;
        margin: 0 15px;
        text-transform: uppercase;
        font-size: 13px;

        a{
            color: black;
            text-decoration: none;

            &.active{
            color: #0282f9;
            border-bottom: 3px solid #0282f9;
            }

            &:hover{
                color: #0282f9;
                border-bottom: 3px solid #0282f9;
            }
        }
    }

</style>