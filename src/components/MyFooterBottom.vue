<template>
<div class="bottom-footer">

    <div class="bottom-footer__left">
        <button> a sign-up now! </button>
    </div>

    <div class="bottom-footer__right">

    <h2>follow us</h2>

    <ul>
        <li> <img src="../assets/img/footer-facebook.png" alt=""></li>
        <li><img src="../assets/img/footer-twitter.png" alt=""></li>
        <li><img src="../assets/img/footer-youtube.png" alt=""></li>
        <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
        <li><img src="../assets/img/footer-periscope.png" alt=""></li>
    </ul>
    
    </div>
</div>

    
</template>





<script>
export default {
    name: "MyFooterBottom"
}


</script>





<style scoped lang="scss">
@import "./style/variables.scss";

.bottom-footer{
    display: flex;
    justify-content: space-around;
    padding: 3rem 0;
    background-color: $background-footer;

    &__left button{
        text-transform: uppercase;
        color: $myFooterBottom-text-button-color;
        font-size: .9rem;
        background-color: inherit;
        padding: .8rem;
        border: 3px solid $selected-and-bluBanner-background-color;
        font-weight: 600;
    }

    &__right{
        display: flex;
        align-items: center;

        h2{
            color:$selected-and-bluBanner-background-color;
            text-transform: uppercase;
            font-size: 1rem;
            margin-right:1rem ;
        }

        ul {
            display: flex;

            li {
                margin-right: 1rem;
            }
            
        }



    }
}






</style>