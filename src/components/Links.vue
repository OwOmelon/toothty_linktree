<script setup lang="ts">
import IconYoutube from "~icons/ri/youtube-fill";
import IconInstagram from "~icons/ri/instagram-fill";
import IconX from "~icons/ri/twitter-x-fill";
import IconTiktok from "~icons/ri/tiktok-fill";
import IconTwitch from "~icons/ri/twitch-fill";

const links = [
	{
		icon: IconYoutube,
	},
	{
		icon: IconInstagram,
	},
	{
		icon: IconX,
	},
	{
		icon: IconTiktok,
	},
	{
		icon: IconTwitch,
	},
];
</script>

<template>
	<div class="flex grow text-night-dark">
		<div
			v-for="link in links"
			class="outline-night-light bg-night-light hover:text-night-light grid w-full place-items-center py-[0.625em] outline-[0.125em] -outline-offset-[0.125em] outline-solid hover:bg-transparent"
		>
			<component :is="link.icon" class="h-[4em] w-[4em]" />
		</div>
	</div>
</template>
