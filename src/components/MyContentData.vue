<template>

    <div class="content__wrap">
        <img :src="(bookInfo.thumb)" alt="">
        <div class="content__wrap__text">{{bookInfo.series}}</div>
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



    

.content__wrap {
    width: calc(100% / 6 - 8px);
    margin: 4px;
    height: 10rem;
    //TEST
    border: 2px solid red;

        &__text {
            text-align: center;
            text-transform: uppercase;
            color: $myContent-text-color;
        }

    }

    
</style>