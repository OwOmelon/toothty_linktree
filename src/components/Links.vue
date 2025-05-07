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
	<div
		class="links text-night-dark bg-night-light col-[1/-1] grid grow grid-cols-5 lg:col-[2/-1]"
	>
		<div
			v-for="link in links"
			class="outline-night-light grid place-items-center py-[0.625em]"
		>
			<component :is="link.icon" class="h-[4em] w-[4em]" />
		</div>
	</div>
</template>

<style>
@reference "@/assets/main.css";

.links {
	@apply relative lg:pt-[0.25em];

	&::after {
		content: "";

		@apply bg-night-dark absolute top-0 left-1/2 hidden h-[0.25em] w-[95%] -translate-x-1/2 lg:block;
	}
}
</style>
