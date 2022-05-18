
<template>

<div class="main-contentList">
    <div class="jumbotron">
        <button class="jumbotron__button">current series</button>
    </div>

    <div class="main-contentList__wrap">
    
        <MyContentData
        v-for="(comic, index) in seriesData"  
        :key="index" 
        :bookInfo="comic"/>
        </div>

        <button class="main-contentList__wrap__button">load more</button>

</div>
    
</template>


<script>
import MyContentData from "./MyContentData.vue";

export default {
    name: "MyContentList",

    components : {
        MyContentData,
    },

     data: function () {
        return {
            seriesData: [
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
        "price": "$19.99",
        "series": "Action Comics",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
        "price": "$3.99",
        "series": "American Vampire 1976",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
        "price": "$16.99",
        "series": "Aquaman",
        "type": "graphic novel"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
        "price": "$2.99",
        "series": "Batgirl",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
        "price": "$3.99",
        "series": "Batman",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
        "price": "$2.99",
        "series": "Batman Beyond",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
        "price": "$3.99",
        "series": "Batman/Superman",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
        "price": "$4.99",
        "series": "Batman/Superman Annual",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
        "price": "$5.99",
        "series": "Batman: The Joker War Zone",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
        "price": "$6.99",
        "series": "Batman: Three Jokers",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
        "price": "$4.99",
        "series": "Batman: White Knight Presents: Harley Quinn",
        "type": "comic book"
    },
    {
        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
        "price": "$16.99",
        "series": "Catwoman",
        "type": "graphic novel"
    }
    ]
        }

    }
}

</script>

<style scoped lang="scss">
@import "./style/variables.scss";
@import "../components/style/common.scss";

.jumbotron{
    height: 20rem;
    width: 100%;
    background-image: url("../assets/img/jumbotron.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;

    &__button {
        position: absolute;
        bottom: 0;
        left: 10rem;
        transform: translate(0, 50%);
        text-transform: uppercase;
        font-size: 1rem;
        font-weight: 550;
        color: $myContent-text-color;
        padding: .5rem 1rem;
        background-color: $selected-and-bluBanner-background-color;
        border: none;
    }
}

.main-contentList {
    background-color: $myContent-section-background;
    position: relative;

    .main-contentList__wrap{
        width: 70%;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        padding: 5rem 0;
        
        &__button {
            position: absolute;
            bottom: 1rem;
            left: 50%;
            transform: translate(-50%, 0);
            text-transform: uppercase;
            font-size: .6rem;
            font-weight: 550;
            color: $myContent-text-color;
            padding: .3rem 2rem;
            background-color: $selected-and-bluBanner-background-color;
            border: none;
        }

    }

}



</style>