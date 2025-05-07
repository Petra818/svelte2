<main class=" w-full">
	<h1 class="tulpen-one-regular p-20 text-center text-8xl">PROJEKTY</h1>
	<span class="block w-full"></span>

	<section class=" tomorrow-medium flex justify-center text-2xl">
		<article class=" tomorrow-medium"></article>
		<p>PLC PROJEKTY</p>
	</section>
<p class="text-white">x</p>

	<article class="">
		<div class=" tomorrow-regular flex flex-col lg:flex-row justify-between">
			<div class="w-full lg:w-4xl tomorrow-regular rounded-2xl border-2 text-xl">
				<p class=" text-center text-sm lg:text-xl">
					Vyvinuli sme PLC program, ktorý na základe signálu zo snímača automaticky spustí sirénu.
				</p>
				<p class=" tomorrow-medium lg:pt-15 lg:pl-5 text-sm pl-2 lg:text-xl"> Celý postup je implementovaný ako jednoduchý stavový stroj v PLC: </p>
				<div class="lg:pt-15 lg:pl-5 text-sm pl-2 lg:text-xl">
				<p>1. Stav „Čakanie" - sleduje prítomnosť vozíka na snímači.</p>
				<p>2. Stav „Časovač" - spustí interný odpočítavacímodul nastavený na 20 s.</p>
				<p>3. Stav „Alarm" - vygeneruje výstupný signál pre sirénu, aktivuje pulzné pípnutie a nastavíopakovací časovač na 60 s.</p>
				<p>4. Stav „Reset" - po potvrdení absencie vozíka obnoví výstupné relé do pokojovej polohy</p>
				<p>a vráti sa do stavu „Čakanie".</p>
				</div>
			</div>
         <p class="text-white">x</p>
			<img
				class=" w-100 h-100 rounded-2xl border"
				src="https://cloud-6.edupage.org/cloud?z%3AdxZt5ajkoF2pJSr7xkeUXBbANdreIHW6nLTtdIKOuoj3%2FSrgVAsZ41OGConOQBRpOtps8V7%2FENhKhQUXyz31jw%3D%3D"
				alt=""
			/>
			<p class="text-white">x</p>
			<img
				class="justify-center flex items-center lg:h-100 lg:w-80 rounded-2xl border"
				src="https://cloud-6.edupage.org/cloud?z%3AsjuxvnTDgMFpgiShMZGfOVwKNUjIWwOxYGrB5%2FkXw8ijODapg6kFVuk4q0x4p3Ck0pdUtMrh7ZLMbDMdEp91Qw%3D%3D"
				alt=""
			/>
			<p class="text-white">x</p>
			<p class="text-white">x</p>
       
     </div>
	    <p class="text-white">x</p>
		   <p class="text-white">x</p>
		<div class=" tomorrow-regular flex flex-col lg:flex-row justify-between">
			<div class="w-full lg:w-4xl rounded-2xl border-2 text-xl">
				<p class="text-center text-sm lg:text-xl">
					Zrealizovali sme funkčný systém signalizácie poruchy na báze PLC , ktorého účelom
				</p>
				<p class="text-center text-sm lg:text-xl">je upozorniť obsluhu na chýbajúcu fóliu prostredníctvom sirény.</p>
				<p class=" tomorrow-medium lg:pt-15 lg:pl-5 text-sm pl-2 lg:text-xl ">Popis funkcie sirény s PLC:</p>

				<div class=" lg:pl-5 text-sm pl-2 lg:text-xl">
					<p>1. Snímač detekuje fóliu neustále kontroluje prítomnosť fólie.</p>

					<p>2. Chýbajúca fólia spustí signál - pri absencii fólie odošle snímač signál do rozvádzača.</p>

					<p>3. Rozvádzač odosiela signál do PLC - PLC prijme vstupný signál o poruche.</p>

					<p>4. PLC aktivuje výstup ak je súčasne zopnuté tlačidlo, PLC pošle 24 V do sirény.</p>

					<p>5. Siréna sa spustí upozorňuje na chýbajúcu fóliu.</p>

					<p>6. Vypnutie sirény - obsluha stlačí tlačidlo, čím sa preruší obvod.</p>

					<p>7. Doplnenie fólie a reset po doplnení fólie sa tlačidlo opäť stlačí, obvod sa uzavrie a systém je pripravený na ďalšie spustenie pri novej poruche</p>
				</div>
			</div>
			<p class="text-white">x</p>
			<div class="lg:pr-1">
			<img
				class=" w-100 h-100 rounded-2xl border"
				src="https://cloud-8.edupage.org/cloud?z%3AlfvHYA1%2Fc1%2BkIDbDljSXHn3C0NXzNtf%2BSXpWPHyiZfbfNj%2FtnvgP9TQ3bKAIU6u7JsKhzJDKQcWGqJJutEkbng%3D%3D"
				alt=""/>
				</div>
			<p class="text-white">x</p>
			<div class="lg:pr-21">
			<img
				class="justify-center flex items-center lg:h-100 lg:w-80 rounded-2xl border "
				src="https://cloud-f.edupage.org/cloud?z%3ARi4sHBpfBw%2F6IkhjBBEt6EuOte2S8Xmx%2FWhwVlDWmr85iqF9wRrgeLUl1vcjUIqSkMV5lV%2FIza7S5cZr2hJUnA%3D%3D"
				alt=""/>
			</div>
		</div>
	</article>
</main>
