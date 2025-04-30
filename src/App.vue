<script setup lang="ts">
import Pfp from "@/components/Pfp.vue";
import Logo_Horizontal from "@/components/Logo_Horizontal.vue";
import Logo_Vertical from "@/components/Logo_Vertical.vue";
import Links from "@/components/Links.vue";
import GrainOverlay from "@/components/GrainOverlay.vue";
</script>

<template>
	<div
		class="debug-outline-[orange] hidden grid w-217.5 grid-cols-[33.33%_auto] gap-5"
	>
		<Pfp />

		<div class="text-night-dark flex h-full flex-col">
			<div
				class="bg-night-light grid grow grid-cols-[auto_auto_auto] gap-2.5 px-4 py-2.5"
			>
				<Logo_Horizontal class="self-end" />
				<i class="block w-1 self-stretch bg-[currentColor]" />
				<div class="flex flex-col justify-center p-2 font-semibold">
					<p>age • pronouns</p>
					<p>
						Lorem ipsum dolor sit amet consectetur. Vulputate platea sit non
						erat curabitur
					</p>
				</div>
			</div>

			<div class="bg-night-light px-2.5">
				<i class="block h-1 bg-[currentColor]" />
			</div>

			<Links />
		</div>
	</div>

	====================

	<div
		class="hidden debug-outline-[orange]/ drop-shadow-night-light/25 grid w-[34.75em] grid-cols-[61%_auto] gap-[1.25em] text-[2.5vw] drop-shadow-[0_0_0.25em] md:text-base"
	>
		<Pfp />
		<div class="bg-night-light grid place-items-center">
			<Logo_Vertical />
		</div>
		<Links class="col-[1/-1]" />
		<div
			class="col-[1/-1] grid grid-cols-[min-content,_min-content,_auto] gap-3 font-semibold"
		>
			<p class="col-start-1">age • pronouns</p>
			<p class="col-start-2">|</p>
			<p class="col-start-3">
				Lorem ipsum dolor sit amet consectetur. Vulputate platea sit non erat
				curabitur
			</p>
		</div>
	</div>

	====================

	<div
		class="drop-shadow-night-light/25 lg:rows-[auto_auto] grid w-[34.75em] grid-cols-[61%_auto] gap-[1.25em] text-[min(2.5vw,_1rem)] drop-shadow-[0_0_0.25em] lg:w-[54.375em] lg:grid-cols-[33.33%_min-content_auto] lg:gap-0 lg:text-base"
	>
		<Pfp class="lg:row-start-1 lg:row-end-3" />

		<div class="bg-night-light grid place-items-center lg:p-[1em] lg:ml-[1.25em]">
			<Logo_Vertical class="lg:hidden" />
			<Logo_Horizontal class="hidden lg:block" />
		</div>

		<Links class="col-[1/-1] lg:col-[2/-1] lg:ml-[1.25em]" />

		<div
			class="lg:px-3 lg:bg-night-light lg:text-night-dark col-[1/-1] grid grid-cols-[min-content,_min-content,_auto] gap-[0.75em] font-semibold lg:col-start-3 lg:row-start-1 lg:flex lg:justify-center flex-col"
		>
			<!-- <p class="col-start-1">age • pronouns</p>
			<p class="col-start-2">|</p>
			<p class="col-start-3">
				Lorem ipsum dolor sit amet consectetur. Vulputate platea sit non erat
				curabitur
			</p> -->

			<p>age • pronouns</p>
			<p>
				Lorem ipsum dolor sit amet consectetur. Vulputate platea sit non erat
				curabitur
			</p>
		</div>
	</div>

	<GrainOverlay />
</template>

<style lang="postcss"></style>
