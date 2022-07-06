<script setup>
	const props = defineProps({
		color: {
			type: String,
			required: false,
			default: '#f00'
		}
	})
</script>

<template>
	<button
		class="pam-button"
		:style="{ backgroundColor: color }"
	>
		<slot />
	</button>
</template>

<style lang="postcss" scoped>
.pam-button {
	@apply rounded-md;
}
</style>