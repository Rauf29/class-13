
<template>
  <div class="container mx-auto">
 <p class="mt-4 mb-4">
   <router-link to="/"
                class="px-2 py-2 bg-amber-500 rounded-2xl mr-2 ">Home
   </router-link>
   <router-link to="/about" class="px-2 py-2 bg-amber-500 rounded-2xl mr-2 " >About</router-link>

 </p>
    <router-view></router-view>
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

