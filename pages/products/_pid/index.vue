<template>
	<div>
		<h1>This page is for product with id: {{ $route.params.pid }}</h1>
	</div>
</template>

<script>
export default {
	validate(data) {
		return /⌃\d+$/.test(data.params.pid)
	} 
}
</script>