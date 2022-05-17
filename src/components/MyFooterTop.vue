<template>
    <div class="footer-top">
        <div class="footer-top__left">

            <div class="footer-top__left__col1">
                <h2> dc comics</h2>
                <ul v-for="(item, index) in dcComics" :key="index">
                    <li> <a href="">  {{ item }} </a> </li>
                </ul>

                <h2>shop</h2>
                <ul v-for="(item, index) in shop" :key="index">
                    <li> <a href="">  {{ item }} </a> </li>
                </ul>
            </div>

            <div class="footer-top__left__col2">
                <h2> DC</h2>
                <ul v-for="(item, index) in dc" :key="index">
                    <li> <a href="">  {{ item }} </a> </li>
                </ul>
            </div>

            <div class="footer-top__left__col3">
                <h2> SITES </h2>
                <ul v-for="(item, index) in sites" :key="index">
                    <li> <a href="">  {{ item }} </a> </li>
                </ul>
            </div>


        </div>


        <div class="footer-top__right">
            <img src="../assets/img/dc-logo-bg.png" alt="">

        </div>



    </div>

</template>





<script>
export default {
    name: "MyFooterTop",
    data: function () {
    return { 
    dcComics: ["Characters", "Comics", "Movies", "TV", "Games", "VIdeos", "News"],    
    shop: ["Shop DC", "Shop DC Collectibles"],
    dc: ["Terms Of Use", "Privacy policy (New)", "Add Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshop", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
    sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power VISA"]
    };
    }
};

</script>





<style scoped lang="scss">
@import "./style/variables.scss";

.footer-top{
    background-image: url("../assets/img/footer-bg.jpg");
    width: 100%;
    overflow: hidden;
    height: 18rem;
    display: flex;
    justify-content: space-around;
    

    &__right{
        display: flex;
        align-items: center;

        img{
            width: 25rem;
        }
    }

    &__left{
        display: flex;
        justify-content: space-between;
        

        &__col1{
            margin-right: 3rem;
            text-align: left;
            font-size: .8rem;
            color: $myFooterTop-text-color;
            
            li{
                margin-top: .3rem ;
            }

            h2{
                margin: 1rem 0;
                text-transform: uppercase;
                font-size: 1rem;
                color: $myFooterTop-title-color ;
            }
        }

        &__col2{
            margin-right: 3rem ;
            text-align: left;
            font-size: .8rem;
            color: $myFooterTop-text-color;
            
            li{
                margin-top: .3rem ;
            }

            h2{
                margin: 1rem 0;
                text-transform: uppercase;
                font-size: 1rem;
                color: $myFooterTop-title-color ;
            }
        }

        &__col3{
              margin-right: 3rem ;
            text-align: left;
            font-size: .8rem;
            color: $myFooterTop-text-color;
            
            li{
                margin-top: .3rem ;
            }

            h2{
                margin: 1rem 0;
                text-transform: uppercase;
                font-size: 1rem;
                color: $myFooterTop-title-color ;
            }
        }
    }
};


</style>