<script setup>
import { GmailIcon, TelegramIcon, BloggerIcon, XIcon, MastodonIcon, GitHubIcon } from 'vue3-simple-icons'

const email = ref(null)
onMounted(() => {
  email.value.href = email.value.href.replace('$', '@')
})
</script>

<template>
  <section class="text-gray-700 bg-white md:pt-6">
    <div class="container flex flex-col items-center py-8 mx-auto sm:flex-row">
      <a
        href="/"
        class="text-xl font-black leading-none text-gray-900 select-none logo"
      >Googa</a>
      <a
        class="mt-4 text-sm text-gray-500 sm:ml-4 sm:pl-4 sm:border-l sm:border-gray-200 sm:mt-0"
        href="/"
        target="_blank"
      >
        &copy; {{ new Date().getFullYear() }} Technical support: HTML.ZONE
      </a>
      
    </div>
  </section>
</template>
