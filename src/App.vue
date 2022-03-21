<script setup>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Macbook from './components/Macbook.vue'
import Experience from './components/Experience.vue'
</script>

<template>
	<header class="py-6">
		<Header/>
	</header>
	<Hero/>
	<div class="mx-12">
		<Macbook>
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
		<h3 class="text-lg font-bold py-2">Experiencia</h3>
		<div class="flex space-x-8	">
			<Macbook>
				<p>2022 - <span class="text-lg font-bold py-2">SMEC</span></p>
				<img src="./assets/smec.png" alt="SMEC" class="mx-auto w-3/4">
			</Macbook>
			<Macbook>
				<p>2020 - 2021 <span class="text-lg font-bold py-2">Clinica ISV</span></p>
				<img src="./assets/clinicaisv.png" alt="SMEC" class="mx-auto w-3/4">
			</Macbook>
			<Macbook>
				<p>2018 - 2019 <span class="text-lg font-bold py-2">Gemma Graphic</span></p>
				<img src="./assets/gemg.png" alt="SMEC" class="mx-auto w-3/4">
			</Macbook>
		</div>
		<h3 class="text-lg font-bold py-2">Ultimos Trabajos</h3>
		<Experience>

		</Experience>
	</div>
</template>

<style>
</style>
