<template>
  <div :class="projectlist?' flex':'flrx hidden'" class="fixed  bg-black/65 h-full z-90 w-full top-0 left-0 flex justify-center items-center">
    <div class="w-11/12 md:w-1/2 bg-white p-6 rounded-lg shadow-lg max-h-[90vh] overflow-y-auto">
      <button @click="toggletemplate" class="  mt-4   bg-red-700 text-white ab  h-6 w-6 rounded-full ">X</button>
      <!-- Warning -->
      <p class="text-red-600 font-semibold text-center mb-4">
        Warning: This website is a student project created by the 2024/2025
        Primary Education students of the University of Ilorin.  
        It is not an official university website. Please beware of fraud.
      </p>

      <!-- Project Info -->
      <p class="text-gray-700 text-center mb-6">
        This project was created as part of a school assignment by the students listed below.
      </p>

      <!-- Participants -->
      <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
        <div
          v-for="(student, index) in participants"
          :key="index"
          class="border rounded-lg p-4 flex items-center gap-4"
        >
          <img
            :src="student.photo"
            alt="Student photo"
            class="w-16 h-16 rounded-full object-cover border"
          />

          <div>
            <p class="font-semibold">{{ student.name }}</p>
            <p class="text-sm text-gray-600">
              Matric No: {{ student.matric }}
            </p>
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';
const projectlist = ref(true)
    
     const  participants= [
        {
          name: "Waliu Waheed",
          matric: "UIL/2024/12345",
          photo: "/images/gallary1.jpg",
        },
        {
          name: "Aisha Bello",
          matric: "UIL/2024/67890",
          photo: "/images/gallary0.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
        {
          name: "John Ade",
          matric: "UIL/2024/54321",
          photo: "/images/gallary4.jpg",
        },
      ]

 const toggletemplate = ()=>{
projectlist.value = !projectlist.value
 }

</script>

<style scoped>
/* Optional: Add custom styles here if needed */
</style>
