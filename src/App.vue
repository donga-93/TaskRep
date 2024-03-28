<script >

import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'
// initialize components based on data attribute selectors
onMounted(() => {
    initFlowbite();
})

 // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  import 'swiper/css/navigation';
  import 'swiper/css/pagination';



  // import required modules
  import { Navigation, Pagination, Mousewheel, Keyboard } from 'swiper/modules';

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [Navigation, Pagination, Mousewheel, Keyboard],
      };
    },
  };


</script>

<template>
<nav class="bg-white border-gray-200 dark:bg-gray-900">
  <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
  <a href="https://flowbite.com/" class="flex items-center space-x-3 rtl:space-x-reverse">
      <img src="https://cdn.icon-icons.com/icons2/2429/PNG/512/basecamp_logo_icon_147315.png" class="h-8" alt="Flowbite Logo" />
      <span class="self-center text-2xl font-semibold whitespace-nowrap dark:text-white">Basecamp</span>
  </a>

  <div class="flex md:order-2">
    <button type="button" data-collapse-toggle="navbar-search" aria-controls="navbar-search" aria-expanded="false" class="md:hidden text-gray-500 dark:text-gray-400 hover:bg-gray-100 dark:hover:bg-gray-700 focus:outline-none focus:ring-4 focus:ring-gray-200 dark:focus:ring-gray-700 rounded-lg text-sm p-2.5 me-1">
      <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
        <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"/>
      </svg>
      <span class="sr-only">Search</span>
    </button>
    <div class="relative hidden md:block">
      <div class="absolute inset-y-0 start-0 flex items-center ps-3 pointer-events-none">
        <svg class="w-4 h-4 text-gray-500 dark:text-gray-400" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
          <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"/>
        </svg>
        <span class="sr-only">Search icon</span>
      </div>
      <input type="text" id="search-navbar" class="block w-full p-2 ps-9 text-sm text-gray-900 border border-gray-300 rounded-lg bg-gray-50 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="ძიება">
    </div>
    <button data-collapse-toggle="navbar-search" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-search" aria-expanded="false">
        <span class="sr-only">Open main menu</span>
        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
        </svg>
    </button>
  </div>
    <div class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1" id="navbar-search">
      <div class="relative mt-3 md:hidden">
        <div class="absolute inset-y-0 start-0 flex items-center ps-3 pointer-events-none">
          <svg class="w-4 h-4 text-gray-500 dark:text-gray-400" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"/>
          </svg>
        </div>
        <input type="text" id="search-navbar" class="block w-full p-2 ps-10 text-sm text-gray-900 border border-gray-300 rounded-lg bg-gray-50 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:ring-blue-500 dark:focus:border-blue-500" placeholder="Search...">
      </div>
      <ul class="flex flex-col p-4 md:p-0 mt-4 font-medium border border-gray-100 rounded-lg bg-gray-50 md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0 md:border-0 md:bg-white dark:bg-gray-800 md:dark:bg-gray-900 dark:border-gray-700">
        <li>
          <a href="#" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">პოლიტიკა</a>
        </li>
        <li>
          <a href="#" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">საზოგადოება</a>
        </li>
        <li>
          <a href="#" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 dark:text-white md:dark:hover:text-blue-500 dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">სამართალი</a>
        </li>
        <li id="business">
          <a href="#" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">ბიზნესი & ეკონომიკა</a>
        </li>
        <li id="business2">
          <a href="#" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">ეკონომიკა</a>
        </li>
        <li id="business3">
          <a href="#" class="block py-2 px-3 text-gray-900 rounded hover:bg-gray-100 md:hover:bg-transparent md:hover:text-blue-700 md:p-0 md:dark:hover:text-blue-500 dark:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">რელიგია</a>
        </li>
        <li>
            <button id="dropdownHoverButton" data-dropdown-toggle="dropdownHover" data-dropdown-trigger="hover" class="text-black focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-4.5 text-center inline-flex items-center   dark:focus:ring-blue-800" type="button">სხვა<svg class="w-2.5 h-2.5 ms-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 10 6">
            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 4 4 4-4"/>
            </svg>
          </button>
          <!-- Dropdown menu -->
            <div id="dropdownHover" class="z-10 hidden bg-white divide-y divide-gray-100 rounded-lg shadow w-44 dark:bg-gray-700">
                <ul class="py-2 text-sm text-gray-700 dark:text-gray-200" aria-labelledby="dropdownHoverButton">
                  <li>
                    <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">ბიზნესი & ეკონომიკა</a>
                  </li>
                  <li>
                    <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">ეკონომიკა</a>
                  </li>
                  <li>
                    <a href="#" class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">რელიგია</a>
                  </li>
               </ul>
            </div>
         </li>
      </ul>
    </div>
  </div>
</nav>

<div>
 <swiper
:pagination="pagination" :modules="modules"
    class="mySwiper"
  >
    <swiper-slide>
     <img
     src="https://s3-alpha-sig.figma.com/img/0f26/9f24/bc698191aa69589fa1db7e13b2222fee?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=kuzec67favVR8~sPbz5r6J6Gx3jAobONP4dJMYchnjDy5vy2ltl5wUqPiWMbJQSSRHf17qNYo240GBIeidFNv5QhUm2d0epjYOD6MDa4UTlVYyxfrL~mG6M6s5gPKwqA0bBouUxadurf36N3Cg0rQZKrN7zqk57XAgpLWCjOuf7oCOBm9jfp47q4khQZ0DnG0mNojMrLESFVXNtOmrauSIvZeSmiZszy2aVl-dGpevb50aXDrWA1QFzIAJhPgtaBbeFqnWRQbjCvn7BGweXpzdbHFQbVG6CL-FIHYTxObYE0dpO12pqHiRYkksItVXsDXyv1P2L5grhIROWUGwSyYQ__" />
     </swiper-slide>
    <swiper-slide>Slide 4</swiper-slide><swiper-slide>Slide 5</swiper-slide>
    <swiper-slide>Slide 6</swiper-slide><swiper-slide>Slide 7</swiper-slide>
    <swiper-slide>Slide 8</swiper-slide><swiper-slide>Slide 9</swiper-slide>
    </swiper>
</div>
    
<div id="info">
<p class="text-lg font-normal text-gray-500 lg:text-xl dark:text-gray-400">12.08.2023  პოლიტიკა</p>
<h1 class="mb-4 text-4xl font-normal leading-none tracking-tight text-gray-900 md:text-2xl  dark:text-white">ქვემო ქართლის რეგიონში 20 მლნ ლარამდე ღირებულების <br /> ინფრასტრუქტურული პროექტები დაიწყება</h1>
<p class="text-lg font-normal text-gray-500 lg:text-xl dark:text-gray-400">განთავსების (ლისტინგის) ორგანიზატორი სომხეთის ბანკი 1000 USD</p>
<br>
<br>
<p class="text-lg font-normal text-gray-500 lg:text-xl dark:text-gray-400">ცნობილი ფაქტები</p>
</div>


<div id="posts">
<ol class="relative border-s border-gray-200 dark:border-gray-700">                  
    <li class="mb-10 ms-6">            
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -start-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue-900">
            <svg class="w-2.5 h-2.5 text-blue-800 dark:text-blue-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 20">
                <path d="M20 4a2 2 0 0 0-2-2h-2V1a1 1 0 0 0-2 0v1h-3V1a1 1 0 0 0-2 0v1H6V1a1 1 0 0 0-2 0v1H2a2 2 0 0 0-2 2v2h20V4ZM0 18a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V8H0v10Zm5-8h10a1 1 0 0 1 0 2H5a1 1 0 0 1 0-2Z"/>
            </svg>
        </span>
        <h3 class="flex items-center mb-1 text-lg font-semibold text-gray-900 dark:text-white">პოპულარული</h3>
        <time class="block mb-2 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Released on January 13th, 2022</time>
    </li>
    <li class="mb-10 ms-6">
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -start-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue-900">
            <svg class="w-2.5 h-2.5 text-blue-800 dark:text-blue-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 20">
                <path d="M20 4a2 2 0 0 0-2-2h-2V1a1 1 0 0 0-2 0v1h-3V1a1 1 0 0 0-2 0v1H6V1a1 1 0 0 0-2 0v1H2a2 2 0 0 0-2 2v2h20V4ZM0 18a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V8H0v10Zm5-8h10a1 1 0 0 1 0 2H5a1 1 0 0 1 0-2Z"/>
            </svg>
        </span>
        <h3 class="mb-1 text-lg font-semibold text-gray-900 dark:text-white"> დღეიდან ასაწონად განკუთვნილი 
პოლიეთილენის პარკები აიკრძალა
</h3>
        <time class="block mb-2 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Released on December 7th, 2021</time>
        <p class="text-base font-normal text-gray-500 dark:text-gray-400">All of the pages and components are first designed in Figma and we keep a parity between the two versions even as we update the project.</p>
    </li>
    <li class="ms-6">
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -start-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue-900">
            <svg class="w-2.5 h-2.5 text-blue-800 dark:text-blue-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 20">
                <path d="M20 4a2 2 0 0 0-2-2h-2V1a1 1 0 0 0-2 0v1h-3V1a1 1 0 0 0-2 0v1H6V1a1 1 0 0 0-2 0v1H2a2 2 0 0 0-2 2v2h20V4ZM0 18a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V8H0v10Zm5-8h10a1 1 0 0 1 0 2H5a1 1 0 0 1 0-2Z"/>
            </svg>
        </span>
        <h3 class="mb-1 text-lg font-semibold text-gray-900 dark:text-white">დღეიდან ასაწონად განკუთვნილი 
პოლიეთილენის პარკები აიკრძალა</h3>
        <time class="block mb-2 text-sm font-normal leading-none text-gray-400 dark:text-gray-500">Released on December 2nd, 2021</time>
        <p class="text-base font-normal text-gray-500 dark:text-gray-400">Get started with dozens of web components and interactive elements built on top of Tailwind CSS.</p>
    </li>
</ol>
</div>


<div id="posts2">
<ol class="relative border-s border-gray-200 dark:border-gray-700">                  
    <li class="mb-10 ms-6">            
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -start-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue-900">
            <svg class="w-2.5 h-2.5 text-blue-800 dark:text-blue-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 20">
                <path d="M20 4a2 2 0 0 0-2-2h-2V1a1 1 0 0 0-2 0v1h-3V1a1 1 0 0 0-2 0v1H6V1a1 1 0 0 0-2 0v1H2a2 2 0 0 0-2 2v2h20V4ZM0 18a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V8H0v10Zm5-8h10a1 1 0 0 1 0 2H5a1 1 0 0 1 0-2Z"/>
            </svg>
        </span>
        <h3 class="flex items-center mb-1 text-lg font-semibold text-gray-900 dark:text-white">პოპულარული</h3>
       <img src="https://s3-alpha-sig.figma.com/img/c051/1868/4e3e239294cad45b2c93c031270a47f0?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=i~RugVuVImcdfbqvPSprhYTDv9uy~CCDjoy1R0ahqFELTIQIqt4lmMCX9g2mfM-hxvPPXE6BQ2w~TALxZbmyZXN8eb6z5BjWI1DONDYXX~rzdQsfV-k8CQRw~Q62YNRMcg19N9z1rE7z~QnnquuVrpzQdFYFqVRiFyisZ-ryreBn9ne0GR9-DtSuWmtkWg7OtQ5Jvmy1DmZTxQetatZh734JZbqVoEx4TRYfTD5oU7zkoNBAIih00~oHQSX0dmzxcAAnyJuclVmL-Cs-op-vFDotfvxgrirtVne4MJsrVt8dF1XJCum6rcGglNRnYcU-ObWPl7rr4e-hAcnGrKjJ0g__" alt="Paris" style="width:150px">
    </li>
    <li class="mb-10 ms-6">
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -start-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue-900">
            <svg class="w-2.5 h-2.5 text-blue-800 dark:text-blue-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 20">
                <path d="M20 4a2 2 0 0 0-2-2h-2V1a1 1 0 0 0-2 0v1h-3V1a1 1 0 0 0-2 0v1H6V1a1 1 0 0 0-2 0v1H2a2 2 0 0 0-2 2v2h20V4ZM0 18a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V8H0v10Zm5-8h10a1 1 0 0 1 0 2H5a1 1 0 0 1 0-2Z"/>
            </svg>
        </span>
        <h3 class="mb-1 text-lg font-semibold text-gray-900 dark:text-white">დღეიდან ასაწონად განკუთვნილი 
პოლიეთილენის პარკები აიკრძალა
</h3>
        <img src="https://s3-alpha-sig.figma.com/img/c051/1868/4e3e239294cad45b2c93c031270a47f0?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=i~RugVuVImcdfbqvPSprhYTDv9uy~CCDjoy1R0ahqFELTIQIqt4lmMCX9g2mfM-hxvPPXE6BQ2w~TALxZbmyZXN8eb6z5BjWI1DONDYXX~rzdQsfV-k8CQRw~Q62YNRMcg19N9z1rE7z~QnnquuVrpzQdFYFqVRiFyisZ-ryreBn9ne0GR9-DtSuWmtkWg7OtQ5Jvmy1DmZTxQetatZh734JZbqVoEx4TRYfTD5oU7zkoNBAIih00~oHQSX0dmzxcAAnyJuclVmL-Cs-op-vFDotfvxgrirtVne4MJsrVt8dF1XJCum6rcGglNRnYcU-ObWPl7rr4e-hAcnGrKjJ0g__" alt="Paris" style="width:150px">
        <p class="text-base font-normal text-gray-500 dark:text-gray-400">All of the pages and components are first designed in Figma and we keep a parity between the two versions even as we update the project.</p>
    </li>
    <li class="ms-6">
        <span class="absolute flex items-center justify-center w-6 h-6 bg-blue-100 rounded-full -start-3 ring-8 ring-white dark:ring-gray-900 dark:bg-blue-900">
            <svg class="w-2.5 h-2.5 text-blue-800 dark:text-blue-300" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 20">
                <path d="M20 4a2 2 0 0 0-2-2h-2V1a1 1 0 0 0-2 0v1h-3V1a1 1 0 0 0-2 0v1H6V1a1 1 0 0 0-2 0v1H2a2 2 0 0 0-2 2v2h20V4ZM0 18a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V8H0v10Zm5-8h10a1 1 0 0 1 0 2H5a1 1 0 0 1 0-2Z"/>
            </svg>
        </span>
        <h3 class="mb-1 text-lg font-semibold text-gray-900 dark:text-white">დღეიდან ასაწონად განკუთვნილი 
პოლიეთილენის პარკები აიკრძალა</h3>
        <img src="https://s3-alpha-sig.figma.com/img/c051/1868/4e3e239294cad45b2c93c031270a47f0?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=i~RugVuVImcdfbqvPSprhYTDv9uy~CCDjoy1R0ahqFELTIQIqt4lmMCX9g2mfM-hxvPPXE6BQ2w~TALxZbmyZXN8eb6z5BjWI1DONDYXX~rzdQsfV-k8CQRw~Q62YNRMcg19N9z1rE7z~QnnquuVrpzQdFYFqVRiFyisZ-ryreBn9ne0GR9-DtSuWmtkWg7OtQ5Jvmy1DmZTxQetatZh734JZbqVoEx4TRYfTD5oU7zkoNBAIih00~oHQSX0dmzxcAAnyJuclVmL-Cs-op-vFDotfvxgrirtVne4MJsrVt8dF1XJCum6rcGglNRnYcU-ObWPl7rr4e-hAcnGrKjJ0g__" alt="Paris" style="width:150px">
        <p class="text-base font-normal text-gray-500 dark:text-gray-400">Get started with dozens of web components and interactive elements built on top of Tailwind CSS.</p>
    </li>
</ol>
</div>




 <swiper
    :slidesPerView="2"
    :centeredSlides="true"
    :spaceBetween="-750"
    :grabCursor="true"
    :pagination="{
      clickable: true,
    }"
    :modules="modules"
    class="mySwiper2"
  >
    <swiper-slide
    style="width: 188px;"
    >
  <div class="gallery">
    <a target="_blank" href="img_5terre.jpg">
    <img
    style="width: 288px; height: 120px;"
     src="https://s3-alpha-sig.figma.com/img/24b0/6366/2a63eb933a283ca80f4847a0a25fcbf1?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=W~oncfdnASzHMYdoanoiqhGRL3br0EgHQYQipq3Df-SnPeXZrub3cllOYdn5e1qP8KlGc8PWspCncYXxxZIKCWZ9zix~hn1E7nvksw6~U-jTJvZZ5FUkJP2Y8jLTaifOz7vu6YwPCy6AZFHmVIgrMe7bQW0BqYinrWeyJ0WaJwZQ-7p0YrK1f4OZfTp~Cr4EKbhcA1Pg~s~tm05DZqG4PI1PR6HF4Bg6FyRhMS4TXMZuYLEcwR159MciY-zdpBFRU5dCCMWp~uZPSNxg9897TfgRqAXjReHrRXp56UCxanhaX13QsfBAQ9puhL33hrB5Nu1tuUuyw-AaLDpT9c9lhQ_" alt="Cinque Terre" width="600" height="400">
     </a>
     <br> 
    <div class="desc">ქვემო ქართლის რეგიონში 20 მლნ <br> ლარამდე ღირებულების </div>
  </div>
     </swiper-slide>
    <swiper-slide>     
     <img
     style="width: 288px; height: 120px;"
     src="https://s3-alpha-sig.figma.com/img/24b0/6366/2a63eb933a283ca80f4847a0a25fcbf1?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=W~oncfdnASzHMYdoanoiqhGRL3br0EgHQYQipq3Df-SnPeXZrub3cllOYdn5e1qP8KlGc8PWspCncYXxxZIKCWZ9zix~hn1E7nvksw6~U-jTJvZZ5FUkJP2Y8jLTaifOz7vu6YwPCy6AZFHmVIgrMe7bQW0BqYinrWeyJ0WaJwZQ-7p0YrK1f4OZfTp~Cr4EKbhcA1Pg~s~tm05DZqG4PI1PR6HF4Bg6FyRhMS4TXMZuYLEcwR159MciY-zdpBFRU5dCCMWp~uZPSNxg9897TfgRqAXjReHrRXp56UCxanhaX13QsfBAQ9puhL33hrB5Nu1tuUuyw-AaLDpT9c9lhQ__" 
     />
     </swiper-slide>
    <swiper-slide>     
    <img
     style="width: 288px; height: 120px;"
     src="https://s3-alpha-sig.figma.com/img/24b0/6366/2a63eb933a283ca80f4847a0a25fcbf1?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=W~oncfdnASzHMYdoanoiqhGRL3br0EgHQYQipq3Df-SnPeXZrub3cllOYdn5e1qP8KlGc8PWspCncYXxxZIKCWZ9zix~hn1E7nvksw6~U-jTJvZZ5FUkJP2Y8jLTaifOz7vu6YwPCy6AZFHmVIgrMe7bQW0BqYinrWeyJ0WaJwZQ-7p0YrK1f4OZfTp~Cr4EKbhcA1Pg~s~tm05DZqG4PI1PR6HF4Bg6FyRhMS4TXMZuYLEcwR159MciY-zdpBFRU5dCCMWp~uZPSNxg9897TfgRqAXjReHrRXp56UCxanhaX13QsfBAQ9puhL33hrB5Nu1tuUuyw-AaLDpT9c9lhQ__" 
     />
     </swiper-slide>

    <swiper-slide>
    <img
         style="width: 288px; height: 120px;"
     src="https://s3-alpha-sig.figma.com/img/24b0/6366/2a63eb933a283ca80f4847a0a25fcbf1?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=W~oncfdnASzHMYdoanoiqhGRL3br0EgHQYQipq3Df-SnPeXZrub3cllOYdn5e1qP8KlGc8PWspCncYXxxZIKCWZ9zix~hn1E7nvksw6~U-jTJvZZ5FUkJP2Y8jLTaifOz7vu6YwPCy6AZFHmVIgrMe7bQW0BqYinrWeyJ0WaJwZQ-7p0YrK1f4OZfTp~Cr4EKbhcA1Pg~s~tm05DZqG4PI1PR6HF4Bg6FyRhMS4TXMZuYLEcwR159MciY-zdpBFRU5dCCMWp~uZPSNxg9897TfgRqAXjReHrRXp56UCxanhaX13QsfBAQ9puhL33hrB5Nu1tuUuyw-AaLDpT9c9lhQ__" 
     />
          </swiper-slide>
    <swiper-slide> 
    <img
         style="width: 288px; height: 120px;"
     src="https://s3-alpha-sig.figma.com/img/24b0/6366/2a63eb933a283ca80f4847a0a25fcbf1?Expires=1712534400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=W~oncfdnASzHMYdoanoiqhGRL3br0EgHQYQipq3Df-SnPeXZrub3cllOYdn5e1qP8KlGc8PWspCncYXxxZIKCWZ9zix~hn1E7nvksw6~U-jTJvZZ5FUkJP2Y8jLTaifOz7vu6YwPCy6AZFHmVIgrMe7bQW0BqYinrWeyJ0WaJwZQ-7p0YrK1f4OZfTp~Cr4EKbhcA1Pg~s~tm05DZqG4PI1PR6HF4Bg6FyRhMS4TXMZuYLEcwR159MciY-zdpBFRU5dCCMWp~uZPSNxg9897TfgRqAXjReHrRXp56UCxanhaX13QsfBAQ9puhL33hrB5Nu1tuUuyw-AaLDpT9c9lhQ__" 
     />
     </swiper-slide>
  </swiper>






</template>

<style scoped>

@media screen and (max-width: 1920px) {
  #business2 {
    display: none;
  }
  #business3 {
    display: none;
  }
}

@media screen and (max-width: 1500px) {
  #info {
  display: block;
  margin-left: 165px !important;
  justify-content: center;
  align-items: center;
}
}

@media screen and (max-width: 1669px) {
  #info {
  display: block;
  margin-left: 240px !important;
  justify-content: center;
  align-items: center;
}
#posts {
  display: grid;
  margin-left: 1200px !important;
  justify-content: center;
  align-items: center;
  width: 304px;
  height: 618;
  margin-top: -525px !important;
  border-radius: 20px;
}

#posts2 {
  display: grid;
  margin-left: 1200px !important;
  justify-content: center;
  align-items: center;
  width: 304px;
  height: 618;
  margin-top: 50px !important;
  border-radius: 20px;
}

}

@media screen and (max-width: 1300px) {
  #info {
  display: block;
  margin-left: 80px !important;
  justify-content: center;
  align-items: center;
}
#posts {
  display: grid;
  margin-left: 1050px !important;
  justify-content: center;
  align-items: center;
  width: 250px !important;
  height: 618;
  margin-top: -525px !important;
  border-radius: 20px;

}

#posts2 {
  display: grid;
  margin-left: 1050px !important;
  justify-content: center;
  align-items: center;
  width: 250px !important;
  height: 618;
  margin-top: 50px !important;
  border-radius: 20px;

}

}

@media screen and (max-width: 1097px) {
  #business {
    display: none;
  }
  #info {
  display: block;
  margin-left: 20px !important;
  justify-content: center;
  align-items: center;
}
#posts {
  display: grid;
  margin-left: 950px !important;
  justify-content: center;
  align-items: center;
  width: 150px !important;
  height: 618;
  margin-top: -525px !important;
  border-radius: 20px;
}
#posts2 {
  display: grid;
  margin-left: 950px !important;
  justify-content: center;
  align-items: center;
  width: 150px !important;
  height: 618;
  margin-top: -52px !important;
  border-radius: 20px;
}
}

  @media screen and (max-width: 767px) {
    #business {
      display: block;
    }
     #business2 {
      display: block;
    }
    #business3 {
      display: block;
    }
    #dropdownHoverButton {
      display: none;
    }
    #info {
  display: block;
  margin-left: 15px !important;
  justify-content: center;
  align-items: center;
}

#posts {
  display: grid;
  margin-left: 50px !important;
  justify-content: center;
  align-items: center;
  width: 150px !important;
  height: 118;
  margin-top: 30px !important;
  border-radius: 20px;
}

#posts2 {
  display: grid;
  margin-left: 50px !important;
  justify-content: center;
  align-items: center;
  width: 150px !important;
  height: 118;
  margin-top: 30px !important;
  border-radius: 20px;
}


  }

.swiper-slide {
  text-align: center;
  font-size: 18px;


  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;

}

.swiper-slide img {
  display: block;
  width: 952px;
  height: 406px;
  object-fit: cover;
  border-radius: 20px;
  margin-right: 15%;
  
}

#info {
  display: block;
  margin-left: 18%;
  justify-content: center;
  align-items: center;

}

#posts {
  display: grid;
  margin-left: 71%;
  justify-content: center;
  align-items: center;
  width: 304px;
  height: 618;
  margin-top: -28%;
  border-radius: 20px;
}

#posts2 {
  display: grid;
  margin-left: 71%;
  justify-content: center;
  align-items: center;
  width: 304px;
  height: 618;
  margin-top: 5%;
  border-radius: 20px;
}

.mySwiper2 {
  margin-top: -860px;
  margin-left: 180px;
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  padding-right: -1px;
    margin-right: -1px;
}




</style>
