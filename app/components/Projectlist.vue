<template>
  <div :class="projectlist?' flex':'flrx hidden'" class="fixed  bg-black/65 h-full z-90 w-full top-0 left-0 flex justify-center items-center">
    <div class="w-11/12 md:w-1/2 bg-white p-6 rounded-lg shadow-lg max-h-[90vh] overflow-y-auto">
     <div class=" fixed">
      <button @click="toggletemplate" class="  relative bottom-9 right-5 mt-4   bg-red-700 text-white text-xs ab  h-6 w-6 rounded-full ">X</button>
     </div> 
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
      <div class="grid grid-cols-1 items-center justify-center sm:grid-cols-2 gap-4">
        <div
          v-for="(student, index) in participants"
          :key="index"
          class="border flex  flex-col items-center justify-center rounded-lg p-4  gap-4"
        >
        <div class="   w-32 h-32  overflow-hidden rounded-full   flex-shrink-0 mr-4">
           <img
            :src="student.photo"
            alt="Student photo"
            class=" rounded-full object-cover border"
          />
        </div>
         

          <div >
             <p class="font-semibold ">
              Matric No: {{ student.matric }}
            </p>
            <p class="text-sm text-gray-600">{{ student.name }}</p>
            
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
          name: "Abdulwaheed Waliyullahi Idowu",
          matric: "24/25OY011",
          photo: "/images/waliu.jpg",
        },
        {
          name: "Dosunmu  Boluwatife Idowu",
          matric: "24/25OY038",
          photo: "/images/38.png",
        },
         {
          name: "Mukadam  Badmos Imam",
          matric: "24/25OY057",
          photo: "/images/57.jpg",
        },
        {
          name: "Nurudeen  Mujeebah Opeyemi",
          matric: "24/25OY059",
          photo: "/images/59.jpg",
        },
      
        {
          name: "Otitoju Eunice Mercy",
          matric: "24/25OY072",
          photo: "/images/72.jpg",
        },
        {
          name: "Oyerinde Deborah ",
          matric: "24/25OY073",
          photo: "/images/73.jpg",
        },
                {
          name: "Okanlawon Fayidat Oyindamola ",
          matric: "22/25OY073",
          photo: "/images/fayidah.jpg",
        },
          {
          name: "Sulyman suliyah oluwakemi ",
          matric: "24/25OY079",
          photo: "/images/79.jpg",
        },
        {
          name: "Umar Fatimat Adeshewa ",
          matric: "24/25OY082",
          photo: "/images/82.jpg",
        },
        {
          name: "Unachukwu Ifeoluma Precious ",
          matric: "24/25OY083",
          photo: "/images/83.jpg",
        },
                {
          name: "Usman Aminat Bisola ",
          matric: "24/25OY084",
          photo: "/images/84.jpg",
        },
         {
          name: "Usman Aminat Bisola ",
          matric: "24/25OY085",
          photo: "/images/85.jpg",
        },
        {
          name: "Usman Aminat Bisola ",
          matric: "24/25OY086",
          photo: "/images/86.jpg",
        },
        

      ]

 const toggletemplate = ()=>{
projectlist.value = !projectlist.value
 }

</script>

<style scoped>
/* Optional: Add custom styles here if needed */
</style>
