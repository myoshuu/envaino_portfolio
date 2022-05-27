<template>
  <p
    class="
      border
      rounded-2xl
      w-fit
      px-4
      py-2
      transition-colors
      text-sm text-slate-500
      cursor-pointer
      flex
      gap-2
      items-center
      hover:bg-slate-100 hover:text-slate-600
      sm:w-full sm:text-center
    "
  >
    <div class="sm:hidden md:block">
      <fa :icon="['fa', 'bars-staggered']" class="mr-1" />
    </div>
    {{ title }}
  </p>
</template>

<script>
export default {
  props: {
    title: String,
  },
  name: "Card",
};
</script>
