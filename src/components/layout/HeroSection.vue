<template>
    <section id="Home" class="relative min-h-100 py-25 p-15">
        <!-- Gradient kiri (mobile-friendly) -->
        <div class="absolute w-1/2 aspect-[16/5] -skew-x-12 rounded-full 
    bg-gradient-to-r from-[#183D3D] via-[#5C8374] to-secondary 
    opacity-30 blur-[100px] left-10 top-0 block">
        </div>

        <!-- Gradient kanan (mobile-friendly) -->
        <div class="absolute w-1/2 aspect-[16/5] skew-x-12 rounded-full 
    bg-gradient-to-l from-[#183D3D] via-[#5C8374] to-secondary 
    opacity-30 blur-[100px] right-10 bottom-0 block">
        </div>

        <main
            class="relative z-10 flex flex-col-reverse md:flex-row md:justify-center md:space-x-20 items-center justify-between">
            <!-- Teks Hero -->
            <header class="text-center md:text-left max-w-xl space-y-6 text-white/70 mt-20 md:mt-0"
                data-aos="fade-right">
                <h1 class="text-3xl md:text-5xl font-bold leading-tight">
                    👋 Hi, I'm <span class="text-secondary">Qadri</span><br />
                    IT Professional
                </h1>
                <p class="text-lg">
                    I'm a passionate and professional IT service provider with experience in web development, software
                    programming, IoT solutions, and more. I help clients build modern, responsive, and efficient digital
                    products tailored to their needs.
                </p>

                <div class="flex justify-center md:justify-start gap-4">
                    <ButtonBase label="View Projects" variant="secondary" />
                </div>
            </header>

            <!-- Gambar Hero -->
            <figure class="w-80 h-80 border-r-20 border-primary rounded-full overflow-hidden shadow-lg md:mt-20"
                data-aos="fade-right">
                <img :src="profile" alt="Profile" class="w-full h-full object-cover" />
            </figure>
        </main>
    </section>
</template>

<script setup>
import profile from "../../assets/profile.jpg"
import ButtonBase from '../ui/Button.vue'
</script>