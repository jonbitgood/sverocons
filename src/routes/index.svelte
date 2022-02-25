<script>
	import Icon from "$lib/Icon.svelte"

	let icons = [
		'academic-cap','adjustments','annotation','archive','arrow-circle','arrow','arrow-narrow','arrow-sm',
		'arrows-expand','at-symbol','backspace','badge-check','ban','beaker','bell','book-open','bookmark-alt',
		'bookmark','briefcase','cake','calculator','calendar','camera','cash','chart-bar','chart-pie','chart-square-bar',
		'chat-alt-2','chat-alt','chat','check-circle','check','chevron-double','chevron','chip','clipboard-check',
		'clipboard-copy','clipboard-list','clipboard','clock','cloud-download','cloud-upload','cloud','code','cog',
		'collection','color-swatch','credit-card','cube-transparent','cube','currency-bangladeshi','currency-dollar',
		'currency-euro','currency-pound','currency-rupee','currency-yen','cursor-click','database','desktop-computer',
		'device-mobile','device-tablet','document-add','document-download','document-duplicate','document-remove',
		'document-report','document-search','document-text','document','dots-circle',
		'dots','download','duplicate','emoji-happy','emoji-sad','exclamation-circle','exclamation','external-link',
		'eye-off','eye','fast-forward','film','filter','finger-print','fire','flag','folder-add','folder-download',
		'folder-open','folder-remove','folder','gift','globe-alt','globe','hand','hashtag','heart','home','identification',
		'inbox-in','inbox','information-circle','key','library','light-bulb','lightning-bolt','link','location-marker',
		'lock-closed','lock-open','login','logout','mail-open','mail','map','menu-alt-1','menu-alt-2','menu-alt-3','menu-alt-4',
		'menu','microphone','minus-circle','minus-sm','minus','moon','music-note','newspaper','office-building','paper-airplane',
		'paper-clip','pause','pencil-alt','pencil','phone-incoming','phone-missed-call','phone-outgoing','phone','photograph',
		'play','plus-circle','plus-sm','plus','presentation-chart-bar','presentation-chart-line','printer','puzzle','qrcode',
		'question-mark-circle','receipt-refund','receipt-tax','refresh','reply','rewind','rss','save-as','save','scale','scissors',
		'search-circle','search','selector','server','share','shield-check','shield-exclamation','shopping-bag','shopping-cart',
		'sort-ascending','sort-descending','sparkles','speakerphone','star','status-offline','status-online','stop','sun','support',
		'switch-horizontal','switch-vertical','table','tag','template','terminal','thumb-down','thumb-up','ticket','translate','trash',
		'trending-down','trending-up','truck','upload','user-add','user-circle','user-group','user-remove','user','users','variable',
		'video-camera','view-boards','view-grid-add','view-grid','view-list','volume-off','volume-up','wifi','x-circle','x','zoom-in',
		'zoom-out'
]
</script>

<div class="flex flex-col px-12 max-w-prose mx-auto mt-12 text-center">
	<div class="py-12">
		<h1 class="text-xl mb-4">Sverocons</h1>
		<p class="text-lg text-gray-400">
			A simple svelte wrapper for the <a href="https://heroicons.com/" class="text-purple-800 bold">Heroicons Library</a> taking inspiration from 
			the <a href="https://svelte.recipes/components/icon/">component approach</a> to svg icons by <a href="https://github.com/Wattenberger">Amelia Wattenberger</a>.
		</p>
	</div>
	<div class="-my-2 overflow-x-auto sm:-mx-6 lg:-mx-8">
	  <div class="py-2 align-middle inline-block min-w-full sm:px-6 lg:px-8">
		<div class="shadow overflow-hidden border-b border-gray-200 sm:rounded-lg">
		  <table class="min-w-full divide-y divide-gray-200">
			<thead class="bg-gray-50">
			  <tr>
				<th scope="col" class="px-6 py-3 text-left text-xs text-gray-500 uppercase tracking-wider">key</th>
				<th scope="col" class="px-6 py-3 text-left text-xs text-gray-500 uppercase tracking-wider">solid</th>
				<th scope="col" class="px-6 py-3 text-left text-xs text-gray-500 uppercase tracking-wider">outline</th>
			  </tr>
			</thead>
			<tbody>
				{#each icons as icon}
				<tr>
					<td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900">{ icon }</td>
					<td class="px-6 py-4 whitespace-nowrap text-sm text-gray-900"><Icon name={ icon } type="solid" /></td>
					<td class="px-6 py-4 whitespace-nowrap text-sm text-gray-500"><Icon name={ icon } type="outline" /></td>
				</tr>
				{/each}
			</tbody>
		  </table>
		</div>
	  </div>
	</div>
  </div>
  