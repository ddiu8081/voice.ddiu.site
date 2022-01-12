<script lang="ts">
  const downList = [
    {
      platform: 'Windows',
      version: '5.0.0-beta66',
      link: 'https://cloud-upyun.ddiu.site/files/teamspeak/teamspeak-client.msi',
    }, {
      platform: 'Windows',
      version: '3.5.6',
      link: 'https://cloud-upyun.ddiu.site/files/teamspeak/TeamSpeak3-Client-win64-3.5.6.exe',
    }, {
      platform: 'MacOS',
      version: '5.0.0-beta66',
      link: 'https://cloud-upyun.ddiu.site/files/teamspeak/teamspeak-client.dmg',
    }, {
      platform: 'MacOS',
      version: '3.5.7-beta1',
      link: 'https://cloud-upyun.ddiu.site/files/teamspeak/TeamSpeak3-Client-macosx-3.5.7.dmg',
    }
  ]
</script>

<div class="mt-3 px-4 py-2 mx-0 my-3 bg-slate-100 rounded-lg text-sm">
  <div class="font-bold py-1 mb-1">本站转存地址</div>
  {#each downList as item (item.link)}
    <div class="flex py-1">
      <span>{item.platform}</span>
      <span class="ml-2 opacity-50">{item.version}</span>
      <span class="flex-1"></span>
      <a href={item.link} target="_blank" class="text-slate-400 hover:text-slate-600 transition-colors cursor-pointer">下载</a>
    </div>
  {/each}
</div>