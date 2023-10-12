<script lang="ts" setup>
defineOptions({
	name: 'Counter',
})
const counter = createCounter()
</script>

<template>
	<button
		class="inline-block cursor-pointer rounded from-pink-500 via-red-500 to-yellow-500 bg-gradient-to-r px-8 py-2 text-sm font-medium text-white transition !border-0 !outline-none"
		hover="scale-110 shadow-xl"
		@click="counter.inc()"
	>
		{{ counter.count }}
	</button>

	<el-row class="mb-4">
		<el-button>Default</el-button>
		<el-button type="primary">Primary</el-button>
		<el-button type="success">Success</el-button>
		<el-button type="info">Info</el-button>
		<el-button type="warning">Warning</el-button>
		<el-button type="danger">Danger</el-button>
	</el-row>
</template>
