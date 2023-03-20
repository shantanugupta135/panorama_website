
<template>
  <div class="bg-white">
    <!-- Header -->
    <!-- <header class="absolute inset-x-0 top-0 z-50">
      <nav class="flex items-center justify-between p-6 lg:px-8" aria-label="Global">
        <div class="flex lg:flex-1">
          <a href="#" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img class="h-8 w-auto bg-white " src="https://panoramacorp.in/img/logo_new.png" alt="" />
          </a>
        </div>
        <div class="flex lg:hidden">
        <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-400" @click="mobileMenuOpen = true">
          <span class="sr-only">Open main menu</span>
          <Bars3Icon class="h-6 w-6" aria-hidden="true" />
        </button>
      </div>
      <div class="hidden lg:flex lg:gap-x-12">
        <a v-for="item in navigation" :key="item.name" :href="item.href" class="text-sm font-semibold leading-6 text-white">{{ item.name }}</a>
      </div>
      <div class="hidden lg:flex lg:flex-1 lg:justify-end">
        <a href="#" class="text-sm font-semibold leading-6 text-white">Log in <span aria-hidden="true">&rarr;</span></a>
      </div>
      </nav>

      <Dialog as="div" class="lg:hidden" @close="mobileMenuOpen = false" :open="mobileMenuOpen">
      <div class="fixed inset-0 z-10" />
      <DialogPanel class="fixed inset-y-0 right-0 z-10 w-full overflow-y-auto bg-gray-900 px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-white/10">
        <div class="flex items-center justify-between">
          <a href="#" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=500" alt="" />
          </a>
          <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-400" @click="mobileMenuOpen = false">
            <span class="sr-only">Close menu</span>
            <XMarkIcon class="h-6 w-6" aria-hidden="true" />
          </button>
        </div>
        <div class="mt-6 flow-root">
          <div class="-my-6 divide-y divide-gray-500/25">
            <div class="space-y-2 py-6">
              <a v-for="item in navigation" :key="item.name" :href="item.href" class="-mx-3 block rounded-lg py-2 px-3 text-base font-semibold leading-7 text-white hover:bg-gray-800">{{ item.name }}</a>
            </div>
            <div class="py-6">
              <a href="#" class="-mx-3 block rounded-lg py-2.5 px-3 text-base font-semibold leading-7 text-white hover:bg-gray-800">Log in</a>
            </div>
          </div>
        </div>
      </DialogPanel>
    </Dialog>

    </header> -->

    <header class="bg-gray-900">
    <nav class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" aria-label="Global">
      <div class="flex lg:flex-1">
        <a href="#" class="-m-1.5 p-1.5">
          <span class="sr-only">Your Company</span>
          <img class="h-8 w-auto" src="https://panoramacorp.in/img/logo_new.png" alt="" />
        </a>
      </div>
      <div class="flex lg:hidden">
        <button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-400" @click="mobileMenuOpen = true">
          <span class="sr-only">Open main menu</span>
          <Bars3Icon class="h-6 w-6" aria-hidden="true" />
        </button>
      </div>
      <div class="hidden lg:flex lg:gap-x-12">
        <a v-for="item in navigation" :key="item.name" :href="'#'+item.href" class="text-sm font-semibold leading-6 text-white">{{ item.name }}</a>
      </div>
      <div class="hidden lg:flex lg:flex-1 lg:justify-end">
        <a href="#" class="text-sm font-semibold leading-6 text-white">Log in <span aria-hidden="true">&rarr;</span></a>
      </div>
    </nav>
    <Dialog as="div" class="lg:hidden" @close="mobileMenuOpen = false" :open="mobileMenuOpen">
      <div class="fixed inset-0 z-10" />
      <DialogPanel class="fixed inset-y-0 right-0 z-10 w-full overflow-y-auto bg-gray-900 px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-white/10">
        <div class="flex items-center justify-between">
          <a href="#" class="-m-1.5 p-1.5">
            <span class="sr-only">Your Company</span>
            <img class="h-8 w-auto" src="https://panoramacorp.in/img/logo_new.png" alt="" />
          </a>
          <button type="button" class="-m-2.5 rounded-md p-2.5 text-gray-400" @click="mobileMenuOpen = false">
            <span class="sr-only">Close menu</span>
            <XMarkIcon class="h-6 w-6" aria-hidden="true" />
          </button>
        </div>
        <div class="mt-6 flow-root">
          <div class="-my-6 divide-y divide-gray-500/25">
            <div class="space-y-2 py-6">
              <a v-for="item in navigation" :key="item.name" :href="'#'+item.href" class="-mx-3 block rounded-lg py-2 px-3 text-base font-semibold leading-7 text-white hover:bg-gray-800"
              @close="mobileMenuOpen = false" :open="mobileMenuOpen">{{ item.name }}</a>
            </div>
            <div class="py-6">
              <a href="#" class="-mx-3 block rounded-lg py-2.5 px-3 text-base font-semibold leading-7 text-white hover:bg-gray-800">Log in</a>
            </div>
          </div>
        </div>
      </DialogPanel>
    </Dialog>
  </header>

    <main id="home">
      <!-- Hero section -->
      <div class="relative isolate overflow-hidden bg-gray-900 pt-14 pb-16 sm:pb-20 w-full">
        <img
          src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2830&q=80&blend=111827&sat=-100&exp=15&blend-mode=multiply"
          alt="" class="absolute inset-0 -z-10 h-full w-full object-cover" />
        <div class="absolute inset-x-0 top-[-10rem] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[-20rem]">
          <svg
            class="relative left-[calc(50%-11rem)] -z-10 h-[21.1875rem] max-w-none -translate-x-1/2 rotate-[30deg] sm:left-[calc(50%-30rem)] sm:h-[42.375rem]"
            viewBox="0 0 1155 678">
            <path fill="url(#45de2b6b-92d5-4d68-a6a0-9b9b2abad533)" fill-opacity=".2"
              d="M317.219 518.975L203.852 678 0 438.341l317.219 80.634 204.172-286.402c1.307 132.337 45.083 346.658 209.733 145.248C936.936 126.058 882.053-94.234 1031.02 41.331c119.18 108.451 130.68 295.337 121.53 375.223L855 299l21.173 362.054-558.954-142.079z" />
            <defs>
              <linearGradient id="45de2b6b-92d5-4d68-a6a0-9b9b2abad533" x1="1155.49" x2="-78.208" y1=".177" y2="474.645"
                gradientUnits="userSpaceOnUse">
                <stop stop-color="#9089FC" />
                <stop offset="1" stop-color="#FF80B5" />
              </linearGradient>
            </defs>
          </svg>
        </div>
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-3xl py-32 sm:py-32 lg:py-48">
            <div class="text-center">
              <h1 class="text-4xl font-bold tracking-tight text-white sm:text-6xl">
                Invest in <span class="bg-sky-800">Verification</span>
                <br />For better & secured growth
              </h1>
              <p class="mt-6 text-lg leading-8 text-gray-300">
                It is said that Information is the resolution of uncertainty.
                This is true about both our personal and professional lives. We
                at Panorama, help in this resolution by providing a
                comprehensive view about the prospective associations that an
                organization might be entering into.
              </p>
              <div class="mt-10 flex items-center justify-center gap-x-6">
                <a href="#"
                  class="rounded-md bg-sky-800 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-slate-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-400">Get
                  started</a>
                <a href="#" class="text-sm font-semibold leading-6 text-white">Live demo <span
                    aria-hidden="true">→</span></a>
              </div>
            </div>
          </div>

          <!-- Logo cloud -->
          <div
            class="mx-auto grid max-w-lg grid-cols-4 items-center gap-x-8 gap-y-10 sm:max-w-xl sm:grid-cols-6 sm:gap-x-10 lg:mx-0 lg:max-w-none lg:grid-cols-5">
             <img class="col-span-2 max-h-12 w-full object-contain lg:col-span-1"
              src="https://tailwindui.com/img/logos/158x48/transistor-logo-white.svg" alt="Transistor" width="158"
              height="48" />
            <img class="col-span-2 max-h-12 w-full object-contain lg:col-span-1"
              src="https://tailwindui.com/img/logos/158x48/reform-logo-white.svg" alt="Reform" width="158" height="48" />
            <img class="col-span-2 max-h-12 w-full object-contain lg:col-span-1"
              src="https://tailwindui.com/img/logos/158x48/tuple-logo-white.svg" alt="Tuple" width="158" height="48" />
            <img class="col-span-2 max-h-12 w-full object-contain sm:col-start-2 lg:col-span-1"
              src="https://tailwindui.com/img/logos/158x48/savvycal-logo-white.svg" alt="SavvyCal" width="158"
              height="48" />
            <img class="col-span-2 col-start-2 max-h-12 w-full object-contain sm:col-start-auto lg:col-span-1"
              src="https://tailwindui.com/img/logos/158x48/statamic-logo-white.svg" alt="Statamic" width="158"
              height="48" />
          </div>
        </div>
        <div
          class="absolute inset-x-0 top-[calc(100%-13rem)] -z-10 transform-gpu overflow-hidden blur-3xl sm:top-[calc(100%-30rem)]">
          <svg
            class="relative left-[calc(50%+3rem)] h-[21.1875rem] max-w-none -translate-x-1/2 sm:left-[calc(50%+36rem)] sm:h-[42.375rem]"
            viewBox="0 0 1155 678">
            <path fill="url(#ecb5b0c9-546c-4772-8c71-4d3f06d544bc)" fill-opacity=".2"
              d="M317.219 518.975L203.852 678 0 438.341l317.219 80.634 204.172-286.402c1.307 132.337 45.083 346.658 209.733 145.248C936.936 126.058 882.053-94.234 1031.02 41.331c119.18 108.451 130.68 295.337 121.53 375.223L855 299l21.173 362.054-558.954-142.079z" />
            <defs>
              <linearGradient id="ecb5b0c9-546c-4772-8c71-4d3f06d544bc" x1="1155.49" x2="-78.208" y1=".177" y2="474.645"
                gradientUnits="userSpaceOnUse">
                <stop stop-color="#9089FC" />
                <stop offset="1" stop-color="#FF80B5" />
              </linearGradient>
            </defs>
          </svg>
        </div>
      </div>

      <!-- Feature section -->
      <div class="mt-32 sm:mt-16">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-5xl sm:text-center">
            <h2 class="text-base font-semibold leading-7 text-sky-800">
              Everything you need
            </h2>
            <p class="mt-2 text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
              Do you want to <span class="text-red-700">K</span>now
              <span class="text-red-700">Y</span>our
              <span class="text-red-700">C</span>ustomer/<span class="text-red-700">A</span>ssociate?
            </p>
            <p class="mt-6 text-lg leading-8 text-gray-600">
              We believe that every organization needs to have a complete and an
              uninterrupted view of whatever it is dealing in. It can be related
              to its business and/or its stakeholders. The company thus proposes
              to be a one-stop shop for all the needs associated with processing
              and verifications. We will make every effort to aid, smoothen,
              fasten and improve the procedures through experience, commitment
              and technology.
            </p>
          </div>
        </div>

         <!-- Services Offered section -->

        <div class="relative overflow-hidden pt-16">
          <div class="mx-auto max-w-7xl px-6 lg:px-8">
            <img src="https://tailwindui.com/img/component-images/project-app-screenshot.png" alt="App screenshot"
              class="mb-[-12%] rounded-xl shadow-2xl ring-1 ring-gray-900/10" width="2432" height="1442" />
            <div class="relative" aria-hidden="true">
              <div class="absolute -inset-x-20 bottom-0 bg-gradient-to-t from-white pt-[7%]" />
            </div>
          </div>
        </div>
        <div class="mx-auto mt-16 max-w-7xl px-6 sm:mt-20 md:mt-20 lg:px-8" id="services">
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl lg:px-8 text-center">
            Services Offered
          </h2>
          <dl
            class="mx-auto grid max-w-2xl grid-cols-1 gap-x-6 gap-y-10 text-base leading-7 text-gray-600 sm:grid-cols-2 lg:mx-0 lg:max-w-none lg:grid-cols-3 lg:gap-x-8 lg:gap-y-16 pt-8">
            <div v-for="feature in features" class="relative pl-9">
              <div class="flex justify-center">
                <div class="w-20 h-20 rounded-full border-2 border-blue flex justify-center items-center bg-sky-800">
                  <div class="text-gray-900 flex justify-center">
                    <component :is="feature.icon" class="h-12 w-12 text-white" />
                  </div>
                </div>
              </div>
            <!-- <div class = "group"> 
              {{ feature.name }}
              <p class="invisible group-hover:visible h-10 hover:h-full animate-pulse">{{ feature.description }}</p>
                        </div> -->
              <div class="flex justify-center mt-7 font-bold">
                {{ feature.name }}
              </div>
              <dd class="mt-7 text-base leading-8 text-gray-600">{{ feature.description }}</dd>
            </div>
          </dl>
        </div>
      </div>


      <div class="bg-white py-16 sm:py-16" id="about">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-2xl text-center sm:text-center">
            <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
              Meet our leadership
            </h2>

            <p class="mt-6 text-lg leading-8 text-gray-600">
              We’re a dynamic group of individuals who are passionate about what
              we do and dedicated to delivering the best results for our
              clients.
            </p>
          </div>

          <ul role="list"
            class="mx-auto mt-20 grid max-w-2xl grid-cols-1 gap-x-6 gap-y-20 sm:grid-cols-2 lg:max-w-4xl lg:gap-x-8 xl:max-w-none">
            <li v-for="person in people" :key="person.name"
              class="flex flex-col gap-6 xl:flex-row items-center text-center">
              <img class="aspect-[4/5] w-52 rounded-2xl object-cover" :src="person.imageUrl" alt="" />
              <div class="flex-auto">
                <h3 class="text-lg font-semibold leading-8 tracking-tight text-gray-900">
                  {{ person.name }}
                </h3>
                <p class="text-base leading-7 text-gray-600">
                  {{ person.role }}
                </p>
                <p class="mt-6 text-base leading-7 text-gray-500">
                  {{ person.bio }}
                </p>
              </div>
            </li>
          </ul>
        </div>
      </div>

      <!-- Why Panorma -->
      <div class="py-3 sm:py-7">
        <div class="">
          <div class="mx-auto max-w-2xl text-center">
            <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
              Why Panorma?
            </h2>
          </div>
          <div class="mt-10 bg-sky-800">
            <ul class="list-disc text-gray-300 px-10 pt-3 pb-2 text-lg leading-8 lg:ml-20">
              <li class="pb-2">Experience in financial products and the intricacies associated with them.</li>
              <li class="pb-2">Domain knowledge of finance industry and its challenges.</li>
              <li class="pb-2">Use of technology as an enabler, to deliver accuracy with speed.</li>
              <li class="pb-2">Dedicated and experienced team of domain experts, field verifiers and backhand support.
              </li>
              <li class="pb-2">Attuned to the dynamic requirements of our clients.</li>
            </ul>
          </div>
        </div>
      </div>

      <!-- Meet our Clients -->

      <div class="bg-white sm:py-10">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-2xl text-center sm:text-center mt-6">
            <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
              Life at Panorma
            </h2>
          </div>
          <div id="controls-carousel" class="relative w-full mt-10" data-carousel="slide">
            <!-- Carousel wrapper -->
            <div class="relative h-56 overflow-hidden rounded-lg md:h-96">
              <!-- Item 1 -->
              <div class="hidden duration-700 ease-in-out" data-carousel-item>
                <img
                  src="https://previews.123rf.com/images/fizkes/fizkes1806/fizkes180600311/102620868-smiling-colleagues-having-fun-laughing-and-doing-piggyback-ride-at-workplace-coworkers-playing.jpg"
                  class="absolute block w-full -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" alt="...">
              </div>
              <!-- Item 2 -->
              <div class="hidden duration-700 ease-in-out" data-carousel-item="active">
                <img
                  src="https://previews.123rf.com/images/opolja/opolja1801/opolja180100213/94962859-cheerful-colleagues-having-fun-in-office-chairs.jpg"
                  class="absolute block w-full -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" alt="...">
              </div>
              <!-- Item 3 -->
              <div class="hidden duration-700 ease-in-out" data-carousel-item>
                <img
                  src="https://previews.123rf.com/images/opolja/opolja1801/opolja180100213/94962859-cheerful-colleagues-having-fun-in-office-chairs.jpg"
                  class="absolute block w-full -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2" alt="...">
              </div>
            </div>

            <!-- Slider controls -->
            <button type="button"
              class="absolute top-0 left-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none"
              data-carousel-prev>
              <span
                class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none">
                <svg aria-hidden="true" class="w-6 h-6 text-white dark:text-gray-800" fill="none" stroke="currentColor"
                  viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path>
                </svg>
                <span class="sr-only">Previous</span>
              </span>
            </button>
            <button type="button"
              class="absolute top-0 right-0 z-30 flex items-center justify-center h-full px-4 cursor-pointer group focus:outline-none"
              data-carousel-next>
              <span
                class="inline-flex items-center justify-center w-10 h-10 rounded-full bg-white/30 dark:bg-gray-800/30 group-hover:bg-white/50 dark:group-hover:bg-gray-800/60 group-focus:ring-4 group-focus:ring-white dark:group-focus:ring-gray-800/70 group-focus:outline-none">
                <svg aria-hidden="true" class="w-6 h-6 text-white dark:text-gray-800" fill="none" stroke="currentColor"
                  viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path>
                </svg>
                <span class="sr-only">Next</span>
              </span>
            </button>
          </div>
        </div>
      </div>

      <div class="bg-white sm:py-10 mt-10 sm:mt-10">
            <div class="mx-auto max-w-7xl px-6 lg:px-8">
              <div class="mx-auto max-w-2xl text-center sm:text-center">
              <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
                Meet our Clients
              </h2>
            </div>
            <div class="carousel-image mt-2">
          <Carousel :settings="settings" :breakpoints="breakpoints" :autoplay="2000" :wrap-around="true">
        <Slide v-for="slide in carouselImg" :key="slide">
          <div class="carousel__item px-7">
            <img src="https://download.logo.wine/logo/Axis_Bank/Axis_Bank-Logo.wine.png" alt="black chair and white table" />
          </div>
        </Slide>
      </Carousel>
      </div>
    </div>
   </div>

      <!-- Blog section -->
      <div class="bg-white py-2 sm:py-8" id="blog">
        <div class="mx-auto max-w-7xl px-6 lg:px-8">
          <div class="mx-auto max-w-2xl text-center">
            <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
              From the blog
            </h2>
            <p class="mt-2 text-lg leading-8 text-gray-600">
              Learn how to grow your business with our expert advice.
            </p>
          </div>

          <div class="mx-auto mt-6 grid max-w-2xl grid-cols-1 gap-y-20 gap-x-8 lg:mx-0 lg:max-w-none lg:grid-cols-3">
            <article v-for="post in posts" :key="post.id" class="flex flex-col items-start justify-between">
            <!-- <div class="relative w-full">
                <img
                  :src="post.imageUrl"
                  alt=""
                  class="aspect-[16/9] w-full rounded-2xl bg-gray-100 object-cover sm:aspect-[2/1] lg:aspect-[3/2]"
                />
                <div
                  class="absolute inset-0 rounded-2xl ring-1 ring-inset ring-gray-900/10"
                />
                        </div> -->
              <div class="max-w-2xl">
                <div class="mt-8 flex items-center text-xs justify-center">
                  <time :datetime="post.datetime" class="text-gray-500">{{
                    post.date
                  }}</time>
                  <a :href="post.category.href"
                    class="relative z-10 rounded-full bg-gray-50 py-1.5 px-3 font-medium text-gray-600 hover:bg-gray-100">{{
                      post.category.title }}</a>
                </div>
                <div class="group relative text-center">
                  <h3 class="mt-3 text-lg font-semibold leading-6 text-gray-900 group-hover:text-gray-600">
                    <a :href="post.href">
                      <span class="absolute inset-0" />
                      {{ post.title }}
                    </a>
                  </h3>
                  <p class="mt-5 text-base leading-6 text-gray-600 line-clamp-3">
                    {{ post.description }}
                  </p>
                </div>
                <div class="relative mt-8 flex items-center gap-x-4 justify-center">
                  <img :src="post.author.imageUrl" alt="" class="h-10 w-10 rounded-full bg-gray-100" />
                  <div class="text-sm leading-6">
                    <p class="font-semibold text-gray-900">
                      <a :href="post.author.href">
                        <span class="absolute inset-0" />
                        {{ post.author.name }}
                      </a>
                    </p>
                    <p class="text-gray-600">{{ post.author.role }}</p>
                  </div>
                </div>
              </div>
            </article>
          </div>
        </div>
      </div>


      <!-- Contact Us -->
      <div class="relative isolate bg-sky-800 mt-6">
        <div class="mx-auto grid max-w-7xl grid-cols-1 lg:grid-cols-2">
          <div class="relative px-6 pt-4 pb-10 sm:pt-12 lg:static lg:py-24 lg:px-8">
            <div class="mx-auto max-w-xl lg:mx-0 lg:max-w-lg">
              <h2 class="text-3xl font-bold tracking-tight text-white">
                Get in touch
              </h2>
              <dl class="mt-10 space-y-4 text-base leading-7 text-white">
                <div class="flex gap-x-4">
                  <dt class="flex-none">
                    <span class="sr-only">Telephone</span>
                    <BuildingOffice2Icon class="h-7 w-6 text-white" aria-hidden="true" />
                  </dt>
                  <dd>WYNN Plaza C-2A <br/> Acharya Niketan Mayur Vihar-I <br />New Delhi-110091</dd>
                </div>
                <div class="flex gap-x-4">
                  <dt class="flex-none">
                    <span class="sr-only">Telephone</span>
                    <PhoneIcon class="h-7 w-6 text-white" aria-hidden="true" />
                  </dt>
                  <dd>
                    <a class="hover:text-gray-900" href="tel:+1 (555) 234-5678">+911149077374</a>
                  </dd>
                </div>
                <div class="flex gap-x-4">
                  <dt class="flex-none">
                    <span class="sr-only">Telephone</span>
                    <PhoneIcon class="h-7 w-6 text-white" aria-hidden="true" />
                  </dt>
                  <dd>
                    <a class="hover:text-gray-900" href="tel:+1 (555) 234-5678">+911149077375</a>
                  </dd>
                </div>
                <div class="flex gap-x-4">
                  <dt class="flex-none">
                    <span class="sr-only">Telephone</span>
                    <EnvelopeIcon class="h-7 w-6 text-white" aria-hidden="true" />
                  </dt>
                  <dd>
                    <a class="hover:text-gray-900" href="info@panoramacorp.in">info@panoramacorp.in</a>
                  </dd>
                </div>
              </dl>
            </div>
          </div>
          <div class="px-6 pb-10 pt-4 sm:pb-10 lg:py-24 lg:px-8 sm:px-8">
            <div class="gmap2">
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3502.696673570967!2d77.2913983149228!3d28.608875182427056!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x390ce5eb1ac8fa23%3A0x4ce0b0aa80b26369!2sWynn%20Plaza!5e0!3m2!1sen!2sin!4v1678902661979!5m2!1sen!2sin" class="g-map" allowfullscreen="" loading="lazy"></iframe>
            </div>
          </div>
        </div>
      </div>

      <!-- FAQ section -->
    <!-- <div class="mx-auto mt-2 mb-8 max-w-7xl px-6 sm:mt-8 lg:px-8">
        <div class="mx-auto max-w-4xl divide-y divide-gray-900/10">
          <h2 class="text-2xl font-bold leading-10 tracking-tight text-gray-900">
            Frequently asked questions
          </h2>
          <dl class="mt-10 space-y-6 divide-y divide-gray-900/10">
            <Disclosure as="div" v-for="faq in faqs" :key="faq.question" class="pt-6" v-slot="{ open }">
              <dt>
                <DisclosureButton class="flex w-full items-start justify-between text-left text-gray-900">
                  <span class="text-base font-semibold leading-7">{{
                    faq.question
                  }}</span>
                  <span class="ml-6 flex h-7 items-center">
                    <PlusSmallIcon v-if="!open" class="h-6 w-6" aria-hidden="true" />
                    <MinusSmallIcon v-else class="h-6 w-6" aria-hidden="true" />
                  </span>
                </DisclosureButton>
              </dt>
              <DisclosurePanel as="dd" class="mt-2 pr-12">
                <p class="text-base leading-7 text-gray-600">
                  {{ faq.answer }}
                </p>
              </DisclosurePanel>
            </Disclosure>
          </dl>
        </div>
          </div> -->
    </main>

    <!-- Footer -->
    <footer class="border-t border-gray-900/10  bg-slate-800">
      <div class="mx-auto max-w-7xl py-12 px-6 md:flex md:items-center md:justify-between lg:px-8">
        <div class="flex justify-center space-x-6 md:order-2">
          <a v-for="item in footerNavigation" :key="item.name" :href="item.href"
            class="text-gray-400 hover:text-gray-500">
            <span class="sr-only">{{ item.name }}</span>
            <component :is="item.icon" class="h-6 w-6" aria-hidden="true" />
          </a>
        </div>
        <div class="mt-8 md:order-1 md:mt-0">
          <p class="text-center text-xs leading-5 text-gray-500">
            &copy; 2023 PanoramaCorp, Inc. All rights reserved.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>
  
<script setup>
import { ref } from "vue";
import { defineComponent, h } from "vue";
import {
  Dialog,
  DialogPanel,
  Disclosure,
  DisclosureButton,
  DisclosurePanel,
} from "@headlessui/vue";
import {
  Bars3Icon,
  MinusSmallIcon,
  PlusSmallIcon,
  XMarkIcon,
  BuildingOffice2Icon,
  EnvelopeIcon,
  PhoneIcon,
} from "@heroicons/vue/24/outline";
import {
  CurrencyDollarIcon,
  UserIcon,
  ArrowTrendingUpIcon,
  HandThumbUpIcon,
  DocumentCheckIcon,
} from "@heroicons/vue/24/solid";
import {
  ArrowPathIcon,
  CheckIcon,
  CloudArrowUpIcon,
  Cog6ToothIcon,
  FingerPrintIcon,
  LockClosedIcon,
  ServerIcon,
} from "@heroicons/vue/20/solid";
import 'flowbite';


const navigation = [
  { name: "Home", href: "home" },
  { name: "Services", href: "services" },
  { name: "Blog", href: "blog" },
  { name: "About", href: "about" },
];
const features = [
  {
    name: "Contact Point Verification.",
    description:
      "The Company is offering its services for CPV as per the requirement of the concerned institution. It may be in financial or any other sector that wants a background check of the addresses being furnished by its clients/employees/ vendors/ associates. We use features like the Geo Tagging and Clic2Call in our system.",
    icon: UserIcon,
  },
  {
    name: "Stock / Asset Verification.",
    description:
      "The company offers its services for conducting dealer/SME stock and WC audit . We are presently operational in NCR/Western UP and Punjab. We also extend our services for Post disbursement verification/ inspection of assets being financed.",
    icon: ArrowTrendingUpIcon,
  },
  {
    name: "Pre Credit Appraisal.",
    description:
      "Pre credit appraisal of a loan proposal is an important job in the sanction and disbursal of a credit facility. The company offers its services towards data entry as well as loan proposal processing.",
    icon: HandThumbUpIcon,
  },
  {
    name: "Document Verification.",
    description:
      "The Company offers to do a due diligent check of the documents being furnished by clients/employees/vendor s/ associates of our customers.",
    icon: DocumentCheckIcon,
  },
  {
    name: "TSR / Valuation.",
    description:
      "The company is offering its services for doing the Legall Verification of Property documents along with its valuation.",
    icon: CurrencyDollarIcon,
  },
  {
    name: "Personal Discussion.",
    description:
      "We offer our services for conducting exhaustive personal discussion for high ticket credit exposure.",
    icon: FingerPrintIcon,
  },
];
const tiers = [
  {
    name: "Hobby",
    id: "tier-hobby",
    href: "#",
    priceMonthly: "$19",
    description:
      "The perfect plan if you're just getting started with our product.",
    features: [
      "25 products",
      "Up to 10,000 subscribers",
      "Advanced analytics",
      "24-hour support response time",
    ],
    featured: false,
  },
  {
    name: "Enterprise",
    id: "tier-enterprise",
    href: "#",
    priceMonthly: "$49",
    description: "Dedicated support and infrastructure for your company.",
    features: [
      "Unlimited products",
      "Unlimited subscribers",
      "Advanced analytics",
      "Dedicated support representative",
      "Marketing automations",
      "Custom integrations",
    ],
    featured: true,
  },
];
const faqs = [
  {
    question: "What's the best thing about Switzerland?",
    answer:
      "I don't know, but the flag is a big plus. Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas cupiditate laboriosam fugiat.",
  },
  // More questions...
];
const footerNavigation = [
  {
    name: "Facebook",
    href: "#",
    icon: defineComponent({
      render: () =>
        h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
          h("path", {
            "fill-rule": "evenodd",
            d: "M22 12c0-5.523-4.477-10-10-10S2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094 0 2.238.195 2.238.195v2.46h-1.26c-1.243 0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12z",
            "clip-rule": "evenodd",
          }),
        ]),
    }),
  },
  {
    name: "Instagram",
    href: "#",
    icon: defineComponent({
      render: () =>
        h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
          h("path", {
            "fill-rule": "evenodd",
            d: "M12.315 2c2.43 0 2.784.013 3.808.06 1.064.049 1.791.218 2.427.465a4.902 4.902 0 011.772 1.153 4.902 4.902 0 011.153 1.772c.247.636.416 1.363.465 2.427.048 1.067.06 1.407.06 4.123v.08c0 2.643-.012 2.987-.06 4.043-.049 1.064-.218 1.791-.465 2.427a4.902 4.902 0 01-1.153 1.772 4.902 4.902 0 01-1.772 1.153c-.636.247-1.363.416-2.427.465-1.067.048-1.407.06-4.123.06h-.08c-2.643 0-2.987-.012-4.043-.06-1.064-.049-1.791-.218-2.427-.465a4.902 4.902 0 01-1.772-1.153 4.902 4.902 0 01-1.153-1.772c-.247-.636-.416-1.363-.465-2.427-.047-1.024-.06-1.379-.06-3.808v-.63c0-2.43.013-2.784.06-3.808.049-1.064.218-1.791.465-2.427a4.902 4.902 0 011.153-1.772A4.902 4.902 0 015.45 2.525c.636-.247 1.363-.416 2.427-.465C8.901 2.013 9.256 2 11.685 2h.63zm-.081 1.802h-.468c-2.456 0-2.784.011-3.807.058-.975.045-1.504.207-1.857.344-.467.182-.8.398-1.15.748-.35.35-.566.683-.748 1.15-.137.353-.3.882-.344 1.857-.047 1.023-.058 1.351-.058 3.807v.468c0 2.456.011 2.784.058 3.807.045.975.207 1.504.344 1.857.182.466.399.8.748 1.15.35.35.683.566 1.15.748.353.137.882.3 1.857.344 1.054.048 1.37.058 4.041.058h.08c2.597 0 2.917-.01 3.96-.058.976-.045 1.505-.207 1.858-.344.466-.182.8-.398 1.15-.748.35-.35.566-.683.748-1.15.137-.353.3-.882.344-1.857.048-1.055.058-1.37.058-4.041v-.08c0-2.597-.01-2.917-.058-3.96-.045-.976-.207-1.505-.344-1.858a3.097 3.097 0 00-.748-1.15 3.098 3.098 0 00-1.15-.748c-.353-.137-.882-.3-1.857-.344-1.023-.047-1.351-.058-3.807-.058zM12 6.865a5.135 5.135 0 110 10.27 5.135 5.135 0 010-10.27zm0 1.802a3.333 3.333 0 100 6.666 3.333 3.333 0 000-6.666zm5.338-3.205a1.2 1.2 0 110 2.4 1.2 1.2 0 010-2.4z",
            "clip-rule": "evenodd",
          }),
        ]),
    }),
  },
  {
    name: "Twitter",
    href: "#",
    icon: defineComponent({
      render: () =>
        h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
          h("path", {
            d: "M8.29 20.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0022 5.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.072 4.072 0 012.8 9.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 012 18.407a11.616 11.616 0 006.29 1.84",
          }),
        ]),
    }),
  },
  {
    name: "GitHub",
    href: "#",
    icon: defineComponent({
      render: () =>
        h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
          h("path", {
            "fill-rule": "evenodd",
            d: "M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z",
            "clip-rule": "evenodd",
          }),
        ]),
    }),
  },
  {
    name: "YouTube",
    href: "#",
    icon: defineComponent({
      render: () =>
        h("svg", { fill: "currentColor", viewBox: "0 0 24 24" }, [
          h("path", {
            "fill-rule": "evenodd",
            d: "M19.812 5.418c.861.23 1.538.907 1.768 1.768C21.998 8.746 22 12 22 12s0 3.255-.418 4.814a2.504 2.504 0 0 1-1.768 1.768c-1.56.419-7.814.419-7.814.419s-6.255 0-7.814-.419a2.505 2.505 0 0 1-1.768-1.768C2 15.255 2 12 2 12s0-3.255.417-4.814a2.507 2.507 0 0 1 1.768-1.768C5.744 5 11.998 5 11.998 5s6.255 0 7.814.418ZM15.194 12 10 15V9l5.194 3Z",
            "clip-rule": "evenodd",
          }),
        ]),
    }),
  },
];

const people = [
  {
    name: "Navneet Handoo",
    role: "CEO of PanoramaCorp",
    imageUrl: "https://panoramacorp.in/img/navneet.jpeg",
    bio: "During his professional career spanning 13 years, he has worked with Apnaloan.com, Bank of Baroda, Bank of Punjab, Tata Motor Finance and ICICI bank. He has the experience of Sales and Marketing, Branch operations and Credit.",
  },
  {
    name: "Prashant Dogra",
    role: "Co-founder of PanoramaCorp",
    imageUrl: "https://panoramacorp.in/img/prashant.jpeg",
    bio: "He has worked with leading Banks and Financial institutions like Tata Motor Finance, HDFC bank and ICICI bank. He is well versed with retail financial products like Auto Loan, TW loans, Commercial Vehicle Loans and Insurance.",
  },
  {
    name: "Ravi Bhattacharya",
    role: "Head Business",
    imageUrl: "https://panoramacorp.in/img/navneet.jpeg",
    bio: "As an Operations Head , he handles the backend operations along with a dedicated and experienced team of individuals who are always responsive to the needs of our principals. Being a BA LLB, he brings in the professional expertise to the day to day working.",
  },
  {
    name: "Vijay Pant",
    role: "Head Opeartion",
    imageUrl: "https://panoramacorp.in/img/prashant.jpeg",
    bio: "Is a B.Com (Hons) from Delhi Univ, an MA in Economics and a fellow member of the Institute of Chartered Accounts of India. She is instrumental in helping in improving the processes and work flow and identifying the areas of improvements.",
  },
  {
    name: "Kanika Goel",
    role: "Consultant",
    imageUrl: "https://panoramacorp.in/img/prashant.jpeg",
    bio: "Is a B.Com (Hons) from Delhi Univ, an MA in Economics and a fellow member of the Institute of Chartered Accounts of India. She is instrumental in helping in improving the processes and work flow and identifying the areas of improvements.",
  },

  // More people...
];

const posts = [
  {
    id: 1,
    title: "Boost your conversion rate",
    href: "#",
    description:
      "Illo sint voluptas. Error voluptates culpa eligendi. Hic vel totam vitae illo. Non aliquid explicabo necessitatibus unde. Sed exercitationem placeat consectetur nulla deserunt vel. Iusto corrupti dicta.",
    imageUrl:
      "https://images.unsplash.com/photo-1496128858413-b36217c2ce36?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=3603&q=80",
    date: "Mar 16, 2020",
    datetime: "2020-03-16",
    category: { title: "Marketing", href: "#" },
    author: {
      name: "Michael Foster",
      role: "Co-Founder / CTO",
      href: "#",
      imageUrl:
        "https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80",
    },
  },
  {
    id: 2,
    title: "Boost your conversion rate",
    href: "#",
    description:
      "Illo sint voluptas. Error voluptates culpa eligendi. Hic vel totam vitae illo. Non aliquid explicabo necessitatibus unde. Sed exercitationem placeat consectetur nulla deserunt vel. Iusto corrupti dicta.",
    imageUrl:
      "https://images.unsplash.com/photo-1496128858413-b36217c2ce36?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=3603&q=80",
    date: "Mar 16, 2020",
    datetime: "2020-03-16",
    category: { title: "Marketing", href: "#" },
    author: {
      name: "Michael Foster",
      role: "Co-Founder / CTO",
      href: "#",
      imageUrl:
        "https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80",
    },
  },
  {
    id: 3,
    title: "Boost your conversion rate",
    href: "#",
    description:
      "Illo sint voluptas. Error voluptates culpa eligendi. Hic vel totam vitae illo. Non aliquid explicabo necessitatibus unde. Sed exercitationem placeat consectetur nulla deserunt vel. Iusto corrupti dicta.",
    imageUrl:
      "https://images.unsplash.com/photo-1496128858413-b36217c2ce36?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=3603&q=80",
    date: "Mar 16, 2020",
    datetime: "2020-03-16",
    category: { title: "Marketing", href: "#" },
    author: {
      name: "Michael Foster",
      role: "Co-Founder / CTO",
      href: "#",
      imageUrl:
        "https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80",
    },
  },
  // More posts...
];

const mobileMenuOpen = ref(false);
</script>

<script>
import { defineComponent } from 'vue'
import { Carousel, Navigation, Slide } from 'vue3-carousel'

import '../node_modules/vue3-carousel/dist/carousel.css';

export default defineComponent({
  name: 'Breakpoints',
  components: {
    Carousel,
    Slide,
    Navigation,
  },
  data: () => ({
    // carousel settings
    settings: {
      itemsToShow: 1,
      snapAlign: 'center',
    },
    // breakpoints are mobile first
    // any settings not specified will fallback to the carousel settings
    breakpoints: {
      // 700px and up
      700: {
        itemsToShow: 3.5,
        snapAlign: 'center',
      },
      // 1024 and up
      1024: {
        itemsToShow: 5,
        snapAlign: 'start',
      },
    },
  }),
})

const carouselImg = [
  {
    imageUrl: "https://panoramacorp.in/img/navneet.jpeg",
  },
  {
    imageUrl: "https://panoramacorp.in/img/prashant.jpeg",
    bio: "He has worked with leading Banks and Financial institutions like Tata Motor Finance, HDFC bank and ICICI bank. He is well versed with retail financial products like Auto Loan, TW loans, Commercial Vehicle Loans and Insurance.",
  },
  {
    imageUrl: "https://panoramacorp.in/img/navneet.jpeg",
    bio: "As an Operations Head , he handles the backend operations along with a dedicated and experienced team of individuals who are always responsive to the needs of our principals. Being a BA LLB, he brings in the professional expertise to the day to day working.",
  },
  {
    imageUrl: "https://panoramacorp.in/img/prashant.jpeg",
    bio: "Is a B.Com (Hons) from Delhi Univ, an MA in Economics and a fellow member of the Institute of Chartered Accounts of India. She is instrumental in helping in improving the processes and work flow and identifying the areas of improvements.",
  },
  {
    imageUrl: "https://panoramacorp.in/img/prashant.jpeg",
    bio: "Is a B.Com (Hons) from Delhi Univ, an MA in Economics and a fellow member of the Institute of Chartered Accounts of India. She is instrumental in helping in improving the processes and work flow and identifying the areas of improvements.",
  },

  // More people...
];

</script>


