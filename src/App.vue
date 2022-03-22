<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Macbook from './components/Macbook.vue'
import Experience from './components/Experience.vue'

import GithubIcon from './components/icons/IconGithub.vue'
import LinkedinIcon from './components/icons/IconLinkedin.vue'
import ArrowRightIcon from './components/icons/IconArrowRight.vue'
import ArrowLeftIcon from './components/icons/IconArrowLeft.vue'
</script>

<template>
	<header class="py-6">
		<Header/>
	</header>
	<Hero/>
	<div class="mx-12">
		<Macbook url>
			<div class="container ">
				<pre><code>
					<span class="text-[#7000FF]">.SobreMi</span> {
						<span class="text-[#0EE6B7]">Profesion:</span> Fullstack Developer;       
						<span class="text-[#0EE6B7]">Lenguajes:</span> PHP, JS, SQL, CSS; 
					}
					<span class="text-[#7000FF]">.Educacion</span> {
						<span class="text-[#0EE6B7]">DuocUC:</span> Analista Desarrollador       
						de Aplicaciones Software; 
					}</code></pre>
			</div>
		</Macbook>
		<h3 id="exp" class="text-lg font-bold py-10">Experiencia</h3>
		<div class="flex flex-wrap md:flex-nowrap md:space-x-8">
			<Macbook>
				<p class="py-2 ml-12">2022 - <span class="text-lg font-bold">SMEC</span></p>
				<img src="./assets/smec.png" alt="SMEC" class="mx-auto w-3/4 py-10">
			</Macbook>
			<Macbook>
				<p class="py-2 ml-12">2020 - 2021 - <span class="text-lg font-bold">Clinica ISV</span></p>
				<img src="./assets/clinicaisv.png" alt="SMEC" class="mx-auto w-3/4 py-5">
			</Macbook>
			<Macbook>
				<p class="py-2 ml-12">2018 - 2019 - <span class="text-lg font-bold">Autónomo</span></p>
				<img src="./assets/gemg.png" alt="SMEC" class="mx-auto w-2/4">
			</Macbook>
		</div>
		<h3 id="works" class="text-lg font-bold py-10">Ultimos Trabajos</h3>
		<Experience>
			<template #imagen>
				<img src="./assets/gestor.png" alt="">
			</template>
			<template #header>Gestor de Examenes y Cursos</template>
			Lorem ipsum dolor sit amet consectetur, adipisicing elit. Impedit veniam temporibus consequatur. Eaque.
			<template #footer>
				<a href="#">Ver Proyecto</a>
				<ArrowRightIcon class="ml-3"/>
			</template>
		</Experience>
		<Experience inverso>
			<template #imagen>
				<img src="./assets/tih.png" alt="">
			</template>
			<template #header>Time on Tools</template>
			Lorem ipsum dolor sit amet consectetur, adipisicing elit. Impedit veniam temporibus consequatur. Eaque.
			<template #footer>
				<ArrowLeftIcon class="mr-3"/>
				<a href="#">Ver Proyecto</a>
			</template>
		</Experience>
		<Experience>
			<template #imagen>
				<img src="./assets/agenda.png" alt="">
			</template>
			<template #header>Agenda Clínica</template>
			Lorem ipsum dolor sit amet consectetur, adipisicing elit. Impedit veniam temporibus consequatur. Eaque.
			<template #footer>
				<a href="#">Ver Proyecto</a>
				<ArrowRightIcon class="ml-3"/>
			</template>
		</Experience>
		<div id="hire" class="container text-center py-8">
			<p>!Me gustaría tener tu contacto!</p>
			<div class="container w-min mx-auto my-4">
				<div class="flex space-x-14">
					<a href="https://www.linkedin.com/in/alexmatias-castillo/">
						<GithubIcon class="w-12" />
					</a>
					<a href="https://github.com/14714">
						<LinkedinIcon class="w-12" />
					</a>
				</div>
			</div>
			<h4 class="my-6 font-bold">
				¿Tenes un proyecto en mente? ¡Hagamoslo realidad!
			</h4>
			<a class="text-[#0EE6B7]" href="mailto:rivera.matias@hotmail.com">rivera.matias@hotmail.com</a>
		</div>
		<p>Tecnologías ocupadas: Vite, Vue y Tailwind</p>
	</div>
</template>

<style>
</style>
