<script setup lang="ts">
useHead({
	title: 'LOGIN',
});
</script>

<template>
	<div>
		<p>{{ $t('pages.landing.title') }}</p>
		<router-link
			:to="{ name: 'home' }"
			class="
				mt-5
				hover:text-gray-200
				dark:hover:text-gray-500
				hover:underline
			"
			>{{ $t('hui-dao-shou-ye') }}</router-link
		>
	</div>
	{{ $t('page.landing.hi') }}
</template>

<style scoped></style>

<route lang="yaml">
name: login
</route>
