<template>
  <div class="flex justify-center align-center">
    <!-- <p class="uppercase text-xs p-2 text-slate-400">Pdt. Edy Pangangkat</p> -->
    <section class="mt-5 border rounded-md w-3/4">
      <!-- Header -->
      <header>
        <div class="title text-lg text-slate-500 text-center">
          Hello 👋, It's Me
        </div>
        <p class="sub-title text-2xl text-center text-blue-900 font-medium">
          Edy Pangangkat
        </p>
        <div class="image mx-auto w-40 mt-8">
          <img class="rounded-xl" src="@/assets/me.jpg" alt="" />
        </div>
      </header>

      <!-- Profesi -->
      <div class="profesi mt-4 flex justify-center content-center">
        <div class="w-fit">
          <div class="grid grid-flow-col grid-rows-max grid-cols-max gap-2">
            <SkillCard title="Gembala Jemaat GKMI Sion" />
            <SkillCard title="Dosen STAK AW" />
          </div>
        </div>
      </div>

      <!-- Medsos -->
      <div class="contact">
        <div class="title text-lg text-slate-500 mt-12 mb-6 text-center">
          My Social Media
        </div>
        <div class="content p-2">
          <Card icon="whatsapp" />
        </div>
      </div>
    </section>
  </div>
</template>

<script>
// Components
import SkillCard from "@/components/SkillCard.vue";
import Card from "@/components/Card.vue";

export default {
  name: "App",
  components: {
    SkillCard,
    Card,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Fredoka&family=Poppins:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Fredoka", monospace;
}

p.sub-title {
  font-family: "Poppins";
}
</style>
