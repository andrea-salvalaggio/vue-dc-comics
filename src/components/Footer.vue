<template>
    <footer>
        <div class="container-img">
            <div class="container">
                <div class="d-flex justify-content-between">
                    <div class="d-flex flex-column" v-for="(footerElement, index) in footerLinks" :key="index">
                        <h4 class="pt-5"> {{ footerElement.title }} </h4>
                        <ul class="p-0">
                            <li v-for="(footerLink, footerLinkIndex) in footerElement.content" :key="footerLinkIndex"><a :href="footerLink.url"> {{ footerLink.text }} </a></li>
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

            footerLinks:[
                {
                    title: "dc comics",
                    content: [
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
                            text: "TV",
                            url: "#",
                        },
                        {
                            text: "Games",
                            url: "#",
                        },
                        {
                            text: "Videos",
                            url: "#",
                        },
                        {
                            text: "News",
                            url: "#",
                        }
                    ]
                },
                {
                    title: "shop",
                    content: [
                        {
                            text: "Shop DC",
                            url: "#",
                        },
                        {
                            text: "Shop DC Collectibles",
                            url: "#",
                        }
                    ]
                },
                {
                    title: "dc",
                    content: [
                        {
                            text: "Term of use",
                            url: "#",
                        },
                        {
                            text: "Privacy Policy (new)",
                            url: "#",
                        },
                        {
                            text: "Ad choises",
                            url: "#",
                        },
                        {
                            text: "Advertising",
                            url: "#",
                        },
                        {
                            text: "Jobs",
                            url: "#",
                        },
                        {
                            text: "Subscription",
                            url: "#",
                        },
                        {
                            text: "Talent workshops",
                            url: "#",
                        },
                        {
                            text: "CPSC Certificates",
                            url: "#",
                        },
                        {
                            text: "Rating",
                            url: "#",
                        },
                        {
                            text: "Shop help",
                            url: "#",
                        },
                        {
                            text: "Contact us",
                            url: "#",
                        }
                    ]
                },
                {
                    title: "sites",
                    content: [
                        {
                            text: "DC",
                            url: "#",
                        },
                        {
                            text: "MAD Magazine",
                            url: "#",
                        },
                        {
                            text: "DC Kids",
                            url: "#",
                        },
                        {
                            text: "DC Universe",
                            url: "#",
                        },
                        {
                            text: "DC Power Visa",
                            url: "#",
                        }
                    ]
                },
            ],

            
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
                }
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
        list-style: none;
        font-weight: 300;
        letter-spacing: 1px;

        a{
            color: #959595;
            text-decoration: none;
        }
    }
    .container-img{
        background-image: url("../assets/img/footer-bg.jpg");
        background-size: cover;
        background-repeat: no-repeat;
    }

    .wrapper {
        height: 430px;
        overflow: hidden;

        img {
        position: relative;     
        top: -50px;
        }
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
        text-decoration: none;
        color: #ffff;
        text-transform: uppercase;
    }

</style>