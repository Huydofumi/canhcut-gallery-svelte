<script lang="ts">
	import NavBar from './NavBar.svelte';
	import NavBarMobile from './NavBarMobile.svelte';
	import sunIcon from '@iconify-icons/material-symbols/sunny-outline-rounded';
	import festivalIcon from '@iconify-icons/material-symbols/festival-rounded';

	const services: ServiceItem[] = [
		{
			name: 'Chụp outdoor',
			description: 'Dành cho các bạn muốn chụp ở outdoor',
			icon: sunIcon
		},
		{
			name: 'Chụp ở studio khác',
			description: 'Dành cho các bạn thích ảnh bên mình và muốn shoot theo concept ở studio khác',
			icon: {
				width: 20,
				height: 20,
				body: `<g fill="currentColor" fill-rule="evenodd" clip-rule="evenodd">
		<path d="M14.168 4.872c.997-.665 2.332.05 2.332 1.248v3.263c0 1.198-1.335 1.913-2.332 1.248l-2.945-1.963l.554-.832l2.946 1.963a.5.5 0 0 0 .777-.416V6.12a.5.5 0 0 0-.777-.416l-2.946 1.964l-.554-.832zm-.711 13.083a.5.5 0 0 1-.66.254L9 16.52v1.73a.5.5 0 0 1-1 0v-1.73l-3.797 1.688a.5.5 0 0 1-.406-.914L8 15.427v-4.175a.5.5 0 1 1 1 0v4.175l4.203 1.868a.5.5 0 0 1 .254.66" />
		<path d="M5 5.752a1.5 1.5 0 0 1 1.5-1.5h4a1.5 1.5 0 0 1 1.5 1.5v4a1.5 1.5 0 0 1-1.5 1.5h-4a1.5 1.5 0 0 1-1.5-1.5zm1.5-.5a.5.5 0 0 0-.5.5v4a.5.5 0 0 0 .5.5h4a.5.5 0 0 0 .5-.5v-4a.5.5 0 0 0-.5-.5z" />
		<path d="M11.146 5.605a.5.5 0 0 1 0-.707l3-3a.5.5 0 0 1 .708.707l-3 3a.5.5 0 0 1-.708 0m3.708 8a.5.5 0 0 1-.708 0l-3-3a.5.5 0 0 1 .707-.707l3 3a.5.5 0 0 1 0 .707" />
	</g>`
			},
			sizeInPx: 28
		},
		{
			name: 'Chụp ảnh tại festival',
			description: 'Dành cho các bạn muốn bọn mình chụp ảnh các bạn tại các festival',
			icon: festivalIcon
		}
	];
</script>

<header class="inline-flex items-center min-h-4 w-full px-3 py-3 sm:px-4 sm:py-4 justify-between shadow-none bg-white dark:bg-gray-950">
	<div class="flex">
		<a href="/" class="px-1">
			<img class="h-8 w-auto" src="/images/weblogo2.webp" alt="logo" />
		</a>
	</div>
	<NavBar {services} />
	<NavBarMobile {services} />
</header>
