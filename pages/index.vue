<template>
	<v-sheet class="margin-high mx-auto rounded-lg fixed-width overflow-hidden" elevation="4">
		<v-row>
			<v-col class="pa-0 overflow-hidden">
				<img src="@/assets/hero.jpg" alt="Hero" width="100%" />
			</v-col>
			<v-divider vertical />
			<v-col class="pa-4 border-col">
				<FormDefaultLogin />
			</v-col>
		</v-row>
	</v-sheet>
</template>

<script>
export default {
	data: () => ({}),
	layout: 'login',
	components: {},
	methods: {},
	mounted() {
		this.$nextTick(() => {})
	},
}
</script>

<style scoped>
.margin-high {
	margin-top: 100px;
}
.fixed-width {
	width: 70%;
	margin: auto;
}
.border-col {
	border-left: 2px solid #c4c4c4;
}
</style>
