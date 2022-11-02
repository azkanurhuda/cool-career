<template>
  <div class="container mx-auto mb-auto px-2 py-5">
    <CarouselVue />
    <div class="mx-auto mb-6">
      <h1 class="text-2xl my-2 font-semibold">IOS Engineer</h1>
      <p class="font-normal text-black dark:text-black">Imogiri, Bantul, DIY</p>
    </div>
    <div class="flex item-center mx-auto mb-6">
      <div class="flex-1 items-center">
        <p class="font-normal text-gray-500 dark:text-gray-400">Job Posted</p>
        <p class="font-medium text-black dark:text-black">Sep 30, 2022</p>
      </div>
      <div class="flex-1 items-center">
        <p class="font-normal text-gray-500 dark:text-gray-400">Employee Type</p>
        <p class="font-medium text-black dark:text-black">Fulltime</p>
      </div>
      <div class="flex-1 items-center">
        <p class="font-normal text-gray-500 dark:text-gray-400">Experience</p>
        <p class="font-medium text-black dark:text-black">> 5 years</p>
      </div>
    </div>
    <div class="mx-auto mb-6">
      <p class="font-normal text-gray-500 dark:text-gray-400">Lorem Ipsum is simply dummy text of the printing and
        typesetting
        industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer
        took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries,
        but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s
        with the release of Letraset sheets containing Lorem Ipsum passages, and morerecently with desktop publishing
        software like Aldus PageMaker including versions of Lorem Ipsum.</p>
    </div>
    <div class="mx-auto mb-12">
      <h2 class="mb-2 text-md font-semibold text-gray-900 dark:text-white">Requirements:</h2>
      <ul class="space-y-1 max-w-full list-disc list-inside text-gray-500 dark:text-gray-400">
        <li>
          Lorem Ipsum is simply dummy text of the printing and typesetting
        </li>
        <li>
          Lorem Ipsum is simply dummy text of the printing and typesetting Lorem Ipsum is simply dummy text of the
          printing and typesetting
        </li>
        <li>
          Lorem Ipsum is simply dummy text of the printing and typesetting
        </li>
      </ul>
    </div>
    <div class="flex justify-center mb-6">
      <button class="bg-primary-red hover:bg-red-700 text-white font-bold py-2 px-6 rounded">
        Apply Now
      </button>
    </div>
  </div>
</template>

<script>
import CarouselVue from "../components/Carousel.vue";
export default {
  name: "view-job",
  components: {
    CarouselVue
  },
  setup() {


    return {};
  },
};
</script>
