[index.HTML.HTML](https://github.com/user-attachments/files/34022133/index.HTML.HTML)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Shubanghi ❤️ - Please Forgive Me</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600;700&family=Lora:ital,wght@0,400..700;1,400..700&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
    <script src="https://unpkg.com/lucide@latest"></script>
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        blush: '#fff0f3',
                        softrose: '#ffb3c6',
                        deeprose: '#c9184a',
                        vintagecream: '#fbf9f5',
                    },
                    fontFamily: {
                        script: ['"Dancing Script"', 'cursive'],
                        serif: ['"Lora"', 'serif'],
                        sans: ['"Poppins"', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        .polaroid {
            background: white;
            padding: 12px 12px 35px 12px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.08);
            transition: all 0.3s ease;
        }
        .polaroid:hover {
            transform: translateY(-5px) rotate(0deg) !important;
            box-shadow: 0 15px 35px rgba(201, 24, 74, 0.15);
        }
        .envelope-flap {
            transition: transform 0.6s ease;
            transform-origin: top;
        }
        .open-flap {
            transform: rotateX(180deg);
        }
        #button-container {
            min-height: 5rem;
        }

        @media (max-width: 640px) {
            body {
                padding: 1rem 0.75rem;
            }

            #main-content {
                padding-top: 2.5rem;
                padding-bottom: 2.5rem;
            }

            #envelope-screen {
                padding: 1.25rem 1rem;
            }

            #envelope {
                width: min(88vw, 24rem);
                height: 12rem;
            }

            .polaroid img {
                height: 13rem;
            }

            #button-container {
                min-height: 8rem;
                flex-wrap: wrap;
                gap: 0.75rem;
            }

            #no-btn {
                position: static !important;
                transform: none !important;
            }
        }
    </style>
</head>
<body class="bg-vintagecream min-h-screen font-sans text-gray-800 flex flex-col items-center justify-center p-4 overflow-x-hidden">

    <!-- STAGE 1: The Interactive Envelope Screen -->
    <div id="envelope-screen" class="fixed inset-0 bg-gradient-to-br from-blush via-vintagecream to-softrose/40 z-50 flex flex-col items-center justify-center p-6 transition-opacity duration-700">
        <div class="text-center space-y-3 mb-8 animate-pulse">
            <span class="text-deeprose font-medium text-sm tracking-widest uppercase">Special Delivery</span>
            <h1 class="font-script text-5xl sm:text-6xl text-deeprose">A Letter For Shubanghi</h1>
            <p class="font-serif italic text-gray-600 text-sm">Tap the envelope to open your message</p>
        </div>

        <!-- Envelope Graphic -->
        <div id="envelope" onclick="openEnvelope()" class="relative w-80 sm:w-96 h-56 sm:h-64 bg-rose-200 rounded-2xl shadow-2xl cursor-pointer transform transition hover:scale-105 flex items-center justify-center border border-rose-300">
            <!-- Envelope Flap -->
            <div id="flap" class="absolute top-0 left-0 w-full h-28 bg-rose-300 rounded-t-2xl origin-top z-20 shadow-md" style="clip-path: polygon(0 0, 50% 100%, 100% 0);"></div>
            
            <!-- Seal Heart -->
            <div class="absolute z-30 w-16 h-16 bg-deeprose rounded-full flex items-center justify-center shadow-lg text-white animate-bounce">
                <i data-lucide="heart" class="w-8 h-8 fill-current"></i>
            </div>

            <div class="absolute bottom-6 text-center z-10">
                <p class="font-script text-2xl text-deeprose font-bold">Open Me ❤️</p>
            </div>
        </div>
    </div>

    <!-- STAGE 2: Main Website Content (Hidden initially until envelope opens) -->
    <div id="main-content" class="opacity-0 pointer-events-none transition-opacity duration-1000 max-w-3xl w-full mx-auto space-y-12 py-12">

        <!-- Header -->
        <header class="text-center space-y-3">
            <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-rose-100 text-deeprose font-medium text-xs tracking-wider shadow-sm">
                <i data-lucide="sparkles" class="w-4 h-4"></i> From The Bottom Of My Heart
            </div>
            <h1 class="font-script text-6xl sm:text-7xl text-deeprose">I'm So Sorry, Shubanghi</h1>
            <p class="font-serif italic text-gray-600 max-w-md mx-auto">
                "I know saying sorry isn't enough to undo my mistake, but I promise to spend every day making it up to you."
            </p>
        </header>

        <!-- Polaroid Memory Wall -->
        <section class="space-y-6">
            <div class="text-center">
                <h2 class="font-serif text-2xl text-gray-800">Our Beautiful Memories</h2>
                <p class="text-xs text-gray-500">The moments that mean everything to me</p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-3 gap-6 pt-4">
                <!-- Polaroid 1 -->
                <div class="polaroid transform -rotate-2">
                    <img src="PXL_20261017_132028084.NIGHT.jpg" alt="Memory 1" class="w-full h-52 object-cover rounded-sm">
                    <p class="font-script text-xl text-center text-gray-700 mt-3">Our special night ✨</p>
                </div>
                <!-- Polaroid 2 -->
                <div class="polaroid transform rotate-1 sm:translate-y-4">
                    <img src="PXL_20261017_115157079.MP.jpg" alt="Memory 2" class="w-full h-52 object-cover rounded-sm">
                    <p class="font-script text-xl text-center text-gray-700 mt-3">Your gorgeous smile ❤️</p>
                </div>
                <!-- Polaroid 3 -->
                <div class="polaroid transform -rotate-1">
                    <img src="PXL_20261017_121057462.MP.jpg" alt="Memory 3" class="w-full h-52 object-cover rounded-sm">
                    <p class="font-script text-xl text-center text-gray-700 mt-3">Always holding onto us</p>
                </div>
            </div>
        </section>

        <!-- Vintage Love & Apology Letter -->
        <section class="bg-white p-8 sm:p-10 rounded-3xl shadow-xl border border-rose-100 relative space-y-4">
            <div class="absolute -top-4 left-1/2 -translate-x-1/2 bg-deeprose text-white px-4 py-1 rounded-full text-xs font-medium tracking-wide shadow">
                Read My Letter
            </div>
            
            <div class="space-y-4 font-serif text-gray-700 text-base sm:text-lg leading-relaxed pt-2">
                <p class="font-script text-3xl text-deeprose">Dearest Shubanghi,</p>
                <p>
                    Ik sorry bol kar nothing will change everything instantly, but I know I made a mistake, and I am truly, deeply sorry for it.
                </p>
                <p>
                    Your happiness, your peace of mind, and our relationship mean everything to me. I promise to listen better, communicate more openly, and work every single day to be the partner you deserve.
                </p>
                <p>Ha this time i used a bit AI but they feelings and memories are mine </p>
                <p class="font-script text-2xl text-deeprose pt-2 text-right">
                    With all my love, <br>Shontae
                </p>
            </div>
        </section>

        <!-- Voice Note Section -->
        <section class="bg-gradient-to-r from-rose-50 to-pink-50 p-6 sm:p-8 rounded-3xl border border-rose-200 shadow-sm space-y-4 text-center">
            <div class="flex items-center justify-center gap-2 text-deeprose font-medium">
                <i data-lucide="mic" class="w-5 h-5"></i>
                <span>Listen to my personal voice note</span>
            </div>

            <audio id="audio-player" class="hidden" src="27 Oct at 12-23 pm.mp3"></audio>

            <div class="flex items-center justify-center gap-4">
                <button id="play-btn" class="px-6 py-3 bg-deeprose text-white rounded-full font-medium shadow-md hover:bg-rose-700 transition flex items-center gap-2">
                    <i data-lucide="play" class="w-4 h-4 fill-current"></i> Play Audio Message
                </button>
            </div>
            <p id="audio-status" class="text-xs text-gray-500">Click play to listen to your voice note.</p>
        </section>

        <!-- The Playful Forgiveness Section -->
        <section class="text-center space-y-6 pt-6">
            <h3 class="font-serif text-2xl sm:text-3xl text-gray-800">
                Can you find it in your heart to forgive me?
            </h3>
            
            <div id="button-container" class="relative flex items-center justify-center gap-6 h-20">
                <button onclick="acceptForgiveness()" class="px-8 py-4 bg-gradient-to-r from-deeprose to-rose-600 text-white font-semibold text-lg rounded-full shadow-lg hover:shadow-xl transition transform hover:scale-105 flex items-center gap-2 z-20">
                    <i data-lucide="heart" class="w-5 h-5 fill-current"></i> Yes, I Forgive You ❤️
                </button>
                
                <!-- The Playful Escaping No Button -->
                <button id="no-btn" onmouseover="moveNoButton()" onclick="moveNoButton()" class="px-6 py-4 bg-gray-200 text-gray-700 font-medium text-base rounded-full shadow-sm transition-all duration-200 absolute">
                    No 🙈
                </button>
            </div>
        </section>

    </div>

    <!-- Success Modal -->
    <div id="success-modal" class="fixed inset-0 bg-black/50 backdrop-blur-sm z-50 flex items-center justify-center p-4 hidden opacity-0 transition-opacity duration-300">
        <div class="bg-white rounded-3xl max-w-md w-full p-8 text-center space-y-6 shadow-2xl">
            <div class="w-20 h-20 bg-rose-100 rounded-full flex items-center justify-center mx-auto text-deeprose">
                <i data-lucide="heart" class="w-10 h-10 fill-current animate-bounce"></i>
            </div>
            <div class="space-y-2">
                <h3 class="font-script text-4xl text-deeprose">Thank You, My Love!</h3>
                <p class="text-gray-600">You just made me the happiest person alive. I promise to cherish you always.</p>
            </div>
            <button onclick="location.reload()" class="w-full py-3 bg-deeprose hover:bg-rose-700 text-white font-medium rounded-full shadow transition">
                Close 🤗
            </button>
        </div>
    </div>

    <script>
        lucide.createIcons();

        // Envelope Open Action
        function openEnvelope() {
            const flap = document.getElementById('flap');
            const envelopeScreen = document.getElementById('envelope-screen');
            const mainContent = document.getElementById('main-content');

            flap.classList.add('open-flap');
            
            setTimeout(() => {
                envelopeScreen.classList.add('opacity-0');
                setTimeout(() => {
                    envelopeScreen.style.display = 'none';
                    mainContent.classList.remove('opacity-0', 'pointer-events-none');
                }, 700);
            }, 500);
        }

        // Playful "No" Button Handler
        function moveNoButton() {
            const noBtn = document.getElementById('no-btn');
            const x = Math.random() * 200 - 100;
            const y = Math.random() * 100 - 50;
            noBtn.style.transform = `translate(${x}px, ${y}px)`;
        }

        // Accept Forgiveness
        function acceptForgiveness() {
            confetti({
                particleCount: 100,
                spread: 80,
                origin: { y: 0.6 },
                colors: ['#c9184a', '#ffb3c6', '#ff4d6d', '#fff']
            });

            const modal = document.getElementById('success-modal');
            modal.classList.remove('hidden');
            setTimeout(() => modal.classList.remove('opacity-0'), 10);
        }

        // Audio Player Logic
        const audioPlayer = document.getElementById('audio-player');
        const playBtn = document.getElementById('play-btn');
        const audioStatus = document.getElementById('audio-status');

        function resetAudioStatusClasses() {
            audioStatus.classList.remove('text-deeprose', 'text-green-600');
            audioStatus.classList.add('text-gray-500');
        }

        playBtn.onclick = () => {
            const hasSource = Boolean(audioPlayer.getAttribute('src') && audioPlayer.getAttribute('src').trim());

            if (!hasSource) {
                audioStatus.textContent = "Please upload an audio file first using the button above!";
                audioStatus.classList.remove('text-gray-500', 'text-green-600');
                audioStatus.classList.add('text-deeprose');
                return;
            }

            if (audioPlayer.paused) {
                audioPlayer.play().catch(() => {
                    audioStatus.textContent = "Your browser blocked playback until you click again.";
                    audioStatus.classList.remove('text-gray-500', 'text-green-600');
                    audioStatus.classList.add('text-deeprose');
                });
                playBtn.innerHTML = `<i data-lucide="pause" class="w-4 h-4 fill-current"></i> Pause Audio`;
                audioStatus.textContent = "Playing your voice note...";
                resetAudioStatusClasses();
                lucide.createIcons();
            } else {
                audioPlayer.pause();
                playBtn.innerHTML = `<i data-lucide="play" class="w-4 h-4 fill-current"></i> Play Audio Message`;
                audioStatus.textContent = "Paused.";
                resetAudioStatusClasses();
                lucide.createIcons();
            }
        };


    </script>
</body>
</html>
