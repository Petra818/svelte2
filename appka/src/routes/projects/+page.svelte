<main class=" h-screen ">
	
	
	<h1 class="tulpen-one-regular p-20 text-center text-8xl">PROJEKTY</h1>
	<span class="block w-full "></span>
	<section class=" justify-center flex tomorrow-medium text-2xl">
	<article class=" tomorrow-medium  ">
		</article>
		<p>PLC PROJEKTY</p>
		
		
</section> 
<div class="justify-between flex p-30 tomorrow-regular">
	<div class="border-2 w-4xl h-100 rounded-2xl text-xl tomorrow-regular">
<p class="text-center pt-3  ">Vyvinuli sme PLC program, ktorý na základe signálu zo snímača automaticky spustí sirénu. </p>
<p class="pl-6.5 tomorrow-medium pt-30">Celý postup je implementovaný ako jednoduchý stavový stroj v PLC:</p>
<div class="pl-6.5">
<p class="pt-5">1. Stav „Čakanie" - sleduje prítomnosť vozíka na snímači.</p>
<p>2. Stav „Časovač" - spustí interný odpočítavacímodul nastavený na 20 s.</p>	
<p>3. Stav „Alarm" - vygeneruje výstupný signál pre sirénu, aktivuje pulzné pípnutie a nastavíopakovací časovač na 60 s.</p>
<p>4. Stav „Reset" - po potvrdení absencie vozíka obnoví výstupné relé do pokojovej polohy</p>
<p>a vráti sa do stavu „Čakanie".</p>
</div></div>


<img class=" border rounded-2xl w-100 h-100" src="https://cloud-6.edupage.org/cloud?z%3AdxZt5ajkoF2pJSr7xkeUXBbANdreIHW6nLTtdIKOuoj3%2FSrgVAsZ41OGConOQBRpOtps8V7%2FENhKhQUXyz31jw%3D%3D" alt="">
<img class=" border rounded-2xl w-80 h-100" src="https://cloud-6.edupage.org/cloud?z%3AsjuxvnTDgMFpgiShMZGfOVwKNUjIWwOxYGrB5%2FkXw8ijODapg6kFVuk4q0x4p3Ck0pdUtMrh7ZLMbDMdEp91Qw%3D%3D" alt="">

</div>
<div class="justify-between flex p-30 tomorrow-regular ">
<div class="border-2 w-4xl h-100 rounded-2xl text-xl">
<p class="pl-6.5 pt-3">Zrealizovali sme funkčný systém signalizácie poruchy na báze PLC , ktorého účelom </p>
<p class="pl-6.5">je upozorniť obsluhu na chýbajúcu fóliu prostredníctvom sirény.</p>
<p class="pl-6.5 pt-12 tomorrow-medium	">Popis funkcie sirény s PLC:</p>

<div class="pt-4 pl-6.5">
	<p>1. Snímač detekuje fóliu neustále kontroluje prítomnosť fólie.</p>

<p>2. Chýbajúca fólia spustí signál - pri absencii fólie odošle snímač signál do rozvádzača.</p>

<p>3. Rozvádzač odosiela signál do PLC - PLC prijme vstupný signál o poruche.</p>

<p>4. PLC aktivuje výstup ak je súčasne zopnuté tlačidlo, PLC pošle 24 V do sirény.</p>

<p>5. Siréna sa spustí upozorňuje na chýbajúcu fóliu.</p>

<p>6. Vypnutie sirény - obsluha stlačí tlačidlo, čím sa preruší obvod.</p>

<p>7. Doplnenie fólie a reset po doplnení fólie sa tlačidlo opäť stlačí, obvod sa uzavrie a systém je pripravený na ďalšie spustenie pri novej poruche</p>
</div>




</div>
<img class=" border rounded-2xl w-100 h-100" src="https://cloud-8.edupage.org/cloud?z%3AlfvHYA1%2Fc1%2BkIDbDljSXHn3C0NXzNtf%2BSXpWPHyiZfbfNj%2FtnvgP9TQ3bKAIU6u7JsKhzJDKQcWGqJJutEkbng%3D%3D" alt="">
<img class=" border rounded-2xl w-80 h-100" src="https://cloud-f.edupage.org/cloud?z%3ARi4sHBpfBw%2F6IkhjBBEt6EuOte2S8Xmx%2FWhwVlDWmr85iqF9wRrgeLUl1vcjUIqSkMV5lV%2FIza7S5cZr2hJUnA%3D%3D" alt="">



</div>
</main>



<section>
	<!-- <img src="https://cloud-6.edupage.org/cloud?z%3AZRh4KnvTP8SO%2FA%2B%2F2R8pI7Jr07XCZlS1%2BRDffEGV4gOOlmdhdUfv0%2FTlXpgYBjUfP7JTcA1FVVRp2Zz7R1OM3w%3D%3D" alt="popis"/> -->

	
</section>

<style>
@import url('https://fonts.googleapis.com/css2?family=Tulpen+One&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Tomorrow:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Tulpen+One&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Tomorrow:wght@500&display=swap');


</style>
  