<template>
    <div class="flex flex-col">
        <p class="text-[#15357A] text-center text-[50px] font-bold lg:leading-[68px]">
{{ title }}
        </p>
        <p class="text-[#06122C] text-center text-base font-normal">
            {{ sub }}
        </p>
    </div>

</template> 
<script setup>
defineProps({
  title: {
    type: String,
    default: ''
  },
  sub: {
    type: String,
    default: ''
  },
});
</script>   