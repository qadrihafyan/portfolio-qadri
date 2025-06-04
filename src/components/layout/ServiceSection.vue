<script setup>
import ServiceCard from '../ui/ServiceCard.vue'
import web from '../../assets/icon/web.svg'
import mobile from '../../assets/icon/mobile.svg'
import iot from '../../assets/icon/iot.svg'
import program from '../../assets/icon/program.svg'
import consult from '../../assets/icon/consult.svg'
import design from '../../assets/icon/design.svg'

const services = [
    {
        icon: web,
        title: 'Web Development',
        description: 'Building modern and responsive websites using Vue, Tailwind, and other frameworks.',
    },
    {
        icon: mobile,
        title: 'Mobile App UI',
        description: 'Mobile interface design using a user-centric approach and interactive layouts.',
    },
    {
        icon: iot,
        title: 'IoT & Automation',
        description: 'Development of IoT solutions based on ESP/Arduino and intelligent automation systems.',
    },
    {
        icon: program,
        title: 'Programming & Software',
        description: 'Development of software and tools based on desktop, CLI, and other utility applications.',
    },
    {
        icon: consult,
        title: 'IT Consulting',
        description: 'Providing technical solutions and advice for system development, troubleshooting, and technology planning.',
    },
    {
        icon: design,
        title: 'UI/UX & Design',
        description: 'Designing intuitive user interfaces and efficiently integrating designs into frontend systems.',
    }



]
</script>

<template>
    <section id="Service" class="relative py-25 px-4 max-w-6xl mx-auto min-h-screen">
        <!-- Background gradient -->
        <div class="absolute w-1/2 aspect-[16/5] -skew-x-12 rounded-full 
      bg-gradient-to-r from-primary via-secondary to-primary 
      opacity-20 blur-[100px] left-10 top-0 block">
        </div>
        <div class="absolute w-1/2 aspect-[16/5] skew-x-12 rounded-full 
      bg-gradient-to-l from-primary via-secondary to-primary 
      opacity-20 blur-[100px] right-10 bottom-0 block">
        </div>

        <div class="relative">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-secondary mb-10" data-aos="fade-down"> Services</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
                <ServiceCard v-for="(service, i) in services" :key="i" :icon="service.icon" :title="service.title"
                    :description="service.description" />
            </div>
        </div>
    </section>
</template>
