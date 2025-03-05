<script setup></script>

<template>
	<section>
		<div class="container container-big">
			<div class="d-flex flex-column col-12 col-lg-6">
				<p class="subtitle mb-40px">Modern art</p>
				<slot name="title">
					<h1 class="title-1">
						{{ title }}
					</h1>
				</slot>
				<p class="mb-40px">
					Nibh nisl condimentum venenatis a condimentum vitae sapien dignissim
					sodales. Consequat ac felis ridiculus mus mauris vitae ultricies leo
					integer malesuada.
				</p>
				<a href="" class="btn btn-md">Styl jest</a>
			</div>
		</div>
		<div class="heroimages col-12 col-lg6">
			<div class="heroimagesitem">
				<img src="/src/assets/images/hellspit.jpg" alt="" />
			</div>
			<div class="heroimagesitem">
				<img src="/src/assets/images/bangpow.jpg" alt="" />
			</div>
			<div class="heroimagesitem">
				<img src="/src/assets/images/Jeckelbros.jpg" alt="" />
			</div>
		</div>

		<img src="" alt="" />
	</section>
</template>

<style lang="scss" scoped>
.hero {
	&images {
		position: relative;

		&__item {
			position: absolute;
			transition: all 800ms;

			&:nth-of-type(1) {
				transition-delay: 600ms;
			}

			&:nth-of-type(2) {
				transition-delay: 1200ms;
			}

			&:nth-of-type(3) {
				transition-delay: 1800ms;
			}

			&:nth-of-type(4) {
				transition-delay: 2400ms;
			}

			&:nth-of-type(5) {
				transition-delay: 3000ms;
			}
		}
	}
}
</style>
