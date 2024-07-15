<script>
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="bg-white grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="bg-green-500 flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="montserrat text-violet-400">David</span>
                Sanchez <br />Software
                <span class="montserrat text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="montserrat text-violet-400">favorite tech</span> includes JavaScript, TailwindCSS & Python!                
            </p>
            <a 
            class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl montserrat relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" 
            href="https://www.linkedin.com/in/david-sanchez-1995ab268/" target="_blank">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"/>
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a> 
        </div>
        <div class="bg-orange-600 relative shadow-2xl grid place-items-center">
            <img src={"images/profilePicture.png"} alt="Profile Picture" class="object-cover z-[2] max-h-[70vh]"/>
        </div>
    </section>
    
    
    
    <section id="projects" class="bg-blue-400 py-20 lg:py-32 flex flex-col gap-24">
        <div class="bg-pink flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="montserrat text-violet-400">see</span> my work?
            </h3>
            <a href="" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
                <i class="fa-regular fa-circle-play"></i>
                <p>Watch the video</p>
            </a>
        </div>


    </section>
</main>
