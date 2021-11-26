<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
</script>

<template>
	<header class="header-bar h-40 bg-black text-white">
		<div class="container mx-auto flex h-full">
			<router-link to="/" class="h-full flex items-center">
				<img class="block w-20" src="./assets/logo.png" alt="">
			</router-link>

			<div class="flex-grow"></div>

			<nav class="header-bar__menu-box-1">
				<ul class="flex h-full">
					<li>
						<router-link to="/" class="h-full flex items-center font-bold px-10 hover:bg-white hover:text-black">
							HOME
						</router-link>
					</li>
					<li>
						<router-link to="/article/list" class="h-full flex items-center font-bold px-10 hover:bg-white hover:text-black">
							ARTIClE LIST
						</router-link>
					</li>
				</ul>
			</nav>
		</div>
	</header>

	<main>
		<router-view></router-view>
	</main>
</template>

<style lang="postcss">
	.btn_primary{
		@apply py-2 px-4 bg-blue-600 hover:bg-blue-700 focus:ring-blue-500 focus:ring-offset-blue-200 text-white transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2 rounded-lg;
	}
	.btn-secondary{
		@apply py-2 px-4 bg-gray-600 hover:bg-gray-700 focus:ring-gray-500 focus:ring-offset-gray-200 text-white transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2 rounded-lg;
	}
	.btn-success {
	@apply py-2 px-4 bg-purple-600 hover:bg-purple-700 focus:ring-purple-500 focus:ring-offset-purple-200 text-white transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2 rounded-lg;
	}
	.btn-danger {
	@apply py-2 px-4 bg-red-600 hover:bg-red-700 focus:ring-red-500 focus:ring-offset-red-200 text-white transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2 rounded-lg;
	}
	.btn-warning {
	@apply py-2 px-4 bg-yellow-600 hover:bg-yellow-700 focus:ring-yellow-500 focus:ring-offset-yellow-200 text-white transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2 rounded-lg;
	}
	.btn-info {
	@apply py-2 px-4 bg-green-600 hover:bg-green-700 focus:ring-green-500 focus:ring-offset-green-200 text-white transition ease-in duration-200 text-center text-base font-semibold shadow-md focus:outline-none focus:ring-2 focus:ring-offset-2 rounded-lg;
	}
</style>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
