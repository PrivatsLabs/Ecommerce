<template>
  <div class="panier">
    <br />
    <br />
    <br />

    <h1 class="text-2xl"><strong>Panier</strong></h1>
    <span style="margin-right: auto !important; font-size: 0.8rem;"> <nuxt-link to="/">Retour</nuxt-link> / panier</span>

<br>
<br>

    <div class="panier-card">
      <div class="img-box">
        <img src="https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2021/01/03154029/ikk.webp" alt="" />
      </div>
      <div class="info-box">
        <p><strong>Farine de patate douce</strong>
        <br /> <span>19,99 £</span> </p> <br>
        <div class="quantity-box">
            <div>-</div>
            <div class="quantity">
                1
            </div>
            <div>+</div>

        </div>
      </div>

      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="size-6"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="m14.74 9-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 0 1-2.244 2.077H8.084a2.25 2.25 0 0 1-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 0 0-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 0 1 3.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 0 0-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 0 0-7.5 0"
        />
      </svg>

    </div>
     <br>
    <hr>

    <div class="bottom shadow-lg">
        <div>
            <p>TOTAL TTC</p>

            <p><strong>19,90 £</strong></p>
        </div>

        <button class="shadow-sm" type="submit">Acceder au paiment</button>

    </div>

  </div>
</template>

<style scoped>
.panier{
    padding: 10px;
    margin-bottom: 300px;
}
.bottom{
    position: fixed;
    bottom: 0;
    left: 0%;
    width: 100%;
    padding: 20px;
    background-color: white;
}
.bottom div{
    display: flex;
    justify-content: space-between;
}
.bottom button{
    width: 100%;
    background-color: gold;
    height: 50px;
    font-weight: bolder;
    margin-top: 10px;
    border-radius: 5px;
}
p{
    font-size: 0.9rem;
}
.panier-card{
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.panier-card img{
    width: 90px;
}
.quantity-box{
    display: flex;
    justify-content: space-between;
    width: 75%;
}
.quantity-box div{
    border: 1px solid rgba(128, 128, 128, 0.584);
    border-radius: 5px;
    padding: 2px;
    width: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.quantity{
    width: 50% !important;
}

.panier-card svg{
    color: grey;
}

</style>