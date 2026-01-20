<template>
    <div class=" bg-primary">
        <!-- Hero section contact us -->
        <section class=" bg-[url('/images/gallary6.jpg')]  bg-cover bg-no-repeat bg-center  ">
            <div class="bg-black/70 pb-10 pt-20 ">
                <Container class="">
                    <div class="md:w-1/2 text-white">
                       <!-- <img src="@/assets/images/4T2A1549.png" alt="4T2A1549" srcset=""> -->
                        <div class=" py-2">
                            <UiTypographyH1 color="white">
                                <span class="  font-bold">Library</span>
                            </UiTypographyH1>
                        </div>
                       
                       

                    </div>
                </Container>
            </div>

        </section>

        <!-- List all the contact details here -->
        <section class=" ">
            <Container>
                <div
                    class=" bg-white md:p-10 p-2 ">
                   <div class=" bg-[url(/images/gallary8.jpg)] w-full mb-4  bg-center bg-cover h-96" ></div>
                   <h2 class="  text-primary  font-bold text-2xl md:text-4xl">Library</h2>
                   <div class=" bg-secondary  w-1/3 h-1  mt-6"> </div>
                   
                   <div class=" mt-10">
                   
                    <UiTypographyP class="mt-4 w-full tracking-wide md:text-lg ">One of our focus areas is imbibing 
                        a reading culture in our children. To achieve this, we have a state of the art 
                        library where pupils can go to have personal study time, with an amazing range 
                        of books to aid study. <br> <br>
                        Our library is completely digitalized, and equipped with computers to allow for internet research for our older pupils. <br> <br>
                        Additionally, each classroom is loaded with interesting and age appropriate books that aid learning.
                        
                        </UiTypographyP>
                   </div>
                   
                 
                   
                 

                 

                   
                  
                   
                    

                   
                   


                   
                  


                   <div class=" mt-10  p-10  flex flex-col justify-center items-center text-white w-full  bg-primary p">
                        <UiTypographyH2 class=" text-white text-center">Enrol your child today</UiTypographyH2>
                       <div class=" h-0.5 w-20  mb-7 mt-3 bg-white"> </div> 

                        <NuxtLink to="/warning" class=" bg-white px-4 rounded-full py-2 cursor-pointer  font-medium hover:bg-secondary hover:text-white duration-300 text-black ">Apply Now</NuxtLink>
                   </div>
                 </div>
            </Container>
        </section>

        


    </div>
</template>

<script setup>
import { ref } from 'vue'
import { useFormStore } from '@/stores/formStore'
import { useRouter } from 'vue-router'

const formStore = useFormStore()
const form = formStore.form
const isLoading = ref(false)
const router = useRouter()

// SAVE FORM ON SUBMIT
const submit = async (e) => {
    e.preventDefault()
    isLoading.value = true
    // Simple contact form: Save data and redirect to forms
    formStore.setFormData({
        fullname: form.value.fullname,
        email: form.value.email,
        phone: form.value.phone,
        message: form.value.message
    })

    setTimeout(() => {
        router.push('/forms')
        isLoading.value = false
    }, 500)
}

const openChat = () => {
    if (window.Tawk_API) {
        window.Tawk_API.maximize();
    }
}
const faqList = ref([
    {
        id: 1,
        title: 'Q1: What is a trademark, and why is it important?',
        description: 'A trademark protects your brand name, logo, or slogan from unauthorized use. It secures your business identity and strengthens customer trust.',
        showdescription: false
    },
    {
        id: 2,
        title: 'Q2: Can I register a trademark in multiple classes?',
        description: 'Yes. You can file a trademark across multiple classes. Our Standard, Deluxe, and Platinum plans support multi-class applications with additional services.',
        showdescription: false
    },
    {
        id: 3,
        title: 'Q3: Do you handle the full trademark registration process?',
        description: 'Absolutely. We take care of everything — from conducting a trademark search to filing your application and managing all USPTO correspondence.',
        showdescription: false
    },
    {
        id: 4,
        title: 'Q4: What are USPTO fees, and are they included in your pricing?',
        description: 'USPTO filing fees are government charges set by the United States Patent and Trademark Office and vary by class. These fees are not included in our service pricing and are paid directly to the USPTO.',
        showdescription: false
    }
])

const toggleDescription = (item) => {
    faqList.value.forEach(faq => {
        if (faq.id !== item.id) {
            faq.showdescription = false     // close all others
        }
    })
    item.showdescription = !item.showdescription
}
</script>
