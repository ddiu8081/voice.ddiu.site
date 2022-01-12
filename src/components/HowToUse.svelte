<script lang="ts">
  import { fade } from 'svelte/transition'
  import { cubicInOut } from 'svelte/easing'
  import Icon from '@iconify/svelte'

  import Download from './Download.svelte'

  let showDownloadPanel = false
</script>

<div class="my-8">
  <h2 class="uppercase opacity-50 text-sm">如何使用</h2>
  <div class="flex flex-col mt-2 text-gray-700">
    <div class="flex py-4 px-4 -mx-4 my-2 rounded-lg md:hover:bg-slate-50">
      <Icon
        class="shrink-0 mr-4 text-2xl md:text-3xl opacity-80"
        icon="twemoji:keycap-1"
      />
      <div class="my-0.5">
        <div>
          下载 TeamSpeak 客户端，请<b>不要</b>使用 ts1.cn 的盗版服务。
        </div>
        <div class="mt-3">
          <a
            target="_blank"
            href="https://www.teamspeak.com/zh-CN/"
            class="inline-flex items-center mr-1 px-4 py-2 border border-gray-300 rounded-md shadow-sm text-sm font-medium text-gray-700 bg-white hover:bg-gray-50 focus:outline-none"
          >
            <Icon class="mr-1" icon="octicon:globe-16" />
            官网
          </a>
          <button
            class="inline-flex items-center mr-1 px-4 py-2 border border-gray-300 rounded-md shadow-sm text-sm font-medium text-gray-700 bg-white hover:bg-gray-50 focus:outline-none"
            on:click={() => { showDownloadPanel = !showDownloadPanel }}
          >
            <Icon class="mr-1" icon="octicon:inbox-16" />
            本站转存地址
          </button>
        </div>
        {#if showDownloadPanel}
          <div transition:fade="{{duration: 300, easing: cubicInOut }}">
            <Download />
          </div>
        {/if}
      </div>
    </div>
    <div class="flex py-3 px-4 -mx-4 my-2 rounded-lg md:hover:bg-slate-50">
      <Icon
        class="shrink-0 mr-4 text-2xl md:text-3xl opacity-80"
        icon="twemoji:keycap-2"
      />
      <div class="my-0.5">
        添加一个新的服务器，服务器地址填写上方内容并建立连接。
      </div>
    </div>
    <div class="flex py-3 px-4 -mx-4 my-2 rounded-lg md:hover:bg-slate-50">
      <Icon
        class="shrink-0 mr-4 text-2xl md:text-3xl opacity-80"
        icon="twemoji:keycap-3"
      />
      <div class="my-0.5">编辑您自己的昵称，昵称将在整个服务器内可见。</div>
    </div>
    <div class="flex py-3 px-4 -mx-4 my-2 rounded-lg md:hover:bg-slate-50">
      <Icon
        class="shrink-0 mr-4 text-2xl md:text-3xl opacity-80"
        icon="twemoji:keycap-4"
      />
      <div class="my-0.5">选择一个房间，开始语音聊天。</div>
    </div>
  </div>
</div>