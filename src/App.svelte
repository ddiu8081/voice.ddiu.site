<script lang="ts">
  import Icon from '@iconify/svelte'

  import HowToUse from './components/HowToUse.svelte'

  const serverName = 'voice.ddiu.site'
</script>

<main class="container max-w-prose mx-auto mt-16 mb-10 px-6 md:px-0">
  <header class="py-2">
    <Icon class="text-6xl" icon="twemoji:radio" />
    <h1 class="text-3xl font-semibold mt-6">Diu Voice Server</h1>
    <p class="opacity-50 mt-2">又一个位于中国的 TeamSpeak 服务器。</p>
  </header>
  <article>
    <div class="my-8">
      <h2 class="uppercase opacity-50 text-sm">服务器地址</h2>
      <div
        class="flex items-center justify-between px-4 py-3 mx-0 md:-mx-4 my-3 bg-slate-100 border border-slate-200 rounded-lg"
      >
        <span class="text-xl font-semibold font-mono text-gray-600">{serverName}</span>
        <Icon
          class="text-3xl opacity-80 mr-2 hidden md:block"
          icon="twemoji:flag-for-flag-china"
        />
      </div>
    </div>
  </article>
  <HowToUse serverName={serverName} />
  <footer class="text-sm opacity-50 py-4">
    2022 ©
    <a href="https://ljl.li/">Diu</a>
  </footer>
</main>
