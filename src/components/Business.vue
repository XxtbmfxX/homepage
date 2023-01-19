<script setup>
import { ref } from 'vue';

const image = "https://img.freepik.com/premium-vector/happy-anime-face-manga-style-big-blue-eyes-little-nose-big-kawaii-mouth-yellow-sparkles-her-eyes-hand-drawn-illustration_163875-596.jpg?w=2000";


const businnes = ref([
  {
    id: 0,
    img: "/src/assets/business/smarthome.jpg",
    type: "Full stack application",
    name: "Smart home dashboard",
  },
  {
    id: 1,
    img: "/src/assets/business/onboard.png",
    type: "UX/UI design",
    name: "Onboard application",
  },

  {
    id: 2,
    img: "/src/assets/business/booking.png ",
    type: "Mobile application",
    name: "Booking system",
  },
  {
    id: 3,
    img: "/src/assets/business/juice-product.png ",
    type: "Front End application",
    name: "Juice product homepage",
  },
]);
</script>

<template>
  <article class="Main_business">
    <h1>Good design means good business</h1>

    <div class="Main_business-items">
      <section class="Main_business-item" v-for="item in businnes" :item="item" :key="item.id">
        <img class="Main_Busines-img" :src="item.img" alt="build" />
        <div class="Main_bussiness-text">

          <small>{{ item.type }}</small>
          <h3>{{ item.name }}</h3>
        </div>
      </section>
    </div>
  </article>

  <span class="Main_business-more">
    see more
    <span style="color: #2d9cdb;" class="material-symbols-outlined">
      arrow_right_alt
    </span>
  </span>

</template>

<style>
.Main_business {
  display: grid;
  align-items: center;
  justify-items: center;
  text-align: start;
  width: 90%;
}

.Main_business h1 {
  margin-block: 20px;
}

.Main_bussiness-text {
  justify-self: start;
}


.Main_bussiness-text small {
  margin-block: 5px;
  display: block;
}

.Main_business-item {
  margin-block: 18px;
  /* display: grid;
  justify-items: center; */
}

.Main_business-item h3 {
  font-size: 1.2rem;
}

.Main_Busines-img {
  max-width: 545px;
}


.Main_business-more {
  display: flex;
  justify-content: space-between;
  width: 100px;
  font-size: 1.4rem;
  margin-block: 20px 90px;
  color: #2d9cdb;
}

.Main_business-more:hover {
  cursor: pointer;
  text-decoration: underline;
}

@media only screen and (min-width: 700px) {
  .Main_business-more {
    font-size: 2.4rem;
    width: 150px;
  }

  .Main_bussiness-text small {
    font-size: 1.4rem;
  }

  .Main_bussiness-text h3 {
    font-size: 2.4rem;
  }

}

@media only screen and (min-width: 1440px) {
  .Main_business-items {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    gap: 20px;
    align-items: flex-end;
    height: 1500px;
  }

  .Main_business-item:nth-child(4),
  .Main_business-item:nth-child(2) {
    align-self: flex-start;
  }

  .Main_business-more {
    align-self: flex-end;
    margin-right: 90px;
  }


}
</style>
