<template>
    <div class=" bg-primary">
        <!-- Hero section contact us -->
        <section class=" bg-[url('/images/4T2A1567.png')] bg-cover bg-no-repeat  ">
            <div class="bg-black/70 pb-10 pt-20 ">
                <Container class="">
                    <div class="md:w-1/2 text-white">
                       
                        <div class=" py-2">
                            <UiTypographyH1 color="white">
                                <span class="  font-bold">Vision and Mission</span>
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
                   <div class=" bg-[url(@/assets/images/0003.png)] w-full mb-4  bg-center bg-cover h-96" ></div>
                   <h2 class="  text-primary  font-bold text-4xl">Vision and Mission</h2>
                   <div class=" bg-secondary  w-1/3 h-1  mt-6"> </div>
                   
                   <div class=" mt-10">
                    <UiTypographyH3> <span class=" underline">Our Vision</span></UiTypographyH3>
                    <UiTypographyP class="mt-4 w-full tracking-wide md:w-3/5">To challenge and inspire every child to reach their full potential in a caring and loving environment.</UiTypographyP>
                   </div>
                   
                   <div class=" mt-10">
                    <UiTypographyH3> <span class=" underline">Our Mission</span></UiTypographyH3>
                    <UiTypographyP class="mt-4 w-full tracking-wide md:w-3/5">To ensure that  UNILORIN nursery and primary school pupils adapt and contribute to the ever changing world as well as engage in continuous life long learning by providing a balanced curriculum designed to meet the academic, cultural and social needs of children from diverse backgrounds in our community.</UiTypographyP>
                   </div>

                   
                   <div class=" mt-10">
                    <UiTypographyH3> <span class=" underline">Our Core Values</span></UiTypographyH3>
                    <UiTypographyP class="mt-4 w-full tracking-wide md:w-3/5">
                        <ul class="list-disc list-inside space-y-1">
                            <li>Excellence</li>
                            <li>Integrity</li>
                            <li>Respect</li>
                            <li>Creativity</li>
                            <li>Collaboration</li>
                            <li>Empathy</li>
                            <li>Resilience</li>
                        </ul>
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

        <section>

            

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
</script>
