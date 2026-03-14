<template>
    <div class="scrollElement review-carousel-body bg-white">
        <div class="review-slider">
            <!-- ========================================
                Review Track Container
                Contains 16 cards (8 unique reviews × 2 for infinite loop)
                Width calculated: 350px per card × 16 cards = 5600px total
            ======================================== -->
            <div class="review-slide-track grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">

                <!-- Review 1 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <!-- Date -->
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        January 2024
                    </p>
                    <!-- Review Text -->
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "[Guide name]—he was so well informed and thoughtful in explaining the historical
                        relationship to history and the importance of understanding it in the present."
                    </p>
                </div>

                <!-- Review 2 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)]  p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Well researched presentation. She did a great job putting various events onto a timeline, 
                        which in turned helped to explain the contemporary mindset. She also communicated her love of the university."
                    </p>
                </div>

                <!-- Review 3 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "I was very impressed with how well the event was organized. 
                        I reached out in January when most students were still on break and got a response within 2 days! 
                        It was a real pleasure to see such professionalism coming from young people! Bravo and thank you for all you do."
                    </p>
                </div>

                <!-- Review 4 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Our tour guide, [guide], was incredibly knowledgeable and engaging. 
                        We learned a lot about UVA, Charlottesville, and Virginia through her fantastic storytelling."
                    </p>
                </div>

                <!-- Review 5 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "[Guide], the tour guide, was knowledgeable, enthusiastic, and articulate. 
                        The tour itself was well-balanced and managed, in a well-structured way, to cover a variety of interesting subjects."
                    </p>
                </div>

                <!-- Review 6 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        October 2025
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "This critical/complicated understanding and connection to the institutions 
                        we come from are so essential to figuring out how we move forward."
                    </p>
                </div>
            
                <!-- Review 7 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        October 2025
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Going to Monticello after UVa was really important and looking back at the Rotunda from Monticello 
                        to see how the organization of the house is related to the organization of the institution, citizenship, 
                        and the nation which makes you really question how these spaces normalized what they stood for."
                    </p>
                </div>
            
                <!-- Review 8 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        October 2025
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Thank you for your outstanding tour and extraordinarily generous hospitality. I think our students got 
                        a chance to see through your example what an exemplary UVa student sounds like. You also allowed me to 
                        reconnect with where I come from. So I can't thank you enough."
                    </p>
                </div>

                <!-- ========================================
                     DUPLICATED REVIEWS (for seamless infinite loop)
                     Same 8 reviews repeated to create continuous scrolling effect
                 ======================================== -->

                <!-- Review 1 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <!-- Date -->
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        January 2024
                    </p>
                    <!-- Review Text -->
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "[Guide name]—he was so well informed and thoughtful in explaining the historical
                        relationship to history and the importance of understanding it in the present."
                    </p>
                </div>

                <!-- Review 2 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Well researched presentation. She did a great job putting various events onto a timeline, 
                        which in turned helped to explain the contemporary mindset. She also communicated her love of the university."
                    </p>
                </div>

                <!-- Review 3 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "I was very impressed with how well the event was organized. 
                        I reached out in January when most students were still on break and got a response within 2 days! 
                        It was a real pleasure to see such professionalism coming from young people! Bravo and thank you for all you do."
                    </p>
                </div>

                <!-- Review 4 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Our tour guide, [guide], was incredibly knowledgeable and engaging. 
                        We learned a lot about UVA, Charlottesville, and Virginia through her fantastic storytelling."
                    </p>
                </div>

                <!-- Review 5 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        February 2024
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "[Guide], the tour guide, was knowledgeable, enthusiastic, and articulate. 
                        The tour itself was well-balanced and managed, in a well-structured way, to cover a variety of interesting subjects."
                    </p>
                </div>
            
                <!-- Review 6 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        October 2025
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "This critical/complicated understanding and connection to the institutions 
                        we come from are so essential to figuring out how we move forward."
                    </p>
                </div>
            
                <!-- Review 7 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        October 2025
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Going to Monticello after UVa was really important and looking back at the Rotunda from Monticello 
                        to see how the organization of the house is related to the organization of the institution, citizenship, 
                        and the nation which makes you really question how these spaces normalized what they stood for."
                    </p>
                </div>
            
                <!-- Review 8 -->
                <div class="review-slide flex flex-col w-full h-64 bg-white rounded-lg shadow-[0px_2px_16px_0px_rgba(14,30,37,0.32)] p-4 relative">
                    <p class="absolute top-2 right-4 text-black text-sm sm:text-base font-semibold font-['Montserrat']">
                        October 2025
                    </p>
                    <p class="mt-8 text-black text-base sm:text-lg font-medium font-['Montserrat'] overflow-auto">
                        "Thank you for your outstanding tour and extraordinarily generous hospitality. I think our students got 
                        a chance to see through your example what an exemplary UVa student sounds like. You also allowed me to 
                        reconnect with where I come from. So I can't thank you enough."
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
    /* === Tour Reviews Auto-Scroll Carousel === */
    .review-carousel-body {
        width: 100%;
        height: var(--height);
        display: grid;
        place-items: center;
    }
    /* Visible window for the carousel */
    .review-slider{
        height: 400px;
        margin: auto;
        position: relative;
        width: 100%;
        display: grid;
        place-items: center;
        overflow: hidden;
    }
    /* Container that moves horizontally */
    .review-slide-track{
        display: flex;
        width: calc(350px * 16); /* 16 slides × 350px each */
        animation: scroll-review 20s linear infinite;
        will-change: transform;
    }
    /* Right-to-left scrolling animation */
    @keyframes scroll-review {
        0% {
            transform: translateX(calc(-350px * 8));
        }
        100% {
            transform: translateX(0);
        }
    }
    /* Pause animation on hover */
    .review-slide-track:hover{
        animation-play-state: paused;
    }
    /* Individual review card */
    .review-slide{
        height: 250px;
        width: 350px;
        display: flex;
        align-items: center;
        padding: 15px;
        perspective: 100px;
    }

    /* === Responsive overrides === */

    /* Tablet (640px – 1023px) */
    @media (max-width: 1023px) {
        .review-slider {
            height: 320px;
        }
        .review-slide {
            width: 280px;
            height: 220px;
            padding: 12px;
        }
        .review-slide .text-sm {
            font-size: 1.25rem;
        }
        .review-slide p {
            font-size: 1rem;
        }
        .review-slide-track {
            width: calc(280px * 16);
        }
        @keyframes scroll-reviews {
            0%   { transform: translateX(calc(-280px * 8)); }
            100% { transform: translateX(0); }
        }
    }

    /* Mobile (< 640px) */
    @media (max-width: 639px) {
        .review-slider {
            height: 260px;
        }
        .review-slide {
            width: 200px;
            height: 180px;
            padding: 8px;
        }
        .review-slide .text-sm {
            font-size: 0.85rem;
        }
        .review-slide p {
            font-size: 0.8rem;
        }
        .review-slide-track {
            width: calc(200px * 16);
        }
        @keyframes scroll-reviews {
            0%   { transform: translateX(calc(-200px * 8)); }
            100% { transform: translateX(0); }
        }
    }
</style>
