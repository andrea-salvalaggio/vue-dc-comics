<template>
    <header class="container d-flex justify-content-between align-items-center">
        <div class="py-3">
            <img src="../assets/img/dc-logo.png" alt="DC logo">
        </div>
        <ul class="m-0 p-0">
            <li>Characters</li>
            <li class="active">Comics</li> 
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Collectibles</li>
            <li>Videos</li>
            <li>Fans</li>
            <li>News</li>
            <li>Shop</li>
        </ul>
    </header>
</template>

<script>
export default {

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
        line-height: 50px;

        &.active{
            color: #0282f9;
            border-bottom: 3px solid #0282f9;
        }

        &:hover{
            color: #0282f9;
            border-bottom: 3px solid #0282f9;
        }
    }

</style>