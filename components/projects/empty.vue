<template>
  <div>
    <button type="button" @click="isOpen = true"
      class="relative block w-full rounded-lg border-2 border-dashed border-zinc-300 p-2 text-center hover:border-zinc-400 focus:outline-none focus:ring-2 focus:ring-emerald-500 focus:ring-offset-2">
      <Icon class="w-8 h-8 text-emerald-500" name="carbon:lightning" />
      <span class="mt-2 block text-sm font-semibold text-gray-900">Connect your supabase project.</span>
    </button>
    <USlideover v-model="isOpen">
      <div class="p-4 flex-1">
        <Placeholder class="h-full" />
      </div>
    </USlideover>
  </div>
</template>


<script setup>
const isOpen = ref(false)
</script>