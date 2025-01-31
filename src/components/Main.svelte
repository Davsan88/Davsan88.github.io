<script>
    import { createEventDispatcher } from "svelte";
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Pokédex",
            icon: "/images/pokedex.png",
            type: "image",
            href: "https://your-pokedex-link.netlify.app/",
            description: `The Pokédex App is a <strong  class="text-violet-400">React-based</strong>
                        web application designed for exploring Pokémon data in an interactive way.
                        It features <strong class="text-violet-400">API integration, local caching</strong> for optimized performance, and a clean, responsive design.
                        Users can <strong class="text-violet-400">search, filter, and view</strong>
                        detailed Pokémon stats, abilities, and types, making it a dynamic and
                        engaging project that showcases <strong class="text-violet-400">advanced data fetching, state management,
                        and UI optimization techniques</strong>.
`,
        },
        {
            name: "Meme Generator",
            icon: "fa-solid fa-images",
            type: "fa",
            href: "https://meme-generator-davsan.netlify.app/",
            description: `The Meme Generator App is a <strong
                            class="text-violet-400">React-based</strong
                        >
                        web application designed for creating and customizing memes.
                        It features
                        <strong class="text-violet-400"
                            >dynamic state management, API integration</strong
                        >
                        to fetch meme data, and responsive design. Users can
                        <strong class="text-violet-400"
                            >generate random meme images</strong
                        > and overlay them with custom text, making it a fun and
                        interactive project that showcases core React skills.`,
        },
        {
            name: "Chef Enzo",
            icon: "/images/chef_enzo.png",
            type: "image",
            href: "https://chefenzo.netlify.app/",
            description: `The Chef Enzo App is a <strong class="text-violet-400"
                            >React-based</strong
                        >
                        web application designed for creating personalized recipe
                        suggestions. It features
                        <strong class="text-violet-400"
                            >API integration, serverless functions</strong
                        >, and a clean, responsive design. Users can input
                        ingredients they have on hand, and the app generates
                        detailed recipes
                        <strong class="text-violet-400"
                            >using AI-powered recommendations</strong
                        >, making it a practical and innovative project that
                        demonstrates modern web development skills.`,
        },
        {
            name: "Davnilla To-Do App",
            icon: "fa-solid fa-list-check",
            type: "fa",
            href: "https://davnilla-to-do-app.netlify.app/",
            description: `Davnilla To-Do is a <strong   class="text-violet-400">feature-rich, intuitive</   strong>
                        task management application built with 
                        <strong class="text-violet-400">HTML</strong>,
                        <strong class="text-violet-400">CSS</strong>,
                        and <strong class="text-violet-400">JavaScript</strong>. 
                        Designed for efficiency and flexibility, it enables users to 
                        <strong class="text-violet-400">create, update, delete, and                            persist</strong> tasks across sessions. 
                        With a sleek, responsive design and a built-in <strong class="text-violet-400">dark mode</strong>, 
                        Davnilla To-Do ensures an optimal user experience in any lighting condition.`,
        },
        {
            name: "Crystal Math",
            icon: "fa-solid fa-cart-shopping",
            type: "fa",
            href: "https://crystal-math-web.netlify.app/",
            description:
                "Crystal Math is a static and responsive webpage created with TailwindCSS and HTML for a classic Vanilla approach.",
        },
    ];

    let benefits = [
        {
            name: "a Self-Taught Developer Driven by Passion",
            description:
                "My transition into the world of software development is a testament to my passion for technology and continuous learning. Starting from scratch, I immersed myself in  HTML, CSS, JavaScript, React, and Python, utilizing free online resources and hands-on projects on GitHub. This self-driven journey has not only equipped me with technical skills but also ignited a deep appreciation for creative problem-solving. This relentless drive to learn and grow keeps me inspired and motivated to contribute to innovative tech projects.",
        },
        {
            name: "a Leader Who Values Effective Communication",
            description:
                "Throughout my career, I've discovered the importance of leadership and clear communication. Whether managing customer accounts at Envelopes Ltd or coordinating with stakeholders at Crowdcube, I have always prioritized building strong relationships and fostering a collaborative environment. My ability to communicate effectively has been key in leading teams, resolving conflicts, and ensuring everyone is on the same page. These experiences have shaped me into a leader who values transparency, empathy, and teamwork, qualities that I bring to every project and team I join.",
        },
        {
            name: "Passionate About Personal Growth and New Challenges",
            description:
                "I am driven by a relentless pursuit of personal and professional growth. From learning new programming languages to adapting to diverse roles across various industries, I thrive on challenges that push my boundaries. My journey from hospitality to tech is a reflection of my adaptability and eagerness to embrace new opportunities. Engaging in self-improvement activities, whether through technology, music, or sports, keeps me energized and curious. This passion for continuous growth and love for tackling new challenges defines my approach to both life and work.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="montserrat text-violet-400">David</span>
                Sanchez <br />Front-End
                <span class="montserrat text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="montserrat text-violet-400">favorite tech</span>
                includes JavaScript, ReactJS & TailwindCSS!
            </p>
            <a
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl montserrat relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer"
                href="https://www.linkedin.com/in/david-sanchez-1995ab268/"
                target="_blank"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profilePicture.png"}
                alt="Profile Picture"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>

    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="montserrat text-violet-400">see</span> my
                work?
            </h3>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-14 lg:gap-18">
            {#each steps as step}
                <a href={step.href} target="_blank">
                    <Step {step}>
                        {#if step.description}
                            <p>{@html step.description}</p>
                        {/if}
                    </Step>
                </a>
            {/each}
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="montserrat text-violet-400">about</span> me.
            </h3>
        </div>
        <p
            class="mx-auto montserrat font-semibold text-lg sm:text-xl md:text-2xl"
        >
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto maz-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="montserrat text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-4xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class="text-2xl sm:text-3xl font-semibold text-center montserrat">
            The <span class="text-violet-400 montserrat">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="whitespace-nowrap bg-violet-700 text-white p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Critical Thinking</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">
            Ready to embrace the <span class="text-violet-400 montserrat"
                >future</span
            >?
        </p>
    </section>
</main>
