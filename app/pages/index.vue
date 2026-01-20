<template>
  <div class=" overflow-x-hidden bg-[#FEFEFE]">
    
    <!-- <UiTypographyH1 color="secondary" class="text-center pt-28 mb-1">United States</UiTypographyH1> -->
    <header class="mt-0 h-[100vh] pt-1 hero-section">
      <Container :addTopBottomPadding="false" class="text-white h-full flex sm:items-end items-center pb-4">
        <div class="lg:w-[70%] md:w-4/5 w-full h-fit">

          <div class="space-y- py-2">
            <UiTypographyP color="white" class="font-bold hero-fade-up delay-1">
              <span class=" text-secondary text-3xl -">Welcome to</span>
            </UiTypographyP>

            <div class=" bg-primary/50 left-0 lg:w-[70%] md:w-4/5  mr-7 z-10 absolute flex j items-center  w-full h-24">
             
            </div>
             <div class="  relative z-10      flex j items-center  w-full h-24">
              <p class=" text-white    px-2 lg:text-4xl md:text-3xl text-xl sm:text-2xl">
               UNILORIN  NURSERY  AND  PRIMARY  SCHOOL
              </p>
            </div>

            <UiTypographyH1 class="font-bold2 hero-fade-up hidden delay-2" color="white">
             World Class Elementary Education For your Child
            </UiTypographyH1>
          </div>

          <UiTypographyP color="white" class="hero-fade-up delay-3">
           At UNILORIN Nursery And Primary School, we don’t just teach – we inspire. With a British Nigerian curriculum, state-of-the-art facilities, and passionate educators, your child’s future starts here.
          </UiTypographyP>

          <div class=" mt-4 h-1 w-1/3 bg-primary"> </div>
           <UiTypographyH3 class=" pt-4 text-white"> Ambience. Love. Content</UiTypographyH3>
          <div class="pt-4 sm:flex block sm:space-y-0 space-y-4 sm:space-x-4 hero-fade-up delay-4">
            <UiButtonsPrimary @click="openform">
              <span>Apply Now</span>
            </UiButtonsPrimary>

           
          </div>

        </div>
      </Container>
    </header>



    <section class="mt-5">
      <div class="text-center md:container w-[90%]  mx-auto">
      
       <div class="grid-cols-2 block md:space-y-0 space-y-3 md:grid gap-4">
        <FlipCard
          title="NURSERY SCHOOL"
          description="Our nursery school is designed to equip your child with learning fundamentals. With a sufficient blend of Montessori and play, we lay a strong foundation on which your child's education will bloom"
          frontBg="#250372"
          backBg="#b78d46"
        
        />
        <FlipCard
          title="PRIMARY SCHOOL"
          description="The importance of primary education can not be overemphasized. This is why we have a robust curriculum for your child. We pay attention to your child's cognitive needs, values and develop their physical abilities."
          frontBg="#b78d46"
          backBg="#250372"
          frontTextColor="#FFFFFF"
          backTextColor="#FFFFFF"
        />
       

       </div>

       
      

      </div>
    </section>
    <!-- hidden this section (what are will do) -->
   


    <!-- Simple Process Steps  details here -->
    <section class="   bg-gray-100/50 reason-choose-us ">
      <Container>
        <div class="  lg:flex gap-5 ">
         

          <div class=" lg:w-1/2 w-full space-y-3 r">
           
           
            <UiTypographyH2 class=" mb-6">
              <span class="text-3xl leading-snug font-bold">
                ABOUT US
              </span>
            </UiTypographyH2>
             <div>
              <UiTypographyH3><span class="font-semibold">Our Vision</span></UiTypographyH3>
               <p class=" text-md text-justify md:text-lg text-gray-700">
           To challenge and inspire every child to reach their full potential in a caring and loving environment.
           </p> 
           

            </div>

             <div>
              <UiTypographyH3><span class="font-semibold">Our Mission </span></UiTypographyH3>
           
           <p class=" text-md text-justify md:text-lg text-gray-700">
            To ensure that 
             UNILORIN Nursery And Primary School pupils adapt and contribute to the ever changing world as well as engage in continuous life long learning by providing a balanced curriculum designed to meet the academic, cultural and social needs of children from diverse backgrounds in our community.
           </p> 
            
           
             <UiButtonsPrimary class="mt-6" @click="openform">
           Read More
          </UiButtonsPrimary>

            </div>

           
           
            
          </div>

           <div class=" hidden w-[50%]  w lg:block">
            <img src="@/assets/images/1-Design-2.png" class="" alt="Simple Process Steps" srcset="">
          </div>

        </div>
      </Container>
    </section>


   

    <section class=" bg-[url('@/assets/images/unilorin1.jpg')] bg-fixed bg-no-repeat bg-cover" id="pricing">
      <Container>
        <div class=" mx-auto">
       
          <div class="  lg:flex justify-center items-center gap-5 ">
         
            <div class="  sm:w-[50%] w-full flex justify-center items-center mb-2  w lg:block">
            <img src="@/assets/images/professionor.jpg" class="  w-[70%] rounded-full" alt="Simple Process Steps" srcset="">
          </div>
          <div class=" lg:w-[70%] text-white bg-primary p-4 w-full space-y-3 r">
           
           
            <UiTypographyP>
             Dear Parent,
            </UiTypographyP>
             <div>
             
         <p class=" text-justify">  It is my pleasure to welcome you to Bowine International School, 
           where every child counts. As a school, we believe that each child
            is a masterpiece and as such, we are committed to bringing the
             dreams of every child to reality. One of the many ways we hope to achieve this
              is by offering the children a wide variety of opportunities in terms
               of curriculum and extracurricular activities. This places value on 
               the importance of raising the total child who will influence his environment 
               and the world at large.
              <br> <br>
               Our facilities are world class and our balanced curriculum is aimed at producing
                internationally minded citizens who will be relevant in the 21st century and beyond.
                 We have a team of experienced, highly qualified and passionate professionals who will make
                  unforgettable impact in the education of each child through the use of technology, inquiry
                   based and hands-on learning to enable them maximize their potential. In addition, we strongly inculcate high moral and ethical standards, good habits and positive attitude in our children.
             <br> <br>
              We enjoin you to partner with us as a parent, as we promise value for the investment you are making
               on the children. Trust us, this is the beginning of the journey
                of “Winning together” in our 7 STAR school.
           </p> 
           

           
            
         
            
           
             
            </div>

           
           
            
          </div>

           

        </div>
          
         


        </div>

      </Container>
    </section>

    <section class=" overflow-hidden  reason-choose-us ">
      <Container>
        <div class=" h-fit   gap-5 ">
           <UiTypographyH2 small_text class="flex  items-center justify-center gap-2 mb-9 uppercase">
              <span class="h-1 aspect-square rounded-full text-center bg-secondary" v-for="i in 2"></span>
            WHY CHOOSE BOWINE?

              <span class="h-1 aspect-square rounded-full bg-secondary" v-for="i in 2"></span>
            </UiTypographyH2>

     

          <Card  class="  "></Card>
          <Card 
          heading="TOP NOTCH ACADEMICS"
          description="Parents are amazed at the quality of content that their children are exposed to. We ensure that children can compete with their peers anywhere around the world."
          bg="#b78d46"
          image="image4.jpg"
           class="  "
           ></Card>
           <Card 
          heading="GREAT STAFF"
          description="Our amazing team of highly qualified, dedicated and passionate professionals are committed to giving your child the best learning experience."
          bg="#250372"
          image="image1.jpg"
           class="  "
           ></Card>
            <Card 
          heading="SPORTS"
          description="With activities like swimming, football, basketball and athletics incorporated into the curriculum, the physical development of your child is guaranteed."
          bg="#b78d46"
          image="image2.jpg"
           class="  "
           ></Card>
           <Card 
          heading="TECHNOLOGY"
          description="We provide an  ultra modern ICT Lab and integrate technology into the learning experiences of pupils. We are a Microsoft Showcase School (Incubator). "
          bg="#250372"
          image="image3.jpg"
           class="  "
           ></Card>
        </div>
      </Container>
    </section>


    <section class=" bg-primary ">
    <Container class="  ">
       <UiTypographyH2 small_text class="flex  text-white  items-center justify-center gap-2 mb-9 uppercase">
              <span class="h-1 text-white aspect-square rounded-full text-center bg-secondary" v-for="i in 2"></span>
            GALLARY

              <span class="h-1 aspect-square rounded-full bg-secondary" v-for="i in 2"></span>
            </UiTypographyH2>
            <div class=" grid grid-cols-2 md:grid-cols-4 gap-4 ">
               <div v-for="(item, index) in 12" :key="index" class="">
                <img  :src="`/images/gallary${index}.jpg`" class="" alt=""  />
               </div>
            </div>
          

    </Container>
 </section>


    <section class="bg-neutral-100 " id="faqs">
      <Container>
        <UiTypographyH2 small_text class="flex    items-center justify-center gap-2 mb-9 uppercase">
              <span class="h-1  aspect-square rounded-full text-center bg-secondary" v-for="i in 2"></span>
           TESTIMONIALS FROM BOWINE PARENTS

              <span class="h-1 aspect-square rounded-full bg-secondary" v-for="i in 2"></span>
            </UiTypographyH2>

          <Testimonials class=" "></Testimonials>

   



          

        
      </Container>
    </section>

    <section class=" bg-primary">
      <Container class="sm:text-center text-left  text-white">
       <UiTypographyH2 small_text class="flex  text-white   items-center justify-center gap-2 mb-9 uppercase">
              <span class="h-1  aspect-square  rounded-full text-center bg-secondary" v-for="i in 2"></span>
          Partners & Accreditation

              <span class="h-1 aspect-square rounded-full bg-secondary" v-for="i in 2"></span>
            </UiTypographyH2>
       <div class="flex justify-center items-center"> 
        <div v-for="(item, index) in 5" :key="index"  class=" flex  ">
           <img   :src="`/images/partner${index}.png`" class=" w-40" alt=""  />
        </div>
        </div>
      </Container>
    </section>

        <section class=" ">
      <Container class="sm:text-center text-left  ">
       <UiTypographyH2 small_text class="flex    items-center justify-center gap-2 mb-9 uppercase">
              <span class="h-1  aspect-square  rounded-full text-center bg-secondary" v-for="i in 2"></span>
         How to find us

              <span class="h-1 aspect-square rounded-full bg-secondary" v-for="i in 2"></span>
            </UiTypographyH2>
       <div class=""> 
         <div class="w-full h-full bg-amber-600 ">
            <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d505105.7485473196!2d4.674583!3d8.485896!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103652c2a85b742f%3A0xbf3011af9f61d6ca!2sUniversity%20of%20Ilorin!5e0!3m2!1sen!2sus!4v1768692138792!5m2!1sen!2sus" width="100%" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
          </div>

        </div>
      </Container>
    </section>
  </div>
</template>

<script setup>
import { useRouter } from 'vue-router'
import Button from '~/components/Form/Button.vue'

const config = useRuntimeConfig()
const projectName = config.public.projectName
const router = useRouter()

const openChat = () => {

}
const openform = () => {
  
  
  router.push('/warning')
}

const stepToTakeList = ref([
  {
    id: 1,
    title: 'Send Us Your Info',
    description: 'Share your business name, logo, and basic details using our secure online form.',
  },
  {
    id: 2,
    title: 'We Do the Filing for You',
    description: 'Our team checks for similar trademarks, prepares your application, and files it with the USPTO.',
  },
  {
    id: 3,
    title: 'Receive Your Trademark',
    description: 'After approval, your trademark gets officially registered and protected across the country.',
    image: 'ongoing-icon.png'
  }
])

const prices = ref([
  {
    package: 'Basic',
    description: 'Best for startups needing protection in one trademark class with simple requirements.',
    price: '$45',
    list: [
      'Case Review',
      'Case', 'Basic Search', 'State E-Filing', 'Trademark Secured', '*(Govt. filing fee not included)']
  },
  {
    package: 'Standard',
    description: 'Great for small businesses covering multiple product or service classes.',
    price: '$149',
    list: [
      'Case Review',
      'Case', 'Basic Search', 'Direct Hit Search', 'Trademark Alerts', 'Trademark Secured', 'High Satisfaction Rate', 'Refusal Risk Meter', '*(Govt. filing fee not included)']
  },
  {
    package: 'Deluxe',
    description: 'For brands needing extra support, including help with USPTO office actions.',
    price: '$299',
    list: [
      'Case Review',
      'Case', 'Basic Search', 'Direct Hit Search', 'Trademark Alerts', 'Trademark Secured', 'High Satisfaction Rate', 'Refusal Risk Meter', 'Trademark Monitoring', 'Complete Documentation', 'Digital File', 'Dedicated Case Manager', '*(Govt. filing fee not included)']
  },

])
</script>

<style>
header {
  background: linear-gradient(rgba(31, 31, 31, 0.838), rgba(41, 41, 41, 0.7)), url('/images/unilorin_gate.jpg');
  background-blend-mode: multiply;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}



.cta {
  background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('/images/unilorin_gate.jpg');
  background-blend-mode: multiply;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: top;
}

.custom-scroll::-webkit-scrollbar {
  width: 6px;
}

.custom-scroll::-webkit-scrollbar-track {
  background: #f1f1f1;
  border-radius: 10px;
}

.custom-scroll::-webkit-scrollbar-thumb {
  background: #b78d46;
  border-radius: 10px;
}

.custom-scroll::-webkit-scrollbar-thumb:hover {
  background: #9e7636;
}
</style>