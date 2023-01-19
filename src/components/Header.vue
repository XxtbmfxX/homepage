
<template>

  <header class="Header">
    <a href="#">
      <h1>Edie</h1>
    </a>
    <div class="Header_menu">
      <span @click="showMenu = !showMenu" class="material-symbols-outlined">menu</span>
      <transition name="slide-fade">
        <ul v-if="showMenu" class="Header_menu-list">
          <li v-for="item in menuItems" :key="item.name">
            {{ item.name }}
          </li>
        </ul>
      </transition>
    </div>
  </header>

</template>



<script>
export default {
  data() {
    return {
      showMenu: false,
      menuItems: [
        { name: 'Home' },
        { name: 'Services' },
        { name: 'Our Work' },
        { name: 'Clients' },
        { name: 'Contact' },
      ],
    };
  },
};
</script>

<style scoped>
.slide-fade-enter-active {
  transition: all .5s ease;
}

.slide-fade-leave-active {
  transition: all .5s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}

.slide-fade-enter,
.slide-fade-leave-to {
  transform: translateX(-10px);
  opacity: 0;
}


.Header_menu span {
  margin-right: 40px;
  color: #333333;
}

Header h1 {
  margin-block: 40px;
  margin-left: 40px;
}

.Header {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.Header_menu-list {
  position: absolute;
  background-color: #efefef;

  right: 10PX;
  padding: 10px;
  border-radius: 12px;
  border: 1px solid #878787;
}

.Header_nav ul {
  display: flex;
}

.Header ul li {
  margin-bottom: 10px;
}

.Header_menu {
  margin-right: 10px;
  font-size: 1.6rem;

}

.Header_nav ul li {
  list-style: none;
}


@media only screen and (min-width: 1440px) {

  .Header {
    width: 86%;
  }

  .Header_menu span {
    font-size: 4rem;
  }

  .Header_menu-list li {
    margin-block: 20px;
  }

  .Header_menu-list {
    font-size: 2.5rem;
    height: 250px;
    width: 200px;
    padding-left: 30px;
    right: 50px;
  }
}
</style>
