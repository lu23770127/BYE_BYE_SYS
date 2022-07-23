<script setup lang="ts">
useHead({
	title: 'LOGIN',
});
</script>

<template>
	<!-- component -->
	<div class="max-h-screen">
		<div class="flex justify-center">
			<div class="flex items-center w-full max-w-md p-6 mx-auto lg:w-2/6">
				<div class="flex-1">
					<icon-la:book-dead
						class="h-20 w-20 p-1 m-auto"
						style="color: #06b6d4"
					/>
					<div class="text-center">
						<h2
							class="
								text-4xl
								font-bold
								text-center text-gray-700
								dark:text-white
								p-5
							"
						>
							{{ $t('bye-bye-sys') }}
						</h2>

						<p class="mt-3 text-gray-500 dark:text-gray-300">
							{{
								$t('pages.login.sign-in-to-access-your-account')
							}}
						</p>
					</div>

					<div class="mt-8">
						<form>
							<div>
								<label
									for="email"
									class="
										block
										mb-2
										text-sm text-gray-600
										dark:text-gray-200
									"
									>{{ $t('pages.login.email') }}</label
								>
								<input
									type="email"
									name="email"
									id="email"
									placeholder="example@example.com"
									class="
										block
										w-full
										px-4
										py-2
										mt-2
										text-gray-700
										placeholder-gray-400
										bg-white
										border border-gray-200
										rounded-md
										dark:placeholder-gray-600
										dark:bg-gray-900
										dark:text-gray-300
										dark:border-gray-700
										focus:border-cyan-400
										dark:focus:border-cyan-400
										focus:ring-cyan-400
										focus:outline-none
										focus:ring
										focus:ring-opacity-40
									"
								/>
							</div>

							<div class="mt-6">
								<div class="flex justify-between mb-2">
									<label
										for="password"
										class="
											text-sm text-gray-600
											dark:text-gray-200
										"
										>{{ $t('pages.login.password') }}</label
									>
									<a
										href="#"
										class="
											text-sm text-gray-400
											focus:text-cyan-500
											hover:text-cyan-500 hover:underline
										"
										>{{
											$t('pages.login.forgetPassword')
										}}</a
									>
								</div>

								<input
									type="password"
									name="password"
									id="password"
									placeholder="{{
									$t('pages.login.yourPassword')
								}}"
									class="
										block
										w-full
										px-4
										py-2
										mt-2
										text-gray-700
										placeholder-gray-400
										bg-white
										border border-gray-200
										rounded-md
										dark:placeholder-gray-600
										dark:bg-gray-900
										dark:text-gray-300
										dark:border-gray-700
										focus:border-cyan-400
										dark:focus:border-cyan-400
										focus:ring-cyan-400
										focus:outline-none
										focus:ring
										focus:ring-opacity-40
									"
								/>
							</div>

							<div class="mt-6">
								<button
									class="
										w-full
										px-4
										py-2
										tracking-wide
										text-white
										transition-colors
										duration-200
										transform
										bg-cyan-500
										rounded-md
										hover:bg-cyan-400
										focus:outline-none
										focus:bg-cyan-400
										focus:ring
										focus:ring-cyan-300
										focus:ring-opacity-50
									"
								>
									{{ $t('pages.login.loginButton') }}
								</button>
							</div>
						</form>

						<p class="mt-6 text-sm text-center text-gray-400">
							{{ $t('pages.login.dontHaveAccount') }}
							<a
								href="#"
								class="
									text-cyan-500
									focus:outline-none focus:underline
									hover:underline
								"
								>{{ $t('pages.login.signup') }}</a
							>.
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped></style>

<route lang="yaml">
name: login
</route>
