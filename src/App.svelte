<script lang="ts">
  import Icon from '@iconify/svelte'
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
        <span class="text-xl font-semibold font-mono text-gray-600"
          >voice.ddiu.site</span
        >
        <Icon
          class="text-3xl opacity-80 mr-2 hidden md:block"
          icon="twemoji:flag-for-flag-china"
        />
      </div>
    </div>
  </article>
  <div class="my-8">
    <h2 class="uppercase opacity-50 text-sm">如何使用</h2>
    <div class="flex flex-col mt-2 text-gray-700">
      <div
        class="flex py-4 px-4 -mx-4 my-2 rounded-lg gap-4 md:hover:bg-slate-100"
      >
        <Icon class="shrink-0 text-2xl md:text-3xl opacity-80" icon="twemoji:keycap-1" />
        <div class="my-0.5">
          <div>下载 TeamSpeak 客户端。</div>
          <div class="mt-3">
            <a
              target="_blank"
              href="https://www.teamspeak.com/zh-CN/"
              class="inline-flex items-center px-4 py-2 border border-gray-300 rounded-md shadow-sm text-sm font-medium text-gray-700 bg-white hover:bg-gray-50 focus:outline-none"
              >
              <Icon class="mr-1" icon="octicon:globe-16" />
              官网
            </a>
          </div>
        </div>
      </div>
      <div
        class="flex py-3 px-4 -mx-4 my-2 rounded-lg gap-4 md:hover:bg-slate-100"
      >
        <Icon class="shrink-0 text-2xl md:text-3xl opacity-80" icon="twemoji:keycap-2" />
        <div class="my-0.5">
          添加一个新的服务器，服务器地址填写上方内容并建立连接。
        </div>
      </div>
      <div
        class="flex py-3 px-4 -mx-4 my-2 rounded-lg gap-4 md:hover:bg-slate-100"
      >
        <Icon class="shrink-0 text-2xl md:text-3xl opacity-80" icon="twemoji:keycap-3" />
        <div class="my-0.5">
          编辑您自己的昵称，昵称将在整个服务器内可见。
        </div>
      </div>
      <div
        class="flex py-3 px-4 -mx-4 my-2 rounded-lg gap-4 md:hover:bg-slate-100"
      >
        <Icon class="shrink-0 text-2xl md:text-3xl opacity-80" icon="twemoji:keycap-4" />
        <div class="my-0.5">
          选择一个房间，开始语音聊天。
        </div>
      </div>
    </div>
  </div>
  <footer class="text-sm opacity-50 py-4">
    2021 © 
    <a href="https://ljl.li/">Diu</a>
  </footer>
</main>
