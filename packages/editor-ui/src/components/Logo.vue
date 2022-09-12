<template>
	<img
		:src="basePath + 'silva-logo.svg'"
		:class="$style.img"
		alt="silva"
	/>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
	computed: {
		basePath(): string {
			return this.$store.getters.getBaseUrl;
		},
	},
});
</script>

<style lang="scss" module>
.img {
	height: 32px;
}
</style>
