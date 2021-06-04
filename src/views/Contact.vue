<template>
  <div class="bg-green-500 h-screen py-20">
    <div class="container mx-auto md:flex items-center min-h-screen">
      <div class="md:w-1/2 p-20">
        <h3 class="text-gray-100 text-2xl md:text-3xl lg:text-4xl mb-10">Contact Form</h3>
        <form @submit.prevent="handleSubmit">
          <div>
            <label class="text-gray-100 uppercase tracking-wide font-semibold" for="name"> Name</label>
            <input class="w-full rounded-md shadow mb-5 border-gray-100" type="text" v-model="fields.name" required />
          </div>
          <div>
            <label class="text-gray-100 uppercase tracking-wide font-semibold" for="name"> Email</label>
            <input class="w-full rounded-md shadow mb-5 border-gray-100" type="email" name="" id="" v-model="fields.email" required />
          </div>
          <div>
            <label class="text-gray-100 uppercase tracking-wide font-semibold" for="name"> Phone</label>
            <input class="w-full rounded-md shadow mb-5 border-gray-100" type="text" v-model="fields.phone" />
          </div>
          <div>
            <label class="text-gray-100 uppercase tracking-wide font-semibold" for="name"> Your Message</label>
            <textarea class="w-full rounded-md shadow mb-5 border-gray-100" required rows="5" v-model="fields.message"></textarea>
          </div>
          <div>
            <button class="w-full bg-red-500 py-4 rounded-md text-gray-100 uppercase font-bold text-md" type="submit">send now</button>
          </div>
        </form>
      </div>
      <div class=" p-10 w-1/2">
        <h1>Social</h1>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  data() {
    return {
      fields: {},
    };
  },
  methods: {
    handleSubmit() {
      axios
        .post("http://localhost:8080/api/contact", this.fields)
        .then((response) => {
          this.fields = {};
        })
        .catch((error) => {
          console.log("Error");
        });
    },
  },
 
};
</script>