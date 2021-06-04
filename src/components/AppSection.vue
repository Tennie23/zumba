<template>
    <div class="py-32">
        <div :class="sectionClass">
            <div class="w-1/2 flex justify-center p-20">
            <!-- All images must be in assets folder and in parent we only need to provide the image name. -->
                <img :src="require(`../assets/${sectionImage}`)" alt="">
            </div>
             <div class="border-l-2 border-b-2 border-white w-1/2 p-20">
             <!-- pass the section title and text as prop in parent component -->
                <h2 class="text-5xl font-bold text-gray-200 uppercase"> {{ sectionTitle }} </h2>
                <p class="text-2xl my-6 text-gray-200 tracking-wide">{{ sectionText }}</p>
                <!-- pass the button value as prop in parent component -->
            <AppButton :button-value="buttonValue" />
            </div>
        </div>
    </div>
</template>

<script>

import AppButton from './AppButton'

export default {
    components: {
        AppButton
    }, 
    props: ['sectionImage', 'sectionTitle', 'sectionText', 'buttonValue', 'sectionClass'],
   
}
</script>

<style scoped>
.section {
    @apply container mx-auto flex items-center min-h-full;
}
.section-reverse {
        @apply container mx-auto flex flex-row-reverse items-center min-h-full;

}
</style>