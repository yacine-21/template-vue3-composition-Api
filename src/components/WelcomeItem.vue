<template>
	<div>
		<h1 class="underline text-red-600">Hello world</h1>
		<p>{{ name }}</p>
	</div>
</template>

<script>
import { ref, onMounted } from "vue";

export default {
	setup() {
		const name = ref("");

		onMounted(() => {
			name.value = "Yacine";
		});

		return {
			name
		};
	}
};
</script>

<style lang="scss" scoped></style>
