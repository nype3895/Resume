![Portfolio AI](https://github.com/user-attachments/assets/efcf7a55-6b7e-4126-90b6-d868f308b9f1)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nylah Perry - Portfolio</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/tailwindcss/2.2.19/tailwind.min.css" rel="stylesheet">
    <style>
        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .gradient-bg {
            background: linear-gradient(-45deg, #ff6b6b, #4ecdc4, #45b7d1, #96e6a1);
            background-size: 400% 400%;
            animation: gradient 15s ease infinite;
        }
        
        .section-card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            transition: transform 0.3s ease;
        }
        
        .section-card:hover {
            transform: translateY(-5px);
        }
        
        .tag {
            background: rgba(79, 209, 197, 0.2);
            border-radius: 15px;
            padding: 4px 12px;
            font-size: 0.875rem;
            color: #2c3e50;
        }
    </style>
</head>
<body class="gradient-bg min-h-screen">
    <nav class="bg-white bg-opacity-90 shadow-lg fixed w-full z-10">
        <div class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <h1 class="text-2xl font-bold text-gray-800">Nylah Perry</h1>
                <div class="space-x-6">
                    <a href="#education" class="text-gray-600 hover:text-gray-900">Education</a>
                    <a href="#experience" class="text-gray-600 hover:text-gray-900">Experience</a>
                    <a href="#leadership" class="text-gray-600 hover:text-gray-900">Leadership</a>
                    <a href="#skills" class="text-gray-600 hover:text-gray-900">Skills</a>
                </div>
            </div>
        </div>
    </nav>

    <main class="container mx-auto px-6 pt-24 pb-12">
        <header class="text-center mb-16">
            <h1 class="text-4xl font-bold text-white mb-4">Strategic Communication Designer</h1>
            <p class="text-xl text-white opacity-90">Content Creator | Athlete | Leader</p>
        </header>

        <section id="education" class="section-card p-8 mb-8">
            <h2 class="text-2xl font-bold mb-6 text-gray-800">Education</h2>
            <div class="space-y-6">
                <div>
                    <h3 class="text-xl font-semibold text-gray-700">University of Colorado, Boulder</h3>
                    <p class="text-gray-600">Masters of CMCI - Strategic Communication Design</p>
                    <p class="text-gray-500">Expected Graduation: August 2025</p>
                </div>
                <div>
                    <h3 class="text-xl font-semibold text-gray-700">University of Iowa</h3>
                    <p class="text-gray-600">Bachelor of Liberal Arts - Enterprise Leadership</p>
                    <p class="text-gray-500">Minor: Communications | Graduated: May 2024</p>
                    <div class="mt-2 flex flex-wrap gap-2">
                        <span class="tag">Dean's List</span>
                        <span class="tag">Academic All-Big Ten</span>
                        <span class="tag">USTFCCCA All-Academic</span>
                    </div>
                </div>
            </div>
        </section>

        <section id="experience" class="section-card p-8 mb-8">
            <h2 class="text-2xl font-bold mb-6 text-gray-800">Work Experience</h2>
            <div class="space-y-8">
                <div>
                    <h3 class="text-xl font-semibold text-gray-700">Digital Marketing Intern</h3>
                    <p class="text-gray-600">Mural Arts of Philadelphia | June 2024 - August 2024</p>
                    <ul class="mt-2 space-y-2 text-gray-600">
                        <li>• Created digital assets for 40th-anniversary campaign</li>
                        <li>• Led content production and social media strategy</li>
                    </ul>
                </div>
                <div>
                    <h3 class="text-xl font-semibold text-gray-700">Content Creator</h3>
                    <p class="text-gray-600">Social Media Influencer</p>
                    <ul class="mt-2 space-y-2 text-gray-600">
                        <li>• 120k+ TikTok followers, 87k+ Instagram followers</li>
                        <li>• Brand partnerships with companies like Milani Makeup</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="leadership" class="section-card p-8 mb-8">
            <h2 class="text-2xl font-bold mb-6 text-gray-800">Athletics & Leadership</h2>
            <div class="space-y-6">
                <div>
                    <h3 class="text-xl font-semibold text-gray-700">Women's Track and Field Team Athlete</h3>
                    <p class="text-gray-600">August 2020 - Present</p>
                    <p class="text-gray-600 mt-2">50-60 hours weekly commitment while maintaining full course load</p>
                </div>
                <div>
                    <h3 class="text-xl font-semibold text-gray-700">Secretary, Black Student Athlete Alliance</h3>
                    <p class="text-gray-600">August 2022 - Present</p>
                    <ul class="mt-2 space-y-2 text-gray-600">
                        <li>• Developed strategic planning initiatives</li>
                        <li>• Organized community engagement events</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="skills" class="section-card p-8">
            <h2 class="text-2xl font-bold mb-6 text-gray-800">Technical Skills</h2>
            <div class="flex flex-wrap gap-3">
                <span class="tag">MS Word</span>
                <span class="tag">PowerPoint</span>
                <span class="tag">Adobe Illustrator</span>
                <span class="tag">Adobe Photoshop</span>
                <span class="tag">Social Media Management</span>
                <span class="tag">Content Creation</span>
                <span class="tag">Digital Marketing</span>
            </div>
        </section>
    </main>

    <footer class="bg-white bg-opacity-90 py-6 mt-12">
        <div class="container mx-auto px-6 text-center text-gray-600">
            <p>© 2025 Nylah Perry. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>

I attempted to create a portfolio website using Claude.ai. While the AI-generated design provided a good starting point, I encountered several functionality issues that prevented the site from working as intended.

Positive Outcomes

Color and Layout Success – The website’s colors came out exactly as I envisioned, and I was satisfied with the overall layout.
Issues Encountered

Navigation Failure – The buttons designed to navigate between pages did not function properly. Clicking them caused the site to freeze.
Error Messages – Instead of transitioning to the next page, the website displayed an error message and became unresponsive.
Sketch Upload Issue – I initially tried to upload my own sketch to describe myself, but it did not convert correctly. As a result, I opted to let the AI generate an image based on my resume instead.
