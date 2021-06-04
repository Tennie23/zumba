<template>
  <Hero />
  <AppSection class="bg-blue-400" section-class="section"  section-image="dancer.png" button-value ="learn more" section-title="Why Us?" section-text ="Lorem ipsum dolor sit, uptas eos facilis doloribus. Ea enim atque vitae maiores adipisci laudantium qui aperiam labore quos sed tenetur earum aspernatur autem molestiae eveniet, commodi accusantium facere reprehenderit a laborum. Aspernatur rem, nesciunt fugiat nemo suscipit culpa aliquam, deleniti libero, a eius aut earum consectetur ut similique tenetur quia sunt illo laudantium corrupti vero soluta sint! Praesentium, esse ex molestias, porro est excepturi doloremque beatae nam corporis dicta cumque facilis, dignissimos incidunt ipsa laboriosam corrupti vitae dolorum aliquid eius minus? Enim?" />
  <AppSection class="bg-purple-500" section-class="section-reverse"  section-image="couple.jpg" button-value ="learn more" section-title="We Breate Zumba" section-text ="Lorem ipsum dolor sit, uptas eos facilis doloribus. Ea enim atque vitae maiores adipisci laudantium qui aperiam labore quos sed tenetur earum aspernatur autem molestiae eveniet, commodi accusantium facere reprehenderit a laborum. Aspernatur rem, nesciunt fugiat nemo suscipit culpa aliquam, deleniti libero, a eius aut earum consectetur ut similique tenetur quia sunt illo laudantium corrupti vero soluta sint! Praesentium, esse ex molestias, porro est excepturi doloremque beatae nam corporis dicta cumque facilis, dignissimos incidunt ipsa laboriosam corrupti vitae dolorum aliquid eius minus? Enim?" />
  <AppVideoSection />
  <Timetable />
  <CallToAction />
  <AppFooter />
</template>

<script>
import Hero from '@/components/Hero'
import AppSection from '@/components/AppSection'
import AppVideoSection from '@/components/AppVideoSection'
import Timetable from '@/components/Timetable'
import CallToAction from '@/components/CallToAction'
import AppFooter from '@/components/AppFooter'

// import AppSection from '../components/AppSection.vue'

export default {
  name: 'Home',
  components: { Hero, AppSection, AppVideoSection, Timetable, CallToAction, AppFooter }
 
}
</script>
