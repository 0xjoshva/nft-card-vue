<template>
  <section>
    <div class="card">
      <div
        class="wrapper"
        @mouseover="monkey = true"
        @mouseleave="monkey = !true"
      >
        <img src="../assets/image-equilibrium.jpg" alt="" class="image" />
        <div class="overlay" v-if="monkey">
          <img src="../assets/icon-view.svg" alt="" />
        </div>
      </div>
      <h3 class="title">Equilibrium #3429</h3>
      <p class="description">
        Our Equilibrium collection promotes balance and calm.
      </p>
      <div class="badges">
        <div class="price">
          <img src="../assets/icon-ethereum.svg" alt="" />
          <p>0.041 ETH</p>
        </div>
        <div class="days">
          <img src="../assets/icon-clock.svg" alt="" />
          <p>3 days left</p>
        </div>
      </div>
      <!-- <hr> -->
      <div class="created">
        <img src="../assets/image-avatar.png" alt="" class="avatar" />
        <p>Creation of <span>Jules Wyvern</span></p>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      monkey: false,
    };
  },
};
</script>
<style scoped>
section {
  width: 100%;
  height: 100vh;
  background: var(--main-bg);
  display: flex;
  justify-content: center;
  align-items: center;
}

.card {
  width: 23rem;
  height: fit-content;
  padding: 1.5rem;
  background: var(--card-bg);
  display: flex;
  flex-direction: column;
  border-radius: 17px;
  box-shadow: 0px 20px 20px 20px #0000002b;
}
.image {
  border-radius: 10px;
  position: relative;
}

.title {
  color: var(--white);
  font-family: "Outfit", sans-serif;
  padding-bottom: 0.5rem;
  padding-top: 1rem;
  font-weight: 600;
}
.description {
  color: var(--softblue);
  font-family: "Outfit", sans-serif;
  padding-bottom: 1rem;
  font-weight: 300;
}
.badges {
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-family: "Outfit", sans-serif;
  padding-bottom: 1.5rem;
  /* line */
  border-bottom: 1px solid var(--line);
  margin-bottom: 1rem;
}
.price {
  display: flex;
  align-items: center;
  column-gap: 0.5rem;
  color: var(--cyan);
  font-weight: 600;
}
.days {
  display: flex;
  align-items: center;
  column-gap: 0.5rem;
  color: var(--softblue);
}
hr {
  height: 1px;
  background: var(--softblue);
}
.created {
  display: flex;
  font-family: "Outfit", sans-serif;
  column-gap: 0.5rem;
}
.created p {
  color: var(--softblue);
}
.created span {
  color: var(--white);
}
.avatar {
  height: 30px;
  border: 1px solid white;
  border-radius: 50%;
  width: auto;
}
.wrapper {
  position: relative;
  width: 320px;
  height: 320px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.image {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1;
}
.overlay {
  position: relative;
  z-index: 10;
  background: hsla(178, 100%, 50%, 0.397);
  width: 320px;
  height: 320px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 7px;
}
.overlay img {
  height: 50px;
  width: auto;
}
</style>
