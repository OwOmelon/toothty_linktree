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
