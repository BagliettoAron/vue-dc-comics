<template>

    <div class="content__wrap">
        <div class="content__wrap__image">
            <img :src="bookInfo.thumb" :alt="bookInfo.series">
        </div>

        <div class="content__wrap__text">
            <span> {{bookInfo.series}}</span>
        </div>

    </div>

</template>

<script>

export default {
    name: "MyContentData",
    props: {
        bookInfo: Object,
    }, 
}


</script>


<style scoped lang="scss">

@import "./style/variables.scss";
@import "../components/style/common.scss";

.content__wrap {
    width: calc(100% / 6 - 8px);
    margin: 4px;
    height: 10rem;
    position: relative;
    text-align: center;
    

        &__image{
         
            height: 70%;


            img{
                height: 100%;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                padding-bottom: 3rem;
                
            }

        }

        


        &__text {
           height: 30%;
           
            

            span{
                width: 100%;
                text-transform: uppercase;
                color: $myContent-text-color;
                font-size: .5rem;

            }
        }

    }

    
</style>