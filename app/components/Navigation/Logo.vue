<template>
  <button @click="$emit('logoClicked')" class="flex items-center font-bold gap-3 text-2xl text-secondary marcellus">
    <img src="@/assets/images/unilorin.png" alt="Logo" class=" w-12 object-contain" />
    <div class=" leading-tight text-left">
      <p class="block text-primary  leading-tight text-lg   ">UNILORIN </p>
      <p class="block  text-black   leading-tight text-xs font-normal   ">Nursery and Primary </p>
    </div>
  </button>
</template>

<script setup>
const config = useRuntimeConfig()
const projectName = config.public.projectName
</script>