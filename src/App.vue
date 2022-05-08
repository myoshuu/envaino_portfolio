<template>
  <div>
    <section class="mt-12 text-center border">
      <header>
        <div class="title text-lg text-slate-500">Hello 👋, It's Me</div>
        <div class="sub-title text-2xl text-indigo-800 font-medium">
          Edy Pangangkat
        </div>
        <div class="image w-40 mx-auto mt-8">
          <img class="" src="@/assets/me.jpg" alt="" />
        </div>
      </header>
    </section>
  </div>
</template>

<script>
export default {
  name: "App",
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

.image {
  img {
    border-radius: 200rem;
  }
}
</style>
