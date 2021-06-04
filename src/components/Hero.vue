<template>
  <div class="min-h-screen bg-hero-bg">
    <div class="container mx-auto flex items-center min-h-screen">
      <div class="w-1/2">
        <h2 class="font-hero text-9xl text-right text-white">get fit</h2>
        <h3 class="font-hero text-5xl text-right uppercase text-black">
          have fun
        </h3>
        <p class="text-2xl text-right mt-6">
          Join Hamilton's leading zumba club
        </p>
        <AppButton class="float-right mt-5" button-value="Join Now" />
      </div>
      <div class="w-1/2">
        <img class="flex flex-wrap content-end max-w-3xl align-bottom" src="../assets/hero.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import AppButton from "./AppButton";

export default {
  components: {
    AppButton,
  },
};
</script>