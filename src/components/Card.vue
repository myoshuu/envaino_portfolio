<template>
  <!-- Website -->
  <div class="border rounded-lg p-2 hover:border-slate-400 transition-colors">
    <a href="https://envaino.id">
      <div class="card-title flex items-center">
        <fa :icon="icon" :class="style" />
        <p class="ml-3 text-slate-600">{{ title }}</p>
      </div>
      <div class="card-content mt-3">
        <p class="text-sm text-slate-500">Edy Pangangkat</p>

        <div class="sub-content flex justify-between items-center">
          <span class="text-base sm:text-sm">{{ desc }}</span>
          <fa :icon="['fas', 'angle-right']" class="mr-3" />
        </div>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: {
    icon: [],
    title: String,
    desc: String,
  },
};
</script>