<template>
  <div>
    <Navbar />
    <h1 class="heading"><span>Experience</span> </h1>
    <footer class="content margin-auto">
      <article style="color: aliceblue" class="text-center">
        <section>
          <span>"{{ motto2 }}"</span>
        </section>
        <section>
          <span>--- {{ author }} ---</span>
        </section>
        <hr />
        <div v-for="e in experiences" :key="e.title">
          <section class="title">
            <span>{{ e.title }}</span>
          </section>

          <article class="skill-menu margin-auto">
            <ul class="ul-navbar">
              <li class="menu-list">
                <a>{{ e.subtitle }}</a>
              </li>
              <li class="menu-list">
                <a>{{ e.subtitle2 }}</a>
              </li>
            </ul>
          </article>
        </div>
      </article>
    </footer>
  </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
import axios from "axios";
//https://63414bb416ffb7e275ce2558.mockapi.io/profile/v1/Pete
export default {
  components: { Navbar },
  methods: {
    async fetchExperience() {
      try {
        let res = await axios.get(
          "https://63414bb416ffb7e275ce2558.mockapi.io/profile/v1/Pete"
        );
        this.experiences = res.data;
      } catch (error) {}
    },
  },

  data() {
    return {
      motto2: "A rose by any other name would smell as sweet.	",
      author: "William Shakespeare",
      experiences: [],
    };
  },
  beforeMount() {
    this.fetchExperience();
  },
};
</script>

<style>
</style>