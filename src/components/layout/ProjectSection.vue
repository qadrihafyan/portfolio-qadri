<script setup>
import ProjectCard from '../ui/ProjectCard.vue'
import project1 from '../../assets/project1.png'
import project2 from '../../assets/project2.png'
import project3 from '../../assets/project3.png'
import project4 from '../../assets/project4.png'
import project5 from '../../assets/project5.png'
import project6 from '../../assets/project6.png'

const projects = [
  {
    icon: project1,
    title: 'HTML & CSS',
    link: 'https://github.com/qadrihafyan/management-keuangan',
    description: 'Semantic, responsive, and modern layout using clean HTML structure and well-organized CSS styling techniques. Ensures accessibility and cross-device compatibility.',
  },
  {
    icon: project2,
    title: 'Vue.js',
    link: 'https://github.com/qadrihafyan/to-doList',
    description: 'SPA and modular components using Vue. Features reactive data binding, component reusability, and clean structure for maintainable web apps.',
  },
  {
    icon: project3,
    title: 'Tailwind CSS',
    link: 'https://github.com/qadrihafyan/32-pbk-uts-233510651',
    description: 'Utility-first CSS for fast and consistent design. Enables rapid UI building with low-level utility classes while maintaining design consistency.',
  },
  {
    icon: project4,
    title: 'JavaScript',
    link: 'https://github.com/qadrihafyan/js-ecommers',
    description: 'Interactivity and logic of web applications. Handles DOM manipulation, form validation, and dynamic content rendering for better user experiences.',
  },
  {
    icon: project5,
    title: 'IoT Programming',
    link: 'https://www.tinkercad.com/things/gKdn9tf6RjP-pintu-otomatis?sharecode=HdgDK2MSkCvBSEgn_r2oagrsiKvOpXerl9kzIJdpxzA',
    description: 'Smart device development with ESP & Arduino. Includes sensor integration, basic automation logic, and real-time response using microcontroller programming.',
  },
  {
    icon: project6,
    title: 'Python',
    link: 'https://github.com/qadrihafyan/algorithm-lr',
    description: 'Scripting and automation from simple to complex. Covers data processing, algorithm design, and small utility scripts for real-world tasks.',
  },
]

</script>

<template>
    <section id="Project" class="relative py-25 px-4 sm:px-6 lg:px-8 max-w-6xl mx-auto min-h-screen">
        <div class="absolute w-1/2 aspect-[16/5] -skew-x-12 rounded-full 
      bg-gradient-to-r from-primary via-[#5C8374] to-secondary 
      opacity-20 dark:opacity-10 blur-[120px] left-10 top-0"></div>

        <div class="absolute w-1/2 aspect-[16/5] skew-x-12 rounded-full 
      bg-gradient-to-l from-primary via-[#5C8374] to-secondary 
      opacity-20 dark:opacity-10 blur-[120px] right-10 bottom-0"></div>

        <!-- Konten Utama -->
        <div class="relative z-10">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-secondary mb-12" data-aos="fade-down">
                Project
            </h2>

            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8">
                <ProjectCard v-for="(project, index) in projects" :key="index" :icon="project.icon"
                    :title="project.title" :description="project.description" :codeLink="project.link" data-aos="fade-right" />
            </div>
        </div>
    </section>
</template>
