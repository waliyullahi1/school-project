<template>
  <div class="min-h-screen mt-32 bg-gray-100 flex items-center justify-center px-4">
    <div class="max-w-3xl w-full bg-white p-6 rounded-lg shadow-md">

      <!-- Warning Header -->
      <h1 class="text-2xl font-bold text-red-600 text-center mb-4">
        Important Notice
      </h1>

      <!-- Warning Message -->
      <p class="text-gray-700 text-center mb-3">
        To prevent fraud, this website does <strong>not</strong> collect any personal information.
        There is no login system, no database, and no online application.
      </p>

      <p class="text-gray-700 text-center mb-3">
        This is a <strong>frontend-only school project</strong> created for academic purposes.
        It is not an official University of Ilorin website.
      </p>

      <p class="text-gray-700 text-center mb-6">
        The project was designed by students. The list of participants is shown below.
      </p>

      <!-- Student List -->
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

      <!-- Back Button -->
      <div class="text-center">
        <NuxtLink
          to="/"
          class="inline-block bg-primary text-white px-6 py-2 rounded hover:bg-primary/90"
        >
          Go Back Home
        </NuxtLink>
      </div>

    </div>
  </div>
</template>

<script setup>



      const  participants= [
        {
          name: "Abdulwaheed Waliyullahi",
          matric: "24/25OY011",
          photo: "/images/waliu.jpg",
          
        },
        {
          name: "Dosunmu  Boluwatife",
          matric: "24/25OY038",
          photo: "/images/38.png",
          paid:true
        },
         {
          name: "Mukadam  Badmos Imam",
          matric: "24/25OY057",
          photo: "/images/157.jpg",
          paid:false
        },
        {
          name: "Nurudeen  Mujeebah Opeyemi",
          matric: "24/25OY059",
          photo: "/images/59.jpg",
          paid:true
        },
      
        {
          name: "Otitoju Eunice Mercy",
          matric: "24/25OY072",
          photo: "/images/172.jpg",
          paid:true
        },
        {
          name: "Oyerinde Deborah ",
          matric: "24/25OY073",
          photo: "/images/173.jpg",
          paid:true
        },
                {
          name: "Okanlawon Fayidat Oyindamola ",
          matric: "22/25OY073",
          photo: "/images/1fayidah.jpg",
          paid:true
        },
         {
          name: "Soliu Nusirah Adeoye",
          matric: "24/25OY078",
          photo: "/images/78.jpg",
          paid:true
        },
          {
          name: "Sulyman suliyah oluwakemi ",
          matric: "24/25OY079",
          photo: "/images/79.jpg",
          paid:true
        },
         {
          name: "Taiwo abiodun Emmanuel ",
          matric: "24/25OY080",
          photo: "/images/80.jpg",
          paid:true
        },
                  {
          name: "Taofeeq Aishat Ttilope ",
          matric: "24/25OY081",
          photo: "/images/81.jpg",
          paid:true
        },
        {
          name: "Umar Fatimat Adeshewa ",
          matric: "24/25OY082",
          photo: "/images/82.jpg",
          paid:true
        },

        {
          name: "Unachukwu Ifeoma Precious ",
          matric: "24/25OY083",
          photo: "/images/83.jpg",
          paid:true
        },
                {                                                                                                                                                                                                                          
          name: "Usman Aminat Bisola ",
          matric: "24/25OY084",
          photo: "/images/184.jpg",
          paid:true
        },
         {
          name: "Yusuf Haneefat Adeshewa ",
          matric: "24/25OY085",
          photo: "/images/85.jpg",
          paid:true
        },
        {
          name: "Yusuf Rukayat Morenikeji  ",
          matric: "24/25OY086",
          photo: "/images/86.jpg",
          paid:true
        },
        

      ]
</script>
