<script lang="ts">
	const features = [
		{
			title: '☕ Librería y cafetería',
			icon: 'upload',
			description:
				'Detalles sobre el café, menú y libros disponibles. '
		},
		{
			title: '🛏️ Habitaciones disponibles',
			icon: 'record',
			description: 'Tipos de habitaciones, características y comodidades.'
		},
		{
			title: '📍 Ubicación y cómo llegar',
			icon: 'stream',
			description: 'Mapa de Google Maps e instrucciones de acceso.'
		},
		{
			title: '📌 Información de costos ',
			icon: 'monetization',
			description: 'Tarifas de hospedaje y consumos en la librería-café.'
		},
		{
			title: '📅 Reservas y contacto',
			icon: 'stream',
			description: 'Formulario o información para hacer reservas.'
		},
		{
			title: '📝 Opiniones y testimonios',
			icon: 'device',
			description: 'Experiencias de huéspedes y clientes.'
		}
	]
</script>

<section class="py-20 text-white bg-black">
	<div class="max-w-screen-xl mx-auto">
		<div class="flex items-center space-x-24">
			<div class="flex flex-col w-1/2">
				<div class="flex flex-col space-y-4">
					<h1 class="text-5xl font-bold font-heading">Bienvenidos a Villa María Hostal<h2 class="text-3xl font-semibold">Un refugio acogedor para viajeros y amantes de la lectura</h2></h1>
					<p>
						En Villa María Hostal, combinamos la calidez de un hospedaje confortable con el encanto de una librería y la tranquilidad de un café. Ubicado en un entorno acogedor, nuestro hostal es el lugar ideal para descansar, descubrir nuevas historias y disfrutar de momentos únicos.
						Disfruta de nuestras cómodas habitaciones, sumérgete en una buena lectura en nuestra librería y relájate con una taza de café recién preparado. Ya sea que busques una escapada tranquila o una experiencia cultural enriquecedora, en Villa María Hostal encontrarás el equilibrio perfecto entre descanso e inspiración.
						¡Te invitamos a ser parte de nuestra historia!
					</p>
				</div>
				<div class="flex mt-12 space-x-3">
					<button class="w-1/3 primary">Ubicacion</button>
					<button class="w-1/3 outline">Servicios</button>
				</div>
			</div>
			<div class="relative w-1/2">
				<img src="/images/casa8.jpg" class="w-full h-full" alt="Hero" />
				<img src="/images/vista3.jpg" class="absolute -bottom-4 -left-3" alt="Hero" />
			</div>
		</div>
		<!-- <div class="flex justify-between mt-32 space-x-24">
			<img
				src="/images/apple-tv.svg"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Apple TV"
			/>
			<img
				src="/images/android-tv.svg"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Android TV"
			/>
			<img
				src="/images/apple-watch.svg"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Apple Watch"
			/>
			<img
				src="/images/iphone.svg"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="iPhone"
			/>
			<img
				src="/images/android.svg"
				class="transform transition duration-300 hover:scale-110 cursor-pointer"
				alt="Android"
			/>
		</div> -->
	</div>
</section>

<section class="py-20">
	<div class="max-w-screen-lg mx-auto">
		<div class="flex flex-col justify-center text-center">
			<div class="flex flex-col space-y-3">
				<h2 class="text-4xl font-bold font-heading"> Descanso, Letras y Café: Una Experiencia Única en la Naturaleza</h2>
				<p>Un refugio acogedor donde el descanso, la lectura y el buen café se encuentran en armonía con la naturaleza.</p>
			</div>
			<!--
						<div class="flex justify-center mt-12 space-x-8">
							<button class="w-1/6 primary">Start Free Trial</button>
							<button class="w-1/6 outline-dark">Login</button>
						</div>
			-->
		</div>
		<div class="grid grid-cols-3 gap-12 mt-20">
			{#each features as feature}
				<div
					class="flex flex-col p-4 space-y-3 hover:shadow-xl transition duration-300 cursor-pointer"
				>
					<div class="flex space-x-3">
						<img
							src={`/icons/${feature.icon}.svg`}
							class="transform transition duration-300 hover:rotate-12"
							alt={feature.title}
						/>
						<h5 class="font-bold font-heading">{feature.title}</h5>
					</div>
					<p>{feature.description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>

<section class="py-20 text-white bg-black">
	<div class="flex flex-col max-w-screen-xl mx-auto space-y-32">
		<div class="flex flex-col justify-center">
			<h2 class="text-4xl font-bold text-center font-heading">Instalaciones</h2>
		</div>

		<div class="flex space-x-24">
			<div class="flex flex-col justify-center w-1/2 space-y-6">
				<h5 class="text-3xl font-semibold">Sala</h5>
				<p>
					Un área acogedora y funcional donde podrás relajarte, leer, trabajar o conversar. Equipada con cómodos asientos, una selección de libros y un ambiente tranquilo, es el lugar ideal para disfrutar de un momento de descanso acompañado de un buen café.
				</p>
				<!--
								<div class="flex space-x-3 cursor-pointer group">
									<p class="transition font-heading group-hover:font-bold">Get started</p>
									<img
										src="/icons/arrow.svg"
										class="transition transform group-hover:translate-x-1"
										alt="Arrow Icon"
									/>
								</div>
				-->
			</div>
			<div class="relative w-1/2">
				<img src="/images/sala2.jpg" alt="Monetize your way" class="w-full h-full" />
				<!--
								<div
									class="absolute flex flex-col py-8 space-y-3 text-black bg-white px-9 rounded-3xl -top-4 -left-6"
								>
									<div
										class="flex w-full px-3 py-4 space-x-16 font-semibold transition duration-300 transform bg-gray-100 font-heading rounded-xl hover:bg-blue-100 hover:text-primary hover:translate-x-1 hover:-translate-y-1 hover:shadow-xl"
									>
										<p>Donate</p>
										<p>45$</p>
									</div>
									<div
										class="flex w-full px-3 py-4 space-x-16 font-semibold transition duration-300 transform bg-gray-100 font-heading rounded-xl hover:bg-blue-100 hover:text-primary hover:translate-x-1 hover:-translate-y-1 hover:shadow-xl"
									>
										<p>Donate</p>
										<p>45$</p>
									</div>
									<div
										class="flex w-full px-3 py-4 space-x-16 font-semibold transition duration-300 transform bg-gray-100 font-heading rounded-xl hover:bg-blue-100 hover:text-primary hover:translate-x-1 hover:-translate-y-1 hover:shadow-xl"
									>
										<p>Donate</p>
										<p>45$</p>
									</div>
								</div>
				-->
			</div>
		</div>

		<div class="flex space-x-24">
			<div class="relative flex w-1/2">
				<img src="/images/habitacion3.jpg" class="w-full h-full" alt="Optimized for growth" />
				<div class="absolute px-4 py-3 bg-white -top-4 -right-4 rounded-2xl">
					<div class="relative">
						<img src="/icons/email-black.svg" alt="Email Icon" class="w-8 h-6" />
						<span
							class="absolute text-xs rounded-full -top-2 -right-2 bg-primary px-[6px] py-[1px] font-heading font-bold"
							>1</span
						>
					</div>
				</div>
			</div>
			<div class="flex flex-col justify-center w-1/2 space-y-6">
				<h5 class="text-3xl font-semibold">Nuestras Habitaciones: Comodidad para tu Estancia</h5>
				<p>
					Espacios cómodos y acogedores, ideales para un descanso tranquilo en un ambiente natural y relajante.
				</p>
				<!--
				<div class="flex space-x-3 cursor-pointer group">
					<p class="transition font-heading group-hover:font-bold">Get started</p>
					<img
						src="/icons/arrow.svg"
						class="transition transform group-hover:translate-x-1"
						alt="Arrow Icon"
					/>
				</div>
				-->
			</div>
		</div>
	</div>
</section>

<section class="pt-20 pb-40 text-white bg-black">
	<div class="flex flex-col max-w-screen-lg mx-auto">
		<div class="flex flex-col space-y-3 text-center">
			<h2 class="text-4xl font-bold font-heading">Ubicacion en Google Maps</h2>
			<p>Encuéntranos fácilmente en Google Maps y descubre cómo llegar a Villa María Hostal (Librería-Café), un rincón acogedor en medio de la naturaleza.</p>
		</div>
		<!--
				<div class="flex justify-center space-x-8 mt-14">
					<button class="w-1/5 secondary">Get started</button>
					<button class="w-1/5 outline">Login</button>
				</div>
		-->
		<div class="relative mt-20">
			<!-- svelte-ignore a11y_missing_attribute -->
			<!-- svelte-ignore a11y-missing-attribute -->
			<iframe
				src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3966.073013073073!2d-73.3610736857367!3d5.536366395253073!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8e5b8b1b1b1b1b1b%3A0x1b1b1b1b1b1b1b1b!2sVilla%20Mar%C3%ADa%20Hostal!5e0!3m2!1ses!2sco!4v1633663666824!5m2!1ses!2sco"
				width="100%"
				height="300"
				style="border:0;"
				allowfullscreen=""
				loading="lazy"
			></iframe>
			<!--
			<img src="/images/business-desktop.png" alt="Business Desktop" class="w-full h-full" />
			<img
				src="/images/business-mobile.png"
				alt="Business Mobile"
				class="absolute -bottom-12 -left-3"
			/>
			-->
		</div>
	</div>
</section>

<section class="pt-20 pb-32">
	<div class="flex flex-col justify-center space-y-3 text-center">
		<h2 class="text-4xl font-bold font-heading">Galeria</h2>
		<p>Explora la esencia de Villa María Hostal (Librería-Café) a través de imágenes. Descubre nuestros espacios acogedores, la calidez de nuestras habitaciones, el encanto de nuestra librería-café y la belleza natural que nos rodea. ¡Déjate inspirar y ven a vivir la experiencia por ti mismo!</p>
	</div>

	<div class="flex flex-col overflow-hidden mt-24 space-y-6">
		<div class="flex space-x-8">
			<img src="/images/vista4-720.jpg" alt="Showcase 1" class="w-[360px] h-[201px]" />
			<img src="/images/vista1-720.jpg" alt="Showcase 2" class="w-[360px] h-[201px]" />
			<img src="/images/vista6-720.jpg" alt="Showcase 3" class="w-[360px] h-[201px]" />
			<img src="/images/quiosco2-720.jpg" alt="Showcase 4" class="w-[360px] h-[201px]" />
		</div>
		<div class="flex space-x-8 -translate-x-72">
			<img src="/images/vista4-720.jpg" alt="Showcase 5" class="w-[360px] h-[201px]" />
			<img src="/images/vista5-720.jpg" alt="Showcase 6" class="w-[360px] h-[201px]" />
			<img src="/images/vista1-720.jpg" alt="Showcase 7" class="w-[360px] h-[201px]" />
			<img src="/images/quiosco2-720.jpg" alt="Showcase 8" class="w-[360px] h-[201px]" />
			<img src="/images/vista6-720.jpg" alt="Showcase 9" class="w-[360px] h-[201px]" />
		</div>
	</div>
</section>
