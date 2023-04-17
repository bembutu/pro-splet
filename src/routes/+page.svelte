<script lang="ts">
    import { Splide, SplideSlide } from '@splidejs/svelte-splide';
    import '@splidejs/svelte-splide/css'; 
</script>

<!-- Hero section -->
<div class="flex bg-[url('page-header-bg-filter.jpg')] bg-center bg-cover bg-no-repeat items-center justify-center">
    <h1 class="text-4xl md:text-5xl text- text-gray-100 pt-64 pb-44 pl-10 pr-10 text-center">Želite kvalitetno spletno mesto?</h1>
</div>

<!-- Cards section  -->
<div class="p-10 bg-[url('cards/odzadje.png')] bg-center bg-cover bg-no-repeat">

    <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 items-center justify-center align-middle">
    
    <a href="/storitve/optimizacija-spletnega-mesta" class="flex flex-col p-4 m-4 bg-white border-oker transform scale-100 hover:scale-110 transition duration-400 ease-out">
        <div class="flex items-center justify-between w-full">            
            <span class="font-bold text-2xl text-gray-300 p-4 mr-2 pl-8">01</span>
            <img src="/cards/seooptimizacija.png" alt="Optimizacija spletnega mesta" class="w-14 h-14 transform scale-100 hover:scale-75 transition duration-500 ease-out" />
        </div>

        <div class="w-full p-4">
          <h2 class="text-lg blue-color hover-text text-center font-bold">OPTIMIZACIJA SPLETNEGA MESTA</h2>
          <p class="text-gray-700 text-center hover-text text-base">Višje uvrščena spletna mesta</p>
        </div>
    </a>

    <a href="/storitve/izdelava-mobilnih-in-spletnih-aplikacij" class="flex flex-col p-4 m-4 bg-white border-oker transform scale-100 hover:scale-110 transition duration-400 ease-out">
        <div class="flex items-center justify-between w-full">            
            <span class="font-bold text-2xl text-gray-300 p-4 mr-2 pl-8">02</span>
            <img src="/cards/seooptimizacija.png" alt="Optimizacija spletnega mesta" class="w-14 h-14 transform scale-100 hover:scale-75 transition duration-500 ease-out" />
        </div>

        <div class="w-full p-4">
          <h2 class="text-lg blue-color hover-text text-center font-bold">IZDELAVA MOBILNIH IN SPLETNIH APLIKACIJ</h2>
          <p class="text-gray-700 text-center hover-text text-base">Inovativne rešitve za vaše stranke</p>
        </div>
    </a>

    <a href="/storitve/spletna-analitika" class="flex flex-col p-4 m-4 bg-white border-oker transform scale-100 hover:scale-110 transition duration-400 ease-out">
        <div class="flex items-center justify-between w-full">            
            <span class="font-bold text-2xl text-gray-300 p-4 mr-2 pl-8">03</span>
            <img src="/cards/seooptimizacija.png" alt="Optimizacija spletnega mesta" class="w-14 h-14 transform scale-100 hover:scale-75 transition duration-500 ease-out" />
        </div>

        <div class="w-full p-4">
          <h2 class="text-lg blue-color hover-text text-center font-bold">SPLETNA ANALITIKA</h2>
          <p class="text-gray-700 text-center hover-text text-base">Dovolite si zunanji vpogled na Vaše podjetje</p>
        </div>
    </a>

    <a href="/storitve/placljivo-oglasevanje" class="flex flex-col p-4 m-4 bg-white border-oker transform scale-100 hover:scale-110 transition duration-400 ease-out">
        <div class="flex items-center justify-between w-full">            
            <span class="font-bold text-2xl text-gray-300 p-4 mr-2 pl-8">04</span>
            <img src="/cards/seooptimizacija.png" alt="Optimizacija spletnega mesta" class="w-14 h-14 transform scale-100 hover:scale-75 transition duration-500 ease-out" />
        </div>

        <div class="w-full p-4">
          <h2 class="text-lg blue-color hover-text text-center font-bold">PLAČLJIVO OGLAŠEVANJE</h2>
          <p class="text-gray-700 text-center hover-text text-base">Vlagajte v rast vašega podjetja</p>
        </div>
    </a>

    <a href="/storitve/izdelava-spletnih-trgovin" class="flex flex-col p-4 m-4 bg-white border-oker transform scale-100 hover:scale-110 transition duration-400 ease-out">
        <div class="flex items-center justify-between w-full">            
            <span class="font-bold text-2xl text-gray-300 p-4 mr-2 pl-8">05</span>
            <img src="/cards/seooptimizacija.png" alt="Optimizacija spletnega mesta" class="w-14 h-14 transform scale-100 hover:scale-75 transition duration-500 ease-out" />
        </div>

        <div class="w-full p-4">
          <h2 class="text-lg blue-color hover-text text-center font-bold">IZDELAVA SPLETNIH TRGOVIN</h2>
          <p class="text-gray-700 text-center hover-text text-base">Vlagajte v rast vašega podjetja</p>
        </div>
    </a>

</div>

</div>


<!-- Reference carousel --> 

<div class="flex flex-col mx-auto max-w-7xl justify-center items-center m-8">

    <h1 class="p-4 text-2xl blue-color"><b>NAŠE ZADOVOLJNE STRANKE</b></h1>
    
      <Splide aria-label="reference-images">        
        <SplideSlide>
          <a href="https://www.example.com" target="_blank">  
            <h2 class="text-center p-2 text-lg">Prva referenca</h2>
            <img src="/page-header-bg.jpg" alt="page header"/>
          </a>
        </SplideSlide>
        

        <SplideSlide>
            <a href="https://www.example.com" target="_blank">  
                <h2 class="text-center p-2 text-lg">Druga referenca</h2>
                <img src="/page-header-bg.jpg" alt="page header"/>
            </a>
        </SplideSlide>
      </Splide>
   
  </div>
  
  


