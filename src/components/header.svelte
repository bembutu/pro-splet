<script>
// @ts-nocheck

  
    let navOpen = false;
    
    function handleNav() {
      navOpen = !navOpen;  
    }

    let subMenuOpen = false; 
  
  </script>


<header class="fixed top-0 w-full h-28 flex header-bg z-50 flex-auto">

  <div class="w-full mx-auto justify-between py-4 px-4 sm:px-6 lg:px-8 flex items-center">

    <!-- Left column - logo -->
    <div class="flex-shrink-0 w-auto ml-4">
      <a href="/">
      <img class="h-9" src="/prosplet-logo-white.png" alt="Logo">
    </a>
    </div>

    <!-- Middle column - navigation menu -->
    <nav class="hidden items-center justify-center md:flex">

      <a href="/" class="text-gray-100 px-3 py-2 text-base font-medium hover-text">DOMOV</a>
      <a href="/o-nas" class="text-gray-100 min-w-fit px-3 py-2 text-base font-medium hover-text">O NAS</a>
      
      <div class="relative inline-block group mx-auto">
        <button class="text-gray-100 px-3 py-2 text-base font-medium hover-text focus:outline-none" aria-haspopup="true" aria-expanded="false">
          STORITVE
        </button>
        <div class="absolute z-10 bg-white shadow-lg mt-9 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-1000 origin-top w-85">
          <a href="/storitve/optimizacija-spletnega-mesta" class="block px-4 py-2 text-blue-950 font-medium dropdown-bg hover:text-white">OPTIMIZACIJA SPLETNEGA MESTA</a>
          <a href="/storitve/izdelava-mobilnih-in-spletnih-aplikacij" class="block px-4 py-2 text-blue-950 font-medium dropdown-bg hover:text-white">IZDELAVA MOBILNIH IN SPLETNIH APLIKACIJ</a>
          <a href="/storitve/spletna-analitika" class="block px-4 py-2 text-blue-950 font-medium dropdown-bg hover:text-white">SPLETNA ANALITIKA</a>
          <a href="/storitve/placljivo-oglasevanje" class="block px-4 py-2 text-blue-950 font-medium dropdown-bg hover:text-white">PLAČLJIVO OGLAŠEVANJE</a>
          <a href="/storitve/izdelava-spletnih-trgovin" class="block px-4 py-2 text-blue-950 font-medium dropdown-bg hover:text-white">IZDELAVA SPLETNIH TRGOVIN</a>
        </div>
      </div>      

      <a href="/reference" class="text-gray-100 px-3 py-2 text-base font-medium hover-text">REFERENCE</a>
      <a href="/kontakt" class="text-gray-100 px-3 py-2 text-base font-medium hover-text">KONTAKT</a>

      <div class="relative min-w-fit inline-block group">
        <button class="text-gray-100 block px-3 py-2 text-base font-medium focus:outline-none" aria-haspopup="true" aria-expanded="false">
          <img src="slo-flag.png" alt="slovensko" class="mr-1 h-4 w-4 inline-block">
          <div class="inline-block hover-text">SLO</div>
        </button>
        <div class="absolute z-10 bg-white shadow-lg mt-9 opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all duration-1000 origin-top w-24">
          <a href="/" class="block px-4 py-2 text-blue-950 font-medium dropdown-bg hover:text-white">
            <img src="eng-flag.png" alt="english" class="mr-1 h-4 w-4 inline-block">
            ENG</a>
        </div>
      </div>

    </nav>

    <!-- Right column - contact -->
    <div class="hidden md:flex md:items-center md:justify-center">
      
      <div class="flex items-center">
        <img class="h-6 w-6 flex-row text-gray-100" src="/phone-icon.png" alt="Phone icon"/>
        <a href="tel:+38641833683" class="ml-2 text-gray-100 hover-text font-medium">+ (386) 41-833-683</a>
      </div>      

    </div>

    <!-- Right column - hamburger mobile menu -->
    <div class="flex items-center md:hidden">
      <button class="p-2 oker-color hover:text-white focus:outline-none transition-all duration-700" type="button" on:click={handleNav}>
        <svg class="h-8 w-8 fill-current" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M4 6h16v2H4zm0 5h16v2H4zm0 5h16v2H4z"/></svg>
      </button>
    </div>

  </div>
</header>

<!-- Side navigation menu -->
<!-- Side navigation menu -->
<div class="fixed top-0 left-0 h-full w-72 z-20 transition duration-700 ease-in-out transform" class:translate-x-0={navOpen} class:-translate-x-full={!navOpen}>
  <div class="sidenav-bg absolute inset-0"></div> <!-- sidenav background -->
  <div class="flex justify-between items-center px-4 py-3 mt-24 relative z-30"> <!-- sidenav content -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <nav class="px-2 py-4 w-full" on:click|stopPropagation={(e) => {if (!e.target.matches('.sub-menu-button')) handleNav();}}>
      <a href="/" class="block py-2 text-white hover-text border-t border-gray-500">Domov</a>
      <a href="/o-nas" class="block py-2 text-white hover-text border-t border-b border-gray-500">O nas</a>
      <div class="relative">
        <div class="flex items-center justify-between py-2">
          <a href="/storitve" class="block py-2 text-white hover-text">Storitve</a>
          <button class="sub-menu-button oker-color ml-8" on:click={() => subMenuOpen = !subMenuOpen}>
            {#if subMenuOpen} &#9650; {:else} &#9660; {/if}
          </button>
        </div>
        {#if subMenuOpen}
          <div class="pl-3">
            <a href="/storitve/optimizacija-spletnega-mesta" class="block py-2 text-white hover-text border-t border-gray-500">Optimizacija spletnega mesta</a>
            <a href="/storitve/izdelava-mobilnih-in-spletnih-aplikacij" class="block py-2 text-white hover-text border-t border-gray-500">Izdelava mobilnih in spletnih aplikacij</a>
            <a href="/storitve/spletna-analitika" class="block py-2 text-white hover-text border-t border-gray-500">Spletna analitika</a>
            <a href="/storitve/placljivo-oglasevanje" class="block py-2 text-white hover-text border-t border-gray-500">Plačljivo oglaševanje</a>
            <a href="/storitve/izdelava-spletnih-trgovin" class="block py-2 text-white hover-text border-t border-gray-500">Izdelava spletnih trgovin</a>
          </div>
        {/if}
      </div>
      <a href="/reference" class="block py-2 text-white hover-text border-t border-gray-500">Reference</a>
      <a href="/kontakt" class="block py-2 text-white hover-text border-t border-b border-gray-500">Kontakt</a>
    </nav>
  </div>
</div>



{#if navOpen}
  <!-- svelte-ignore a11y-click-events-have-key-events -->
  <div class="fixed top-0 left-0 h-screen w-screen bg-gray-500 bg-opacity-50 z-10" on:click={handleNav}></div>
{/if}

