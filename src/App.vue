
<template>
  <div class="container mx-auto">
    <h3
        class="font-bold text-orange-800 inline-block mb-4 mt-4 m-auto justify-center flex">{{
        msg
      }}</h3>
    <div v-for="course in courses " class="shadow p-5 mb-4 border border-gray-200">
      <h2>{{ course
    .name
}}</h2>
      <p>{{ course.description }}</p>
    </div>
    <button
        class="inline-block m-auto py-2 px-5 border rounded shadow bg-amber-500 text-red-50 flex justify-start"
            @click="test">
      Test
    </button>
  </div>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      msg: 'Welcome to your vue.js App',
      courses: [
        {
          id: 1,
          name: 'Vue.js',
          description: 'Vue.js is a progressive framework for building user interfaces ',
          price: 100,
        },
        {
          id: 3,
          name: 'React.js',
          description: 'React.js is a progressive framework for building user interfaces ',
          price: 100,
        },
        {
          id: 3,
          name: 'Angular',
          description: 'Angular is a TypeScript based open source web application framework ',
          price: 100,
        }
      ]
    }
  },
  // mounted() {
  //   this.test()
  // },
  methods: {
    test() {
      this.msg = 'Start learn';
    }
  }
};
</script>

