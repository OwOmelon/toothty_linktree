<template>
	<svg class="hidden">
		<filter id="grain">
			<feTurbulence type="turbulence" baseFrequency="0.33" />
		</filter>
	</svg>

	<div
		style="filter: url(#grain) grayscale(100%)"
		class="pointer-events-none fixed top-0 left-0 z-50 h-full w-full opacity-25"
	/>
</template>
