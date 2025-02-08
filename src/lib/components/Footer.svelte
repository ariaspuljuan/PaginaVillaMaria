<footer class="py-20 bg-gray-100">
	<div class="max-w-screen-xl mx-auto flex justify-between space-x-14">
		<div class="flex flex-col space-y-6 w-1/4">
			<img src="/images/villaMariaLogo.png" width={200} height={24} alt="Screeno Logo" />
			<p>Es para nosotros un gusto poder recibirlo</p>
			<div class="flex space-x-4">
				<img src="/icons/facebook.svg" alt="Facebook" />
				<img src="/icons/instagram.svg" alt="Instagram" />
			</div>
		</div>
		<div class="flex flex-col space-y-6 w-1/4">
			<h6 class="font-semibold font-heading">Contacto e informacion</h6>
			<div class="flex items-start space-x-2">
				<img src="/icons/location.svg" alt="Location Icon" />
				<p>Verda Caicedos en Ramiriquí Boyacá</p>
			</div>
			<div class="flex items-center space-x-2">
				<img src="/icons/phone.svg" alt="Phone Icon" />
				<p>+57 3227869892</p>
			</div>
			<div class="flex items-center space-x-2">
				<img src="/icons/email-blue.svg" alt="Email Icon" />
				<p>villamariahostal@gmail.com</p>
			</div>
		</div>
		<div class="flex flex-col space-y-6 w-1/2">
			<h6 class="font-heading font-semibold">Nosotros lo Contactaremos</h6>
			<form class="flex flex-col space-y-6">
				<input type="text" placeholder="Your name" />
				<input type="email" placeholder="Your email" />
				<textarea placeholder="Your message" rows={5} />
				<div>
					<button class="primary font-heading font-semibold px-8">Enviar</button>
				</div>
			</form>
		</div>
	</div>
</footer>
<div class="border-t-[1px] border-neutral-300 text-center py-4">
	<p>©2025 Villa Maria Web, Todos los derechos reservados</p>
</div>

<style lang="postcss">
	input,
	textarea {
		@apply text-neutral-700 py-3 px-4 outline-none rounded-xl border-[1px] border-white focus:border-primary transition duration-300;
	}
</style>
