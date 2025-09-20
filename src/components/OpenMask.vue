<template>
  <div class="w-screen h-screen bg-black flex items-center justify-center">
    <div class="w-1/4 aspect-square flex items-center justify-center">
      <div class="heart"></div>
    </div>
  </div>
</template>

<style scoped>
@reference "tailwindcss";

@layer components {
  .heart {
    @apply w-full aspect-square bg-pink-500;
    --_m: radial-gradient(#000 69%, #0000 70%) 84.5%/50%;
    -webkit-mask-box-image: var(--_m);
    mask-border: var(--_m);
    clip-path: polygon(-42% 0, 50% 91%, 142% 0);
  }
}
</style>
