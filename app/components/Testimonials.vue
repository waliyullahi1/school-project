<template>
  <ClientOnly>
    <Carousel v-bind="carouselConfig">
      <Slide v-for="(testimonial, idx) in testimonials" :key="testimonial.name || idx">
        <div class="carousel__item bg-primary mx-1 text-white">
           <div class=" bg-[url('@/assets/images/4T2A1567.png')] bg-no-repeat bg-center bg-cover h-32  flex justify-center  items-center ">
           <div class="bg-primary/50 w-full h-full flex justify-center items-center " >  
            <UiTypographyH2 class="text-white text-center  mb-4">
              <span class="font-bold">Testimonials</span>
            </UiTypographyH2></div>
          </div>

          <div class=" relative -top-16">
            <div class="flex mx-3 justify-center items-center">
             <div class=" relative top-9 rounded-full overflow-hidden border-2 p-4   bg-gray-100 ">
              <img
               src="@/assets/images/unilorin.webp"
               alt="Quote Icon"
               class=" w-16 "/>
               </div>
            </div>

            <div class=" mx-3 rounded-lg text-black p-3 bg-white justify-center pt-12 mb-4">
             
                <p class="text-center text-[12px] font-semibold ">
                  {{ testimonial.quote }}
                </p>
                <div class=" pt-5 flex justify-between">
                  <div>
                    <p class=" text-[12px] leading-tight  font-bold text-secondary">
                     {{ testimonial.name }} <br> <small class="text-[12px] text-black">Parent</small>
                    </p>
                  </div>
                  <div class="flex w-10 space-x-1">
                    <UiIconsStar class="w-5 text-secondary" v-for="i in 5" :key="i" />
                  </div>
                  
                </div>
            </div>
          </div>
         
         
          
        </div>
      </Slide>
    </Carousel>
  </ClientOnly>
</template>
<script setup>
import 'vue3-carousel/carousel.css'
import { Carousel, Slide } from 'vue3-carousel'

const carouselConfig = {
  itemsToShow: 3,
  wrapAround: true,
  autoplay: 3000,

  breakpoints: {
    // Mobile (0px – 639px)
    0: {
      itemsToShow: 1.1,
    },

    // Small tablets (640px+)
    640: {
      itemsToShow: 2,
    },

    // Tablets / small laptops (768px+)
    768: {
      itemsToShow: 3,
    },

    // Large screens (1024px+)
    1024: {
      itemsToShow: 4,
    },

    // Extra large (1280px+)
    1280: {
      itemsToShow: 5,
    },
  },
}


const testimonials = [
  {
    name: "Mrs. Adebayo",
    position: "Parent, Nursery Section",
    quote:
      "My child looks forward to school every day. The teachers are patient, caring, and truly understand how to nurture young learners."
  },
  {
    name: "Mr. Johnson",
    position: "Parent, Primary 3",
    quote:
      "The learning environment is clean, safe, and very supportive. My son's confidence and academic performance have improved greatly."
  },
  {
    name: "Mrs. Okafor",
    position: "Parent, Nursery 2",
    quote:
      "The school provides a wonderful balance between play and learning. My daughter has developed good communication and social skills."
  },
  {
    name: "Mr. Bello",
    position: "Parent, Primary 5",
    quote:
      "The teachers are dedicated and always keep parents informed. The school focuses on both academic excellence and good character."
  },
  {
    name: "Mrs. Ahmed",
    position: "Parent, Primary 1",
    quote:
      "I am impressed with how well the school supports early reading and numeracy. My child has made great progress in a short time."
  },
  {
    name: "Mr. Adekunle",
    position: "Parent, Nursery 1",
    quote:
      "The staff are friendly and professional. The school provides a warm, safe, and stimulating environment for young children."
  }
];

</script>