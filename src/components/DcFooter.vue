<script>
    export default{
        name: "DcFooter"
    }
</script>

<template>
    <footer>
        <div id="top-footer">
            <div id="container-top-footer" class="container py-5">
                <div class="d-flex">
                    <div>
                        <ul>
                            <li class="h4 text-white">DC COMICS</li>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>News</li>
                            <li>Videos</li>
                        </ul>

                        <ul>
                            <li class="h4 text-white">SHOP</li>
                            <li>Shop DC</li>
                            <li>Shop DC Collecitbles</li>
                        </ul>
                    </div>

                    <div>
                        
                        <ul>
                            <li class="h4 text-white">DC</li>
                            <li>Terms of use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>

                    <div>
                        <ul>
                            <li class="h4 text-white">SITES</li>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Universe</li>
                            <li>DC Kids</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                    
                </div>
            </div>
        </div>

        <div id="bottom-footer">
            <div class="container d-flex justify-content-between">
                <button>
                    SIGN UP NOW
                </button>
                
                <div>
                    <span>FOLLOW US</span>
                    <i class=""></i>
                    

                </div>
            </div>
        </div>

    </footer>
</template>

<style lang="scss" scoped>
    #top-footer{
        background-image: url("/img/footer-bg.jpg");
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        position: relative;
        color: white;

        #container-top-footer{
            background-image: url("/img/dc-logo-bg.png");
            background-repeat: no-repeat;
            background-position: right;
        }
        
        ul{
            list-style-type: none;
            li{
                color: rgb(155, 155, 155);
            }
        }
    }
    
    #bottom-footer{
            padding-block: 40px ;
            background-color: #313131;
            z-index: 100;
    }



</style>