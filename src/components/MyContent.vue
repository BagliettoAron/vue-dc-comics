
<template>
<div class="main-content">
    <h4> Content goes here </h4>

</div>
    
</template>


<script>
export default {
    name: "MyContent",
    
}

</script>

<style scoped lang="scss">
@import "./style/variables.scss";

.main-content {
    background-color: $myContent-section-background;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 3rem;

    h4{
        color: $myContent-text-color;
    }


}



</style>