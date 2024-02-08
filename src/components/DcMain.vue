<script>
    import DcComics from '../components/DcComics.vue';

    export default{
        name: "DcMain",
        
        components: {
            DcComics,

        },

        data() {
            return {
                comics: [
                    {
                        thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                        price: "$19.99",
                        series: "Action Comics",
                        type: "comic book",
                    },
                    {
                        thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                        price: "$3.99",
                        series: "American Vampire 1976",
                        type: "comic book",
                    },
                    {
                        thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                        price: "$16.99",
                        series: "Aquaman",
                        type: "graphic novel",
                    },
                    {
                        thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                        price: "$2.99",
                        series: "Batgirl",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                        price: "$3.99",
                        series: "Batman",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                        price: "$2.99",
                        series: "Batman Beyond",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                        price: "$3.99",
                        series: "Batman/Superman",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                        price: "$4.99",
                        series: "Batman/Superman Annual",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                        price: "$5.99",
                        series: "Batman: The Joker War Zone",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                        price: "$6.99",
                        series: "Batman: Three Jokers",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                        price: "$4.99",
                        series: "Batman: White Knight Presents: Harley Quinn",
                        type: "comic book",
                    },
                    {
                        thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                        price: "$16.99",
                        series: "Catwoman",
                        type: "graphic novel",
                    },
                ]
            };
        }
    }
</script>

<template>
    
    <main>
        
        <div id="jumbotron"></div>
        <div id="main-container" class="bg-black-1">
            
                
            <div id="comicsContainer" class="container d-flex flex-wrap">

                <DcComics
                v-for="(comic, index) in comics"
                :key="index"
                :propsImg="comic.thumb"
                :propsTitle="comic.series"
                />
                <!-- <div id="comic" v-for="(comic, index) in comics" :key="index" class="me-3 mb-5">
                    
                    <img :src="comic.thumb">
                    <p class="text-center ">{{comic.series}}</p>
                                
                </div> -->
            
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

        #jumbotron{
            background-image: url("/img/jumbotron.jpg");
            background-position: top;
            background-repeat: no-repeat;
            background-size: cover;
            padding: 220px;

            position: relative;
        }

        #comic{
            flex-basis: calc(100% / 6 - 20px);
            height: 220px;

            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
                
            }
        }
        
        .bg-black-1{
            background-color: #252525;
            padding-block: 50px ;
        }

        .bg-blue{
            background-color: #0C7CEC;
            padding-block: 60px;
            position: relative;
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
            z-index: 5;
        }

    

    }
</style>