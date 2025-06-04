<script setup>
import SkillIcon from '../ui/SkillIcon.vue'
import html from '../../assets/icon/html.svg'
import css from '../../assets/icon/css.svg'
import js from '../../assets/icon/javascript.svg'
import vue from '../../assets/icon/vue.svg'
import react from '../../assets/icon/react.svg'
import python from '../../assets/icon/python.svg'
import java from '../../assets/icon/java.svg'
import git from '../../assets/icon/git.svg'
import tailwind from '../../assets/icon/tailwind.svg'
import c from '../../assets/icon/c.svg'
const skills = [
    { icon: html, label: 'HTML' },
    { icon: css, label: 'CSS' },
    { icon: js, label: 'JavaScript' },
    { icon: vue, label: 'Vue.js' },
    { icon: react, label: 'React' },
    { icon: python, label: 'Python' },
    { icon: java, label: 'Java' },
    { icon: git, label: 'Git' },
    { icon: tailwind, label: 'Tailwind' },
    { icon: c, label: 'C++' },
]
</script>

<template>
    <section id="Skill" class="relative py-25 px-4 max-w-6xl mx-auto min-h-screen">
        <div class="absolute w-1/2 aspect-[16/5] -skew-x-12 rounded-full 
      bg-gradient-to-r from-[#183D3D] via-[#5C8374] to-secondary 
      opacity-30 blur-[100px] left-10 top-0 block"></div>

        <div class="absolute w-1/2 aspect-[16/5] skew-x-12 rounded-full 
      bg-gradient-to-l from-[#183D3D] via-[#5C8374] to-secondary 
      opacity-30 blur-[100px] right-10 bottom-0 block"></div>

        <div class="relative z-10">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-secondary mb-10" data-aos="fade-down">
                My Skill
            </h2>
            <div class="grid grid-cols-3 sm:grid-cols-4 md:grid-cols-5 gap-6 place-items-center">
                <SkillIcon v-for="(skill, index) in skills" :key="index" :icon="skill.icon" :label="skill.label" class="mt-10" data-aos="fade-right"/>
            </div>
        </div>
    </section>
</template>
