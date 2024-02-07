<script>
    export default{
        name: "DcHeader"
    }
</script>

<template>
    <header>
        <figure>
            <img src="/img/dc-logo.png">
        </figure>
        <nav>
            

            <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">comics</a></li>
                <li><a href="#">movies</a></li>
                <li><a href="#">tv</a></li>
                <li><a href="#">games</a></li>
                <li><a href="#">collectibles</a></li>
                <li><a href="#">videos</a></li>
                <li><a href="#">fans</a></li>
                <li><a href="#">news</a></li>
                <li><a href="#">shop</a></li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss"scoped>
    header{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding-inline: 50px;
        height: 150px;
        border: 1px solid red;

        nav{
            display: flex;
            align-items: center;

            ul{
                display: flex;
                align-items: center;
                gap: 15px;
                list-style-type: none;

                li{
                    
                    a{
                        color: black;
                        text-decoration: none;
                        text-transform: uppercase;
                        font-weight: 500;
                        position: relative;

                        &:hover{color: #0C7CEC;}
                    }

                }
            }
        }
    }
    
</style>