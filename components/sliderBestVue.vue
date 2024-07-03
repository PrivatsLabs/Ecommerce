<template>
  <div class="best">
    <div class="card">
      <div class="img-box">
        <img
          src="https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2021/01/03154029/ikk.webp"
          alt=""
        />
      </div>
      <div class="info-box">
        <p class="h2">{{item.nom}}</p>
        <p class="subtit">{{item.info}}</p>

        <span>{{item.prix}}</span>
      </div>
    </div>
  </div>
</template>



<style scoped>
.best {
}

.card{
    width: 200px;
    border-radius: 15px;
}

img {
  height: auto;
  max-width: 100%;
  border-radius: 15px;

}

.img-box {
    background-color: #F5F4F0;
}

.info-box{
    padding: 10px;

}

.h2 {
  font-family: Montserrat;
  font-size: 18px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  color: var(--black-dark);
}
.subtitle {
  font-size: 15px;
}
.info-box span{
    font-weight: bolder;
}
</style>

