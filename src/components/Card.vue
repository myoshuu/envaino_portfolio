<template>
  <a
    href="https://api.whatsapp.com/send?phone=https://api.whatsapp.com/send?phone=https://wa.me/628979704444"
  >
    <div class="border rounded-lg w-1/4 p-2">
      <div class="card-title flex items-center">
        <fa :icon="['fab', 'whatsapp']" class="text-xl text-green-600" />
        <p class="ml-3 text-green-600">Whatsapp</p>
      </div>
      <div class="card-content mt-3">
        <p class="text-sm text-slate-500">Pdt. Edy Pangangkat</p>

        <div class="sub-content flex justify-between items-center">
          <span>(+62) 897-9704-444</span>
          <fa :icon="['fas', 'angle-right']" class="mr-3" />
        </div>
      </div>
    </div>
  </a>
</template>

<script>
export default {
  name: "Card",
  props: {
    icon: null,
  },
};
</script>