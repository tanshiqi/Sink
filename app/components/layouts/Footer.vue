<script setup>
const { title, github } = useAppConfig()
</script>

<template>
  <section class="md:pt-6">
    <div class="container flex flex-col items-center py-8 mx-auto sm:flex-row">
      <a
        href="https://sink.cool"
        class="text-xl font-black leading-none text-gray-900 select-none dark:text-gray-100 logo"
        :title="title"
      >{{ title }}</a>
      <a
        class="mt-4 text-sm text-gray-500 sm:ml-4 sm:pl-4 sm:border-l sm:border-gray-200 sm:mt-0"
        :href="github"
        target="_blank"
        title="Sink"
      >
        &copy; {{ new Date().getFullYear() }} Based on the open-source project from Sink
      </a>
    </div>
  </section>
</template>
