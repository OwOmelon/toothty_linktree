<script setup lang="ts">
import Pfp from "@/components/Pfp.vue";
import LogoContainer from "@/components/logo/LogoContainer.vue";
import Desc from "@/components/Desc.vue";
import Links from "@/components/Links.vue";

import ValoBg from "@/components/ValoBg.vue"
import GrainOverlay from "@/components/GrainOverlay.vue";
</script>

<template>
	<div
		class="drop-shadow-night-light/25 lg:rows-[auto_auto] grid w-[34.75em] grid-cols-[61%_auto] gap-[1.25em] text-[min(2.5vw,_1rem)] drop-shadow-[0_0_0.25em] lg:w-[54.375em] lg:grid-cols-[33.33%_min-content_auto] lg:gap-0 lg:text-base"
	>
		<Pfp />
		<LogoContainer />
		<Links />
		<Desc />
	</div>

	<ValoBg />
	<GrainOverlay />
</template>

<style>
@reference "@/assets/main.css";

.logo-container,
.links {
	@apply lg:ml-[1.25em];
}
</style>
