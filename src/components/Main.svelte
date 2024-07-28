<script>
    import Step from './Step.svelte';

    let steps = [
        {name: 'Sales Coach AI', icon: 'fa-brands fa-rocketchat', imageUrl: '/images/sales-coach-ai.png'}, 
        {name: 'PGA Tour Statistics', icon: 'fa-solid fa-chart-line', imageUrl: '/images/golfer-ai.png'}, 
        {name: 'Marketing Data LLM', icon: 'fa-solid fa-table', imageUrl: '/images/marketing-llm.png'}, 
        {name: 'Tomato Classification', icon: 'fa-solid fa-magnifying-glass', imageUrl: '/images/tomato-classification.png'}, 
    ];

    let benefits = [
        {name: "a self taught developer", description: "I taught myself to code using free online resources and absolutely fell in love with the usefullness of code and the ability to create apps. Starting off with Python, JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, machine learning with Python, and much much more."}, 
        {name: 'a clear impact', description: 'At my current company, I have grown our revenue from ~$700,000 USD in 2022 to over $2.1 Million USD in 2023! The keys to this growth were installing a consistent lead generation system, building out a sales funnel, and onboarding and ramping a sales team to within KPI.'},
        {name: "an excellent leader", description: "I have led teams of up to 4 people, ensuring strong chemistry and consistent performance within set KPIs. I pride myself on honest, yet kind communication that allows lean teams to accomplish major objectives.",},
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Rohan</span> Saxena <br/> Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">favorite tech</span> includes Python, MySQL, 
                Javascript (NEXT.js or SvelteKit), TailwindCSS, Node.js, and React.js.
            </p>
            <p class="text-base sm:text-lg md:text-xl">
                I also like <span class="text-violet-400">Machine Learning</span> with TensorFlow, Cloud Storage in Azure, and Prompt Engineering using ChatGPT.
            </p>
            <a class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl
            poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" href="https://www.linkedin.com/in/rohan-saxena-ai/" target="_blank">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 
                group-hover:translate-x-full z-0 duration-200"/>

                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img src={"images/profile-picture.png"} alt="Profile image" class="object-cover z-[2] max-h-[70vh]"/>
        </div>
    </section>

    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endeavors. 
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 lg:gap-10">
            <Step step={steps[0]} githubLink="https://github.com/RohanSaxena2020/sales-coach-ai-v3" liveLink="#">
                <p>
                    This is a <strong class="text-violet-400">full-stack</strong> app 
                    which allows users to upload sales call transcripts and received expert coaching from AI. 
                    With the ability to login and see previous submissions!
                </p>
            </Step>

            <Step step={steps[1]} githubLink="https://github.com/RohanSaxena2020/PGA-tour-ai-v2" liveLink="#">
                <p>
                    The project takes in statistics on a golfer's driving, iron play, short game, and putting and outputs 
                    a predicted scoring average using a <strong class="text-violet-400">linear regression model</strong> trained on PGA tour data (from their website).
                </p>
            </Step>

            <Step step={steps[2]} githubLink="https://github.com/RohanSaxena2020/LLM-Project" liveLink="https://www.loom.com/share/dd76439a2803409da616f1ce00f77701?sid=5bc5703b-ab43-4f00-917b-6a12f398e294">
                <p>
                    This is a <strong class="text-violet-400">custom built LLM</strong> that allows my CEO to ask questions about the marketing data.
                    It then turns those questions into custom SQL queries and pulls the response from the <strong class="text-violet-400">MySQL database.</strong> 
                </p>
            </Step>

            <Step step={steps[3]} githubLink="https://github.com/RohanSaxena2020/AI/tree/main/Tomato%20Classification%20Project" liveLink="https://www.loom.com/share/3e080c8e468647f392bacd78335d64f7?sid=372fcc37-237d-4cfc-8508-3774dbd679bd">
                <p>
                    This is a neural network deep learning model built using <strong class="text-violet-400">Tensor Flow</strong>
                     designed to classify tomato diseases. It is trained on over 16000 images.
                </p>
            </Step>
        </div>
    </section>

    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl">
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
                <div class="flex gap-6 sm:gap-8">
                    <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
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

        <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">
            The <span class="text-violet-400">Complete</span> Package
        </h5>

        <div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr>
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th class="bg-violet-700 text-white whitespace-nowrap p-4 px-8">Me</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Dedication</td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Critical Thought</td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Interpersonal Skills</td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Programming Ability</td>
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

        <p class="mx-auto">So why not invest?</p>
    </section>
</main>