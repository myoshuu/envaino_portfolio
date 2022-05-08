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
      hover:bg-slate-100 hover:text-slate-600
    "
  >
    <fa :icon="['fa', 'bars-staggered']" class="mr-1" />
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
