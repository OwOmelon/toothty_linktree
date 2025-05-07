<script setup lang="ts">
import Logo_Horizontal from "./Logo_Horizontal.vue";
import Logo_Vertical from "./Logo_Vertical.vue";
</script>

<template>
	<div class="logo-container bg-night-light grid place-items-center lg:p-[1em]">
		<Logo_Vertical class="lg:hidden" />
		<Logo_Horizontal class="hidden lg:block" />
	</div>
</template>

<style scoped>
@reference "@/assets/main.css";

.logo-container {
	@apply relative lg:pr-[calc(1em_+0.25em)];

	&::before {
		content: "";

		@apply bg-night-dark absolute top-1/2 right-0 hidden h-[80%] w-[0.25em] -translate-y-1/2 lg:block;
	}
}
</style>
