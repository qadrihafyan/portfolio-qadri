<template>
  <footer id="Contact"
    class="text-white py-16 px-6 text-center bg-white/5 backdrop-blur-sm mt-20 relative overflow-hidden">
    
    <!-- Background gradient blur kiri -->
    <div class="absolute w-2/3 aspect-[16/5] -skew-x-12 rounded-full 
        bg-gradient-to-r from-[#183D3D] via-[#5C8374] to-secondary 
        opacity-20 blur-[100px] left-0 top-0 -z-10">
    </div>

    <!-- Background gradient blur kanan -->
    <div class="absolute w-2/3 aspect-[16/5] skew-x-12 rounded-full 
        bg-gradient-to-l from-[#183D3D] via-[#5C8374] to-secondary 
        opacity-20 blur-[100px] right-0 bottom-0 -z-10">
    </div>

    <!-- Title -->
    <h2 class="text-3xl md:text-4xl font-bold text-secondary mb-3">Contact Me</h2>
    <p class="text-white/70 mb-8 max-w-3xl mx-auto leading-relaxed">
      I am an enthusiastic Frontend Developer focused on creating modern, clean, and interactive user interfaces
      using technologies like Vue and React. Additionally, I have a keen interest in IoT, automation, and digital
      design, and enjoy exploring new technologies to create practical and impactful solutions. Ready to
      collaborate on projects that make a difference.
    </p>

    <!-- Info Grid -->
    <div class="grid md:grid-cols-3 md:text-center gap-8 text-sm text-white/80 mb-10 max-w-4xl mx-auto text-left">
      <div>
        <h3 class="text-secondary font-semibold mb-2">Address</h3>
        <p>Jl. Pahlawan Kerja<br>Pekanbaru, Riau<br>Indonesia</p>
      </div>
      <div>
        <h3 class="text-secondary font-semibold mb-2">Contact</h3>
        <p>Email: qadrihafyan03@gmail.com<br>Phone: +62 812-9262-3426</p>
      </div>
      <div>
        <h3 class="text-secondary font-semibold mb-2">Working Hours</h3>
        <p>Monday – Friday: 09:00 – 17:00<br>Saturday: 10:00 – 14:00<br>Sunday: Closed</p>
      </div>
    </div>

    <!-- Social Icons -->
    <div class="flex justify-center gap-8 text-2xl mb-10">
      <a href="https://wa.me/6281292623426" target="_blank"
        class="hover:text-[#25D366] transition transform hover:scale-110">
        <i class="fab fa-whatsapp"></i>
      </a>
      <a href="https://github.com/qadrihafyan" target="_blank"
        class="hover:text-gray-300 transition transform hover:scale-110">
        <i class="fab fa-github"></i>
      </a>
      <a href="https://instagram.com/qadrihafyann" target="_blank"
        class="hover:text-pink-500 transition transform hover:scale-110">
        <i class="fab fa-instagram"></i>
      </a>
    </div>

    <!-- Copyright -->
    <p class="text-xs text-white/40">
      &copy; {{ new Date().getFullYear() }} Qadri Hafyan Ramadhan. All rights reserved.
    </p>
  </footer>
</template>

<style scoped>
a {
  touch-action: manipulation;
}
</style>
