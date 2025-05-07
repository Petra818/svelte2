<script>
	import { assets } from '$app/paths';

	import { Aperture, Menu} from '@lucide/svelte';


	import '../app.css';
	import { page } from '$app/state';
	import { render } from 'svelte/server';
	import Footer from '$lib/components/Footer.svelte';
	import { afterNavigate } from '$app/navigation';


	let { children } = $props();
	let mobileNavOpen = $state(false)

	afterNavigate(() => {
		mobileNavOpen = false;
	});
</script>

<header class="  h-15 justify-center flex border-b-2 bg-gray-400">
<!-- MOBILE -->
<button
		class=""
		onclick={() => {
			mobileNavOpen = !mobileNavOpen;
		}}><Menu /></button>
	
 <section class=" absolute left-0 right-0 flex-col  lg:hidden {mobileNavOpen ? 'flex top-0.5 duration-1000' : 'top-[-1000px] duration-2000'}">
	<div class=" bg-gray-300 gabarito-uniquifier w-full mt-14 fixed left-0 p-6 border-t-gray-500 border-t-2 border-b-2   ">
		<div class=" justify-center  items-center flex">
		<a class="hover:bg-gray-500  rounded-4xl p-3 " href="/">Domov</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/aboutme">O nás</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/websites">Stránky</a>
		</div>
			<div class="justify-center items-center flex " >	
		<Aperture class='size-10 stroke-2 text-black '/>
		</div>
		<div class=" justify-center items-center flex">
		<a  href="/projects" class=" hover:bg-gray-500  rounded-4xl p-3 " >Projekty</a> 
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/skills">Zručnosti</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/contact">Kontakt</a>
		</div>
	   </div>

	</section>

	<section class="hidden lg:flex">
	<div class="p-3 gabarito-uniquifier space-x-7 text-2xl ">
		<a class="hover:bg-gray-500  rounded-4xl p-3 " href="/">Domov</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/aboutme">O nás</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/websites">Stránky</a>
	
	
	</div>
	<div class="p-2" >	
		<Aperture class='size-10 stroke-2 text-black'/>
	</div>
	<div class="p-3 gabarito-uniquifier space-x-7 text-2xl">
		<a  href="/projects" class=" hover:bg-gray-500  rounded-4xl p-3 " >Projekty</a> 
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/skills">Zručnosti</a>
		<a class=" hover:bg-gray-500  rounded-4xl p-3 " href="/contact">Kontakt</a>
	</div>
	</section>

</header>


<main class="min-h-screen px-2 lg:px-6 mx-auto">
	{@render children()}
</main>


<footer>
	<Footer/>
</footer>



<style>
	@import url('https://fonts.googleapis.com/css2?family=Gabarito:wght@400..900&display=swap');
	:global(body) {
		background-color: rgba(255, 255, 255, 0.932);
	}
</style>




