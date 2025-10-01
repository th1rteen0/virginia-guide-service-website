<template>
    <div style="height:100vh; background:lightgray">
      Scroll down 👇
    </div>
  
    <!-- This will fade in -->
    <div class="scrollElement" style="height:200px; background:tomato">
      I should fade in!
    </div>
  
    <div style="height:100vh"></div>
  </template>
  
  <script setup>
  import { onMounted } from "vue"
  
  onMounted(() => {
    const observer = new IntersectionObserver((entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.add("show")
        } else {
          entry.target.classList.remove("show")
        }
      })
    })
  
    const scrollElements = document.querySelectorAll(".scrollElement")
    console.log("Found:", scrollElements)
    scrollElements.forEach((el) => observer.observe(el))
  })
  </script>
  
  <style>
  .scrollElement {
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 0.6s ease, transform 0.6s ease;
  }
  .scrollElement.show {
    opacity: 1;
    transform: translateY(0);
  }
  </style>
  