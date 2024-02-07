<script>
    export default{
        name: "DcMain"
    }
</script>

<template>
    <main>
        <div id="main-container" class="bg-black">
            <div class="container">
                <h2> -- Content goes here -- </h2>
            </div>
        </div>
        

        <div class="bg-blue">
            <div id="navigation-main" class="container" >
                <div>
                    <img src="/img/buy-comics-digital-comics.png" alt="">
                    <span>DIGITAL COMICS</span>
                </div>

                <div>
                    <img src="/img/buy-comics-merchandise.png" alt="">
                    <span>MERCHANDISE</span>
                </div>

                <div>
                    <img src="/img/buy-comics-shop-locator.png" alt="">
                    <span>COMIC SHOP LOCATOR</span>
                </div>

                <div>
                    <img src="/img/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </div>

                <div>
                    <img src="/img/buy-dc-power-visa.svg" alt="">
                    <span>COMIC SHOP LOCATOR</span>
                </div>
               
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
    main{
        color: white;
        .bg-black{
            background-color: #121212;
            padding-block: 50px ;
        }

        .bg-blue{
            background-color: #0C7CEC;
            padding-block: 60px;
        }

        img{
            width: 60px;
            margin-right: 10px;
        }

        #navigation-main{
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 40px;
        }

    

    }
</style>