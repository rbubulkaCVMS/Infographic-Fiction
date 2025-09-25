# Infographic-Fiction
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- (all your code as provided above) -->
</head>
<body class="bg-gray-100 text-gray-800">
    <!-- (rest of your code) -->
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Anatomy of a Story: An Infographic</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 350px;
            }
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-800">

    <div class="container mx-auto p-4 md:p-8">

        <header class="text-center mb-12">
            <h1 class="text-4xl md:text-6xl font-black text-[#E84855] mb-2">The Anatomy of a Story</h1>
            <p class="text-lg md:text-xl text-[#403F4C]">A visual guide to the elements of fiction that make stories unforgettable.</p>
        </header>

        <main class="grid grid-cols-1 md:grid-cols-2 gap-8">

            <section id="plot" class="md:col-span-2 bg-white rounded-lg shadow-md p-6">
                <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 text-center flex items-center justify-center space-x-2">
                    <span>The Plot Mountain 🗺️</span>
                    <button id="speakPlot" class="p-2 rounded-full hover:bg-gray-200 focus:outline-none">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.536 8.464a5 5 0 010 7.072m2.828-9.9a9 9 0 010 12.728m-9.9-2.828a5 5 0 010-7.072m-2.828 9.9a9 9 0 010-12.728M12 19V5" />
                        </svg>
                    </button>
                </h2>
                <p class="text-center mb-6 text-[#403F4C]">Plot is the sequence of events in a story, like a road map from beginning to end. The tension builds to a peak and then winds down. This chart shows the rise and fall of excitement throughout a typical story.</p>
                <div class="chart-container">
                    <canvas id="plotChart"></canvas>
                </div>
            </section>

            <section id="characters" class="bg-white rounded-lg shadow-md p-6">
                <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 text-center flex items-center justify-center space-x-2">
                    <span>Meet the Characters 🧑‍🤝‍🧑</span>
                    <button id="speakCharacters" class="p-2 rounded-full hover:bg-gray-200 focus:outline-none">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.536 8.464a5 5 0 010 7.072m2.828-9.9a9 9 0 010 12.728m-9.9-2.828a5 5 0 010-7.072m-2.828 9.9a9 9 0 010-12.728M12 19V5" />
                        </svg>
                    </button>
                </h2>
                <p class="text-center mb-6 text-[#403F4C]">Stories need characters to drive the action forward. The two most important roles are the protagonist and the antagonist.</p>
                <div class="flex flex-col sm:flex-row gap-4">
                    <div class="flex-1 text-center bg-[#00A6A6] text-white p-4 rounded-lg">
                        <div class="text-5xl mb-2">🦸</div>
                        <h3 class="text-xl font-bold">Protagonist</h3>
                        <p>The main character. The story is all about their journey and their struggles.</p>
                    </div>
                    <div class="flex-1 text-center bg-[#E84855] text-white p-4 rounded-lg">
                        <div class="text-5xl mb-2">🦹</div>
                        <h3 class="text-xl font-bold">Antagonist</h3>
                        <p>The character or force that works against the protagonist, creating the main conflict.</p>
                    </div>
                </div>
            </section>
            
            <section id="char-traits" class="bg-white rounded-lg shadow-md p-6">
                <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 text-center flex items-center justify-center space-x-2">
                    <span>Understanding a Character</span>
                    <button id="speakTraits" class="p-2 rounded-full hover:bg-gray-200 focus:outline-none">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.536 8.464a5 5 0 010 7.072m2.828-9.9a9 9 0 010 12.728m-9.9-2.828a5 5 0 010-7.072m-2.828 9.9a9 9 0 010-12.728M12 19V5" />
                        </svg>
                    </button>
                </h2>
                 <p class="text-center mb-6 text-[#403F4C]">How do we get to know a character? Authors reveal character traits through a combination of their thoughts, actions, and dialogue. Each piece gives us a clue to who they really are.</p>
                <div class="chart-container h-64 md:h-[300px]">
                    <canvas id="characterTraitsChart"></canvas>
                </div>
            </section>

            <section id="setting" class="md:col-span-2 bg-white rounded-lg shadow-md p-6">
                <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 text-center flex items-center justify-center space-x-2">
                    <span>Setting the Scene 🕰️</span>
                    <button id="speakSetting" class="p-2 rounded-full hover:bg-gray-200 focus:outline-none">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.536 8.464a5 5 0 010 7.072m2.828-9.9a9 9 0 010 12.728m-9.9-2.828a5 5 0 010-7.072m-2.828 9.9a9 9 0 010-12.728M12 19V5" />
                        </svg>
                    </button>
                </h2>
                <p class="text-center mb-6 text-[#403F4C]">The setting tells us the "when" and "where" of the story. It creates the mood and provides context for the events. A spooky old house creates a very different feeling than a sunny beach!</p>
                <div class="flex flex-col md:flex-row justify-center items-center gap-8">
                    <div class="text-center p-6 bg-[#F28F3B] rounded-lg text-white">
                        <div class="text-6xl mb-2">🕰️</div>
                        <h3 class="text-2xl font-bold">Time</h3>
                        <p>The historical period, year, season, or time of day.</p>
                    </div>
                    <div class="text-center p-6 bg-[#00A6A6] rounded-lg text-white">
                        <div class="text-6xl mb-2">🗺️</div>
                        <h3 class="text-2xl font-bold">Place</h3>
                        <p>The geographical location, from a single room to an entire galaxy.</p>
                    </div>
                </div>
            </section>

            <section id="conflict" class="md:col-span-2 bg-white rounded-lg shadow-md p-6">
                 <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 text-center flex items-center justify-center space-x-2">
                     <span>The Heart of the Story: Conflict 🥊</span>
                    <button id="speakConflict" class="p-2 rounded-full hover:bg-gray-200 focus:outline-none">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.536 8.464a5 5 0 010 7.072m2.828-9.9a9 9 0 010 12.728m-9.9-2.828a5 5 0 010-7.072m-2.828 9.9a9 9 0 010-12.728M12 19V5" />
                        </svg>
                    </button>
                 </h2>
                 <p class="text-center mb-6 text-[#403F4C]">Conflict is the main problem that the protagonist must face. Without conflict, there is no story! The two main types feel very different, as one is a battle within the mind and the other is a battle against the world.</p>
                <div class="chart-container">
                    <canvas id="conflictChart"></canvas>
                </div>
            </section>
            
            <section id="theme" class="md:col-span-2 bg-white rounded-lg shadow-md p-6 text-center">
                 <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 flex items-center justify-center space-x-2">
                     <span>The Big Idea: Theme 💡</span>
                    <button id="speakTheme" class="p-2 rounded-full hover:bg-gray-200 focus:outline-none">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.536 8.464a5 5 0 010 7.072m2.828-9.9a9 9 0 010 12.728m-9.9-2.828a5 5 0 010-7.072m-2.828 9.9a9 9 0 010-12.728M12 19V5" />
                        </svg>
                    </button>
                 </h2>
                <p class="mb-6 text-[#403F4C]">The theme is the central message or lesson the author wants you to learn. It's an idea about life that you can apply to your own world.</p>
                <div class="flex flex-wrap justify-center gap-4">
                    <span class="bg-[#00A6A6] text-white py-2 px-4 rounded-full font-semibold">Friendship is powerful</span>
                    <span class="bg-[#F28F3B] text-white py-2 px-4 rounded-full font-semibold">Honesty is the best policy</span>
                    <span class="bg-[#E84855] text-white py-2 px-4 rounded-full font-semibold">Never give up</span>
                    <span class="bg-[#7A3B69] text-white py-2 px-4 rounded-full font-semibold">Courage in the face of fear</span>
                </div>
            </section>

            <section id="gemini-tools" class="md:col-span-2 grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="bg-white rounded-lg shadow-md p-6">
                    <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 text-center">✨ Character Idea Generator ✨</h2>
                    <p class="text-center mb-4 text-[#403F4C]">Click the button to get a brand new character idea, complete with thoughts, actions, and personality.</p>
                    <div class="flex justify-center mb-4">
                        <button id="generateCharacterBtn" class="bg-[#00A6A6] text-white font-bold py-2 px-4 rounded-full hover:bg-[#007A7A] transition-colors focus:outline-none">Generate a Character</button>
                    </div>
                    <div id="characterOutput" class="bg-gray-50 p-4 rounded-lg text-left text-[#403F4C] hidden">
                        <p class="text-sm italic text-gray-500 mb-2">Generating...</p>
                    </div>
                </div>

                <div class="bg-white rounded-lg shadow-md p-6">
                    <h2 class="text-3xl font-bold text-[#7A3B69] mb-4 text-center">✨ Story Idea from a Theme ✨</h2>
                    <p class="text-center mb-4 text-[#403F4C]">Enter a theme below and get a story idea! (e.g., bravery, teamwork, kindness).</p>
                    <div class="flex flex-col items-center mb-4">
                        <input type="text" id="themeInput" placeholder="Enter a theme here..." class="w-full px-4 py-2 border rounded-full mb-2 focus:outline-none focus:ring-2 focus:ring-[#7A3B69]">
                        <button id="generateStoryBtn" class="bg-[#E84855] text-white font-bold py-2 px-4 rounded-full hover:bg-[#B73842] transition-colors focus:outline-none">Generate Idea</button>
                    </div>
                    <div id="storyOutput" class="bg-gray-50 p-4 rounded-lg text-left text-[#403F4C] hidden">
                        <p class="text-sm italic text-gray-500 mb-2">Generating...</p>
                    </div>
                </div>
            </section>

        </main>

        <footer class="text-center mt-12 text-gray-500">
            <p>Infographic created to make learning fun.</p>
        </footer>

    </div>

    <script>
        const vibrantPalette = {
            blue: '#00A6A6',
            orange: '#F28F3B',
            red: '#E84855',
            purple: '#7A3B69',
            darkGray: '#403F4C'
        };

        const chartTooltipOptions = {
            plugins: {
                tooltip: {
                    callbacks: {
                        title: function(tooltipItems) {
                            const item = tooltipItems[0];
                            let label = item.chart.data.labels[item.dataIndex];
                            if (Array.isArray(label)) {
                              return label.join(' ');
                            } else {
                              return label;
                            }
                        }
                    }
                }
            }
        };

        function wrapLabel(str, maxWidth = 16) {
            if (str.length <= maxWidth) {
                return str;
            }
            const words = str.split(' ');
            const lines = [];
            let currentLine = '';
            words.forEach(word => {
                if ((currentLine + word).length > maxWidth) {
                    lines.push(currentLine.trim());
                    currentLine = '';
                }
                currentLine += word + ' ';
            });
            lines.push(currentLine.trim());
            return lines.filter(line => line);
        }

        const plotCtx = document.getElementById('plotChart').getContext('2d');
        const plotChart = new Chart(plotCtx, {
            type: 'line',
            data: {
                labels: ['Exposition', 'Rising Action', 'Climax', 'Falling Action', 'Resolution'],
                datasets: [{
                    label: 'Story Tension',
                    data: [10, 60, 100, 50, 10],
                    backgroundColor: 'rgba(232, 72, 85, 0.2)',
                    borderColor: vibrantPalette.red,
                    tension: 0.4,
                    fill: true,
                }]
            },
            options: {
                ...chartTooltipOptions,
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    y: {
                        beginAtZero: true,
                        title: {
                            display: true,
                            text: 'Tension / Excitement Level'
                        }
                    }
                },
                plugins: {
                     ...chartTooltipOptions.plugins,
                    legend: {
                        display: false
                    }
                }
            }
        });

        const characterTraitsCtx = document.getElementById('characterTraitsChart').getContext('2d');
        const characterTraitsChart = new Chart(characterTraitsCtx, {
            type: 'doughnut',
            data: {
                labels: ['Actions', 'Dialogue', 'Thoughts'],
                datasets: [{
                    label: 'Character Clues',
                    data: [33.3, 33.3, 33.3],
                    backgroundColor: [vibrantPalette.blue, vibrantPalette.orange, vibrantPalette.purple],
                    hoverOffset: 4
                }]
            },
            options: {
                ...chartTooltipOptions,
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    ...chartTooltipOptions.plugins,
                    legend: {
                        position: 'bottom',
                    }
                }
            }
        });

        const conflictCtx = document.getElementById('conflictChart').getContext('2d');
        const conflictChart = new Chart(conflictCtx, {
            type: 'radar',
            data: {
                labels: ['Mental Struggle', 'Physical Obstacle', 'Emotional Turmoil', 'Societal Pressure', 'Force of Nature'],
                datasets: [{
                    label: 'Internal Conflict',
                    data: [90, 10, 85, 40, 5],
                    backgroundColor: 'rgba(0, 166, 166, 0.2)',
                    borderColor: vibrantPalette.blue,
                    pointBackgroundColor: vibrantPalette.blue
                }, {
                    label: 'External Conflict',
                    data: [20, 80, 30, 75, 90],
                    backgroundColor: 'rgba(242, 143, 59, 0.2)',
                    borderColor: vibrantPalette.orange,
                    pointBackgroundColor: vibrantPalette.orange
                }]
            },
            options: {
                 ...chartTooltipOptions,
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                     ...chartTooltipOptions.plugins,
                    legend: {
                        position: 'bottom',
                    }
                },
                 scales: {
                    r: {
                        angleLines: {
                            display: true
                        },
                        suggestedMin: 0,
                        suggestedMax: 100
                    }
                }
            }
        });

        const apiKey = "";
        const generateCharacterBtn = document.getElementById('generateCharacterBtn');
        const characterOutput = document.getElementById('characterOutput');
        const themeInput = document.getElementById('themeInput');
        const generateStoryBtn = document.getElementById('generateStoryBtn');
        const storyOutput = document.getElementById('storyOutput');
        const textToSpeak = {
            plot: "The Plot Mountain, the story's road map.",
            characters: "Meet the characters, the people or creatures in the story.",
            traits: "Understanding a character, through their thoughts, words, and actions.",
            setting: "Setting the scene, when and where it happens.",
            conflict: "The heart of the story, conflict.",
            theme: "The big idea, theme, the central message of the story."
        };

        async function callGeminiAPI(prompt) {
            const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-05-20:generateContent?key=${apiKey}`;
            const payload = {
                contents: [{ parts: [{ text: prompt }] }]
            };
            try {
                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });
                const result = await response.json();
                return result.candidates[0].content.parts[0].text;
            } catch (error) {
                console.error('Error calling Gemini API:', error);
                return 'Sorry, something went wrong. Please try again.';
            }
        }

        async function speakText(text) {
            const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-tts:generateContent?key=${apiKey}`;
            const payload = {
                contents: [{ parts: [{ text: text }] }],
                generationConfig: {
                    responseModalities: ["AUDIO"],
                    speechConfig: {
                        voiceConfig: {
                            prebuiltVoiceConfig: { voiceName: "Puck" }
                        }
                    }
                },
                model: "gemini-2.5-flash-preview-tts"
            };
            try {
                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });
                const result = await response.json();
                const audioData = result?.candidates?.[0]?.content?.parts?.[0]?.inlineData?.data;
                const mimeType = result?.candidates?.[0]?.content?.parts?.[0]?.inlineData?.mimeType;

                if (audioData && mimeType && mimeType.startsWith("audio/")) {
                    const sampleRate = parseInt(mimeType.match(/rate=(\d+)/)[1], 10);
                    const pcmData = base64ToArrayBuffer(audioData);
                    const pcm16 = new Int16Array(pcmData);
                    const wavBlob = pcmToWav(pcm16, sampleRate);
                    const audioUrl = URL.createObjectURL(wavBlob);
                    const audio = new Audio(audioUrl);
                    audio.play();
                } else {
                    console.error('TTS API response error:', result);
                }
            } catch (error) {
                console.error('Error calling TTS API:', error);
            }
        }

        function base64ToArrayBuffer(base64) {
            const binaryString = atob(base64);
            const len = binaryString.length;
            const bytes = new Uint8Array(len);
            for (let i = 0; i < len; i++) {
                bytes[i] = binaryString.charCodeAt(i);
            }
            return bytes.buffer;
        }

        function pcmToWav(pcmData, sampleRate) {
            const buffer = new ArrayBuffer(44 + pcmData.length * 2);
            const view = new DataView(buffer);

            writeString(view, 0, 'RIFF');
            view.setUint32(4, 36 + pcmData.length * 2, true);
            writeString(view, 8, 'WAVE');
            writeString(view, 12, 'fmt ');
            view.setUint32(16, 16, true);
            view.setUint16(20, 1, true);
            view.setUint16(22, 1, true);
            view.setUint32(24, sampleRate, true);
            view.setUint32(28, sampleRate * 2, true);
            view.setUint16(32, 2, true);
            view.setUint16(34, 16, true);
            writeString(view, 36, 'data');
            view.setUint32(40, pcmData.length * 2, true);

            let offset = 44;
            for (let i = 0; i < pcmData.length; i++) {
                view.setInt16(offset, pcmData[i], true);
                offset += 2;
            }

            return new Blob([view], { type: 'audio/wav' });
        }

        function writeString(view, offset, string) {
            for (let i = 0; i < string.length; i++) {
                view.setUint8(offset + i, string.charCodeAt(i));
            }
        }

        generateCharacterBtn.addEventListener('click', async () => {
            generateCharacterBtn.disabled = true;
            characterOutput.classList.remove('hidden');
            characterOutput.innerHTML = '<p class="text-sm italic text-gray-500 mb-2">Generating...</p>';
            const prompt = "Generate a character description for a fiction story for 6th graders. Include their inner thoughts, a short biography, and an action they often perform. The character should be a relatable student.";
            const generatedText = await callGeminiAPI(prompt);
            characterOutput.innerHTML = `<p>${generatedText}</p>`;
            generateCharacterBtn.disabled = false;
        });

        generateStoryBtn.addEventListener('click', async () => {
            const theme = themeInput.value.trim();
            if (!theme) {
                storyOutput.classList.remove('hidden');
                storyOutput.innerHTML = '<p class="text-red-500">Please enter a theme!</p>';
                return;
            }
            generateStoryBtn.disabled = true;
            storyOutput.classList.remove('hidden');
            storyOutput.innerHTML = '<p class="text-sm italic text-gray-500 mb-2">Generating...</p>';
            const prompt = `Write a short story idea for 6th graders based on the theme: ${theme}. The idea should include a clear plot, character, and conflict.`;
            const generatedText = await callGeminiAPI(prompt);
            storyOutput.innerHTML = `<p>${generatedText}</p>`;
            generateStoryBtn.disabled = false;
        });
        
        document.getElementById('speakPlot').addEventListener('click', () => speakText(textToSpeak.plot));
        document.getElementById('speakCharacters').addEventListener('click', () => speakText(textToSpeak.characters));
        document.getElementById('speakTraits').addEventListener('click', () => speakText(textToSpeak.traits));
        document.getElementById('speakSetting').addEventListener('click', () => speakText(textToSpeak.setting));
        document.getElementById('speakConflict').addEventListener('click', () => speakText(textToSpeak.conflict));
        document.getElementById('speakTheme').addEventListener('click', () => speakText(textToSpeak.theme));
    </script>
</body>
</html>
