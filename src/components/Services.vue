
<script setup >
import { ref } from 'vue';

const services = ref([
  { id: 0, hover: false, color: "#2D9CDB", icon: `edit`, text: "UI/UX Design" },
  { id: 1, hover: false, color: "#27AE60", icon: `code`, text: "Front End" },
  { id: 2, hover: false, color: "#EB5757", icon: `storage`, text: "Back End" },
]);



</script>


<template>
  <article class="Main_service">
    <h1 style="width: 270px;">We offer high demand services</h1>

    <div class="Main_service-items">
      <section class="itemClass" v-for="(item, index) in services" :item="item" :key="item.id"
        @mouseenter="services[index].hover = true" @mouseleave="services[index].hover = false"
        v-bind:class="{ 'hover-bg': item.hover }">

        <div :style="{ backgroundColor: item.color }" class="Icon">
          <span class="material-symbols-outlined"> {{
            item.icon
          }}
          </span>
        </div>
        <div class="Main_service-text">

          <h3>{{ item.text }}</h3>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis a metus ac nulla consequat aliquet id quis
            turpis.
          </p>
          <button>Get Started</button>
        </div>
      </section>
    </div>
  </article>

</template>



<style>
.Main_service {
  margin-bottom: 10px;
  display: grid;
  justify-items: center;
}

.Main_service-items {
  display: grid;
  justify-items: center;
}


.Icon {
  display: grid;
  align-items: center;
  justify-items: center;

  background-color: #2D9CDB;
  border-radius: 16px;
  width: 67px;
  height: 67px;
}

.itemClass {
  display: grid;

  grid-template-rows: 65px 120px;

  gap: 35px;
  width: 70%;
  max-width: 340px;

  height: 420px;
  padding: 30px;
  border-radius: 12px;
  margin-block: 40px;
}

.itemClass p {
  width: 90%;
}

.itemClass h3 {
  font-size: 2.4rem;

}


.hover-bg button {
  background-color: #2D9CDB;
}

.hover-bg {
  box-shadow: 0px 10px 30px rgba(51, 51, 51, 0.1);
}

.actionClass {
  box-shadow: 0px 10px 30px rgba(51, 51, 51, 0.1);
}

.actionClass button {
  background-color: #2D9CDB;
}

.Main_service-text {
  display: grid;
  grid-template-rows: 36px 120px;
  gap: 35px;
}

.Main_service-text p {
  font-size: 1.6rem;
  line-height: 24px;

}

.Main_service-text button {
  width: 116px;
  padding: 12px 10px;
  text-align: center;

}



@media only screen and (min-width: 700px) {

  .Main_service h1 {
    justify-self: start;
    margin-left: 50px;
    font-size: 3.6rem;
    line-height: 54px;
    width: 346px !important;
  }

  .Main_service-items {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    margin: 20px;
  }

  .itemClass h3 {
    font-size: 2.4rem;
  }

  .itemClass p {
    font-size: 1.8rem;
  }

}
</style>