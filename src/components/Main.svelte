<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Image Gallery Project",
            icon: "fa-solid fa-list-check",
            description:
                "Since pandemic started I came up to love online shopping up until now,especially there are so many online shops.",
        },
        {
            name: "KanBan Project",
            icon: "fa-solid fa-list-check",
            description:
                "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
        },
        {
            name: "Flight Booking System",
            icon: "fa-solid fa-list-check",
            description:
                "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "as a dog lover",
            description:
        "As a dog lover,I gain a wide range of emotional, physical, and social benefits from my bond with dogs.Unconditional Love and Companionship.Dogs remind you to appreciate the present. Their joy in simple things—like a belly rub or chasing a ball—teaches you the value of living in the moment and finding happiness in everyday experiences. ",
        },
        {
            name: "a Struggling student in Major Subjects",
            description:
                "I'm also a student who struggles when it comes to major subjects but can handle it for the dream, it has a huge impact on me that I have classmates who help me understand the things that I struggle with when it comes to studying..",
        },
        {
            name: "a Girl with a Dream",
            description:
"A young girl stands on the edge of possibility, her eyes bright with ambition and hope. She dreams of a future where she breaks barriers, explores new worlds, and makes her mark. With determination in her heart and a spark of creativity in her soul, she knows that no matter how far away her dreams may seem, every step forward brings her closer to making them a reality.",
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
                Hi! I'm <span class="poppins text-violet-400">Casey</span> Nojadera
                <br />A BSCS 
                <span class="poppins text-violet-400">College student.</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                I am  <span class="text-violet-400"> currently a 3rd Year College student.</span> I hope I can be successful someday!
            </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/njdra.png"}
                alt="casey"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
        <!-- <div  class="flex p-0.5 relative max-w-[700px] w-full mx-auto">
            <div
                class="absolute inset-0 overflow-hidden rounded-md flex items-center justify-center"
            >
                <div
                    class="bg-gradient-to-r absolute inset-[-20px]  from-violet-800 to-indigo-800 specialSpin"
                />
            </div>

            <img
                src={"images/njdra.png"}
                alt="casey"
                class="w-full h-full object-cover z-[2]"
            />
        </div> -->
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative works.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href="https://youtu.be/ZiewIylF0f4?si=7ZY-o3MUCeZEozBX"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    ''Design an interface to display image thumbnails and allow users to view full size images. Implement functionality for image uploads. Consider incorporating functionalities like image editing and user comments.'' <strong
                        class="text-violet-400"
                        ></strong
                    > 
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    ''An interface design with columns representing stages in workflow (To Do, In progress, Done) implement drag and drop functionality to move task between columns. Considering adding functionalities like editing task details and due dates.''<strong
                        class="text-violet-400"></strong
                    >
                    <strong class="text-violet-400"></strong
                    >
                     <strong class="text-violet-400"></strong>
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    A Flight Booking System is a software that allows users to search, book, and manage airline tickets. It enables customers to browse flights, compare prices, choose seats, and securely pay. Key features include user registration, real-time flight availability, booking confirmations, and itinerary management. For airline staff, it offers tools to manage schedules, track bookings, and handle cancellations. The system aims to simplify booking, improve customer convenience, and boost airline efficiency. <strong class="text-violet-400"
                        ></strong
                    >
                    
                    <strong class="text-violet-400"></strong>, 
                    <strong class="text-violet-400"></strong>
                    
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            CASEY <span class="text-violet-400">NOJADERA</span> PORFOLIO
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">Thats All!</p>
    </section>
</main>