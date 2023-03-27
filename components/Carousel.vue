<template>
    <div class="carousel">
      <div class="carousel-inner">
        <slot />
      </div>
    </div>
  </template>
  
  <script>
  export default {
    mounted() {
      const carouselInner = this.$el.querySelector('.carousel-inner')
      const carouselItem = carouselInner.querySelectorAll('.carousel-item')
      const carouselItemWidth = carouselItem[0].clientWidth
      const carouselItemMarginRight = parseInt(window.getComputedStyle(carouselItem[0]).marginRight)
      const carouselItemTotalWidth = carouselItemWidth + carouselItemMarginRight
      const carouselItemsCount = carouselItem.length
      const carouselContainerWidth = carouselInner.clientWidth
  
      let currentIndex = 0
      let scrollAmount = 0
  
      setInterval(() => {
        currentIndex++
        if (currentIndex > carouselItemsCount - 1) {
          currentIndex = 0
        }
        scrollAmount = currentIndex * carouselItemTotalWidth
        if (scrollAmount > carouselContainerWidth) {
          carouselInner.style.transform = `translateX(-${scrollAmount}px)`
          currentIndex = 0
          scrollAmount = 0
        } else {
          carouselInner.style.transform = `translateX(-${scrollAmount}px)`
        }
      }, 3000)
    }
  }
  </script>
  
  <style>
  .carousel {
    width: 100%;
    overflow: hidden;
  }
  
  .carousel-inner {
    display: flex;
    flex-wrap: nowrap;
    transition: transform 0.3s ease-in-out;
  }
  
  .carousel-item {
    flex: 0 0 auto;
    width: 180px; /* Change this to your desired width */
    margin-right: 20px; /* Change this to your desired margin */
  }
  </style>