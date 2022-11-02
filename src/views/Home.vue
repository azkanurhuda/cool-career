<template>
  <div class="container mx-auto mb-auto px-2 py-5">
    <CarouselVue />
    <SearchVue />
    <div class="text-center">
      <span class="text-base">
        Posisi yang tersedia
      </span>
    </div>
    <div class="mt-6">
      <router-link to="/" v-for="job in jobs" :key="job.id"
        class="block p-6 w-full bg-white hover:border-white border-b border-gray-400 hover:shadow-lg mb-1 hover:bg-white dark:bg-white">
        <h5 class="mb-2 text-xl font-bold tracking-tight text-gray-900 dark:text-white">{{ job.job_title }}</h5>
        <div class="flex item-center mx-auto my-4">
          <div class="flex-1 items-center flex">
            <img class="w-6 h-6 mr-4" src="../assets/images/portfolio.png">
            <div>
              <span class="font-normal text-gray-700 dark:text-gray-400">{{ job.employment_type }}</span>
            </div>
          </div>
          <div class="flex-1 items-center flex">
            <img class="w-6 h-6 mr-4" src="../assets/images/volume.png">
            <div>
              <span class="font-normal text-gray-700 dark:text-gray-400">{{ job.experience_range }}</span>
            </div>
          </div>
          <div class="flex-1 items-center flex">
            <img class="w-6 h-6 mr-4" src="../assets/images/location.png">
            <div>
              <span class="font-normal text-gray-700 dark:text-gray-400">{{ job.location }}</span>
            </div>
          </div>
        </div>
      </router-link>
    </div>
  </div>
</template>

<script>
import CarouselVue from '../components/Carousel.vue';
import SearchVue from '../components/Search.vue'
import axios from "axios";
export default {
  name: "Home",
  components: {
    CarouselVue,
    SearchVue
  },
  data() {
    return {
      jobs: []
    }
  },
  methods: {
    setJobs(data) {
      this.jobs = data
    }
  },
  mounted() {
    axios
      .get("http://localhost:3000/external/v1/job")
      .then((response) => this.setJobs(response.data.data))
      .catch((error) => console.log(error))
  }
};
</script>
