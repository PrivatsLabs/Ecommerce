<template>
   <div class="wrapper">

    <img src="https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2023/03/02155535/Banniere-mobile.png" alt="">

    <br> <br>

    <div class="meilleur">

        <h1>Nos meilleures <br> ventes</h1>
        <br>

        <sliderBestVue v-for="item in items" :key="item.id"> </sliderBestVue>


    </div>

</div>

</template>
<style scoped>



h1{
    font-size: 30px !important;
    font-style: normal !important;
    font-weight: 700 !important;
    line-height: normal;
}

.meilleur{
    padding: 15px;
}
</style>