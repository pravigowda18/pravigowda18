<!DOCTYPE html>
<html lang="en" class="scroll-smooth">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Praveen S - AI/ML Engineer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #111827;
            /* Dark Gray-Blue */
            color: #d1d5db;
            /* Light Gray */
        }

        .text-gradient {
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            background-image: linear-gradient(to right, #3b82f6, #8b5cf6);
        }

        /* For the typing effect */
        .typing-cursor {
            border-right: .15em solid #3b82f6;
            animation: blink-caret .75s step-end infinite;
        }

        @keyframes blink-caret {

            from,
            to {
                border-color: transparent
            }

            50% {
                border-color: #3b82f6;
            }
        }

        .glass-effect {
            background: rgba(31, 41, 55, 0.5);
            /* Semi-transparent dark gray */
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        /* For the project details expansion */
        .collapsible-content {
            max-height: 500px;
            /* Expanded by default for mobile-first */
            overflow: hidden;
            transition: max-height 0.5s ease-in-out;
        }

        /* For desktop view (md and larger), collapse it by default */
        @media (min-width: 768px) {
            .collapsible-content {
                max-height: 0;
            }

            .collapsible-content.expanded {
                max-height: 500px;
                /* Adjust if content is taller */
            }
        }
    </style>
</head>

<body class="antialiased">

    <!-- Header -->
    <header id="header" class="fixed top-0 left-0 right-0 z-50 transition-all duration-300">
        <div class="container mx-auto px-6 py-4">
            <div class="flex items-center justify-between">
                <div class="text-2xl font-bold text-white">
                    <a href="#hero">PS.</a>
                </div>
                <nav class="hidden md:flex space-x-8">
                    <a href="#about" class="text-gray-300 hover:text-blue-400 transition">About</a>
                    <a href="#experience" class="text-gray-300 hover:text-blue-400 transition">Experience</a>
                    <a href="#education" class="text-gray-300 hover:text-blue-400 transition">Education</a>
                    <a href="#projects" class="text-gray-300 hover:text-blue-400 transition">Projects</a>
                    <a href="#contact" class="text-gray-300 hover:text-blue-400 transition">Contact</a>
                </nav>
                <!-- Mobile Menu Button -->
                <button id="mobile-menu-btn" class="md:hidden text-white">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"
                        xmlns="http://www.w3.org/2000/svg">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                            d="M4 6h16M4 12h16m-7 6h7"></path>
                    </svg>
                </button>
            </div>
        </div>
    </header>

    <!-- Mobile Menu -->
    <div id="mobile-menu" class="hidden fixed inset-0 z-40 bg-gray-900 bg-opacity-95">
        <div class="flex flex-col items-center justify-center h-full space-y-8">
            <a href="#about" class="mobile-menu-link text-2xl text-gray-300 hover:text-blue-400 transition">About</a>
            <a href="#experience"
                class="mobile-menu-link text-2xl text-gray-300 hover:text-blue-400 transition">Experience</a>
            <a href="#education"
                class="mobile-menu-link text-2xl text-gray-300 hover:text-blue-400 transition">Education</a>
            <a href="#projects"
                class="mobile-menu-link text-2xl text-gray-300 hover:text-blue-400 transition">Projects</a>
            <a href="#contact"
                class="mobile-menu-link text-2xl text-gray-300 hover:text-blue-400 transition">Contact</a>
        </div>
    </div>

    <main class="container mx-auto px-6 pt-24 md:pt-32">

        <!-- Hero Section -->
        <section id="hero" class="min-h-[80vh] flex items-center">
            <div class="max-w-3xl">
                <h1 class="text-5xl md:text-7xl font-bold text-white leading-tight">
                    Hi, I'm Praveen S
                </h1>
                <h2 class="text-2xl md:text-4xl mt-4 font-semibold">
                    I'm an <span id="typing-text" class="text-gradient"></span><span class="typing-cursor"></span>
                </h2>
                <p class="mt-6 text-lg text-gray-400 max-w-xl">
                    I’m an AI/ML enthusiast and backend developer passionate about building intelligent, real-world
                    applications. I specialize in computer vision, NLP, and deep learning, creating solutions like
                    AI-powered surveillance, gesture recognition, and chatbot systems. I enjoy taking projects from
                    concept to deployment, combining cutting-edge AI models with scalable web applications
                </p>
                <div class="mt-10 flex items-center gap-4">
                    <a href="#contact"
                        class="bg-blue-600 hover:bg-blue-700 text-white font-semibold py-3 px-6 rounded-lg transition duration-300">
                        Get In Touch
                    </a>
                    <a href="#projects"
                        class="border-2 border-gray-600 hover:bg-gray-700 text-white font-semibold py-3 px-6 rounded-lg transition duration-300">
                        View My Work
                    </a>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="py-20 md:py-32">
            <h2 class="text-4xl font-bold text-white text-center mb-12">About Me</h2>
            <div class="max-w-4xl mx-auto">
                <div class="flex flex-col md:flex-row items-center gap-12">
                    <div class="md:w-1/3 flex-shrink-0">
                        <img src="images/IMG-20241215-WA0057.jpg" alt="Praveen S Portrait"
                            class="rounded-full shadow-lg mx-auto w-64 h-64 md:w-80 md:h-80 object-cover">
                    </div>
                    <div class="md:w-2/3">
                        <p class="text-gray-300 mb-6 leading-relaxed">
                            I’m an AI/ML Enthusiast and Backend Developer passionate about building intelligent
                            systems that bridge the gap between research and real-world applications. My work spans
                            across computer vision, natural language processing, and deep learning, where I’ve developed
                            solutions such as AI-powered surveillance systems, gesture recognition applications, virtual
                            mouse interfaces, biometric authentication, and intelligent task management tools
                        </p>
                        <p class="text-gray-300 mb-6 leading-relaxed">
                            I enjoy working on end-to-end projects — from data preprocessing and model training to
                            deployment with scalable backends and web interfaces. Along the way, I’ve gained hands-on
                            experience with technologies like TensorFlow, PyTorch, LangChain, LangGraph, FastAPI, Flask,
                            React, and PostgreSQL, as well as cloud platforms such as AWS and GCP.
                        </p>
                        <p>Beyond technical skills, I bring strong problem-solving abilities, a curiosity-driven
                            mindset, and a constant drive to learn, innovate, and deliver impactful AI solutions.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Work Experience Section -->
        <section id="experience" class="py-20 md:py-20 bg-gray-900">
            <h2 class="text-4xl font-bold text-white text-center mb-16">Work Experience</h2>
            <div class="max-w-3xl mx-auto">
                <div class="space-y-8">
                    <div class="glass-effect p-6 rounded-lg">
                        <div class="flex justify-between items-start">
                            <div>
                                <h3 class="text-xl font-bold text-white">AI/ML Intern</h3>
                                <p class="text-blue-400">Codelab Systems, Mangalore</p>
                            </div>
                            <p class="text-gray-400">March 2025 - July 2025</p>
                        </div>
                        <ul class="mt-4 text-gray-300 list-disc list-inside space-y-2">
                            <li>During my internship, I designed and implemented an AI-powered chatbot leveraging
                                LangChain and Retrieval-Augmented Generation (RAG) to provide accurate, context-aware
                                responses. I built a custom knowledge base by integrating vector databases and document
                                embeddings, enabling the chatbot to retrieve relevant information before generating
                                responses. The system was optimized for low-latency query handling and included features
                                like conversation history management and fallback mechanisms for unanswered queries.
                            </li>
                            <li>This project gave me hands-on experience with LLM orchestration, vector search, prompt
                                engineering, and API integration, while strengthening my understanding of end-to-end AI
                                product development. It also improved my ability to design scalable architectures that
                                combine machine learning models with real-world applications</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Education Section -->
        <section id="education" class="py-20 md:py-20">
            <h2 class="text-4xl font-bold text-white text-center mb-16">Education</h2>
            <div class="max-w-3xl mx-auto">
                <div class="space-y-8">
                    <div class="glass-effect p-6 rounded-lg">
                        <div class="flex justify-between items-start">
                            <div>
                                <h3 class="text-xl font-bold text-white">Masters of Science, Computer Science</h3>
                                <p class="text-blue-400">Mangalore University</p>
                            </div>
                            <p class="text-gray-400">August 2025</p>
                        </div>
                        <p class="mt-2 text-gray-300">CGPA: 8.5</p>
                    </div>
                    <div class="glass-effect p-6 rounded-lg">
                        <div class="flex justify-between items-start">
                            <div>
                                <h3 class="text-xl font-bold text-white">Bachelor of Science, PMCs</h3>
                                <p class="text-blue-400">Mangalore University</p>
                            </div>
                            <p class="text-gray-400">August 2023</p>
                        </div>
                        <p class="mt-2 text-gray-300">CGPA: 8.33</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section id="projects" class="py-20 md:py-20">
            <h2 class="text-4xl font-bold text-white text-center mb-16">My Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project Card 1 -->
                <div class="project-card glass-effect rounded-lg overflow-hidden shadow-lg">
                    <img src="images/tweet.png" alt="Project 3" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">Automated Tweet Generator with Multi-Agent
                            Workflow | LangChain, LangGraph, FastAPI, PostgreSQL</h3>
                        <a href="https://github.com/pravigowda18/tweet-generator-langgraph-faastapi" target="_blank"
                            rel="noopener noreferrer" class="text-blue-400 hover:underline font-semibold">View on GitHub
                            &rarr;</a>
                        <div class="project-details collapsible-content mt-4">
                            <p class="text-gray-300">Developed an AI-powered tweet generation system using LangChain and
                                LangGraph, featuring multi-agent orchestration with conditional edges and a
                                human-in-the-loop (HITL) mechanism for controlled content approval. <br>
                                Implemented persistence with PostgreSQL to manage agent states, user feedback, and
                                workflow execution history. <br>
                                Built the backend with FastAPI, integrating JWT and OAuth authentication for secure user
                                access and role-based control. <br>
                                Designed the system to allow automated tweet creation while enabling human
                                review/override, ensuring both scalability and accountability. <br>
                                Delivered an end-to-end project combining AI-driven text generation, HITL workflow
                                management, and production-ready backend with database persistence</p>
                        </div>
                    </div>
                </div>
                <!-- Project Card 2 -->
                <div class="project-card glass-effect rounded-lg overflow-hidden shadow-lg">
                    <img src="images/atm.png" alt="Project 2" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">AI-Powered ATM Surveillance System | YOLOv8,
                            Flask, OpenCV</h3>
                        <a href="https://github.com/pravigowda18/yolo-atm-security" target="_blank"
                            rel="noopener noreferrer" class="text-blue-400 hover:underline font-semibold">View on GitHub
                            &rarr;</a>
                        <div class="project-details collapsible-content mt-4">
                            <p class="text-gray-300">Built a real-time surveillance system to enhance ATM security by
                                detecting individuals wearing helmets or masks and blocking transactions if the face is
                                obscured. <br>
                                Trained a custom YOLOv8 model on a labeled dataset, achieving >90% mAP@0.5 with robust
                                detection under varying lighting conditions. <br>
                                Integrated with Flask backend and a web interface (HTML, CSS, JavaScript) for real-time
                                monitoring, alerts, and transaction control</p>
                        </div>
                    </div>
                </div>
                <!-- Project Card 3 -->
                <div class="project-card glass-effect rounded-lg overflow-hidden shadow-lg">
                    <img src="images/hand.png" alt="Project 3" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">Real-Time Hand Gesture Recognition | MediaPipe,
                            OpenCV, NumPy</h3>
                        <a href="https://github.com/pravigowda18/real-time-hand-gesture-recognition" target="_blank"
                            rel="noopener noreferrer" class="text-blue-400 hover:underline font-semibold">View on GitHub
                            &rarr;</a>
                        <div class="project-details collapsible-content mt-4">
                            <p class="text-gray-300">Developed a real-time hand gesture recognition system capable of
                                detecting and classifying four static gestures: ✋ Open Palm, ✊ Fist, ✌️ Peace Sign, and
                                👍 Thumbs Up. <br>
                                Utilized MediaPipe Hands to extract 21 hand landmarks with high precision and applied
                                custom gesture logic for classification based on finger openness/closure. <br>
                                Integrated with OpenCV for live webcam feed, gesture overlay, and bounding box
                                visualization. <br>
                                Achieved accurate real-time detection (>30 FPS) on CPU without requiring GPU
                                acceleration.</p>
                        </div>
                    </div>
                </div>
                <!-- Project Card 4 -->
                <div class="project-card glass-effect rounded-lg overflow-hidden shadow-lg">
                    <img src="images/car.png" alt="Project 1" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">License Plate Recognition Web App | YOLOv8,
                            PaddleOCR, Flask, JSON</h3>
                        <a href="https://github.com/pravigowda18/Automatic-Car-Number-Plate-Recognition-with-PaddleOCR"
                            target="_blank" rel="noopener noreferrer"
                            class="text-blue-400 hover:underline font-semibold">View on GitHub &rarr;</a>
                        <div class="project-details collapsible-content mt-4">
                            <p class="text-gray-300">Built a web-based application to detect and recognize vehicle
                                license plates from images and live video.
                                Implemented YOLOv8 for license plate detection and PaddleOCR for text recognition.
                                Matched recognized plates against a JSON database to retrieve owner details.
                                Developed Flask backend to serve predictions and integrated frontend for displaying
                                results.
                                Delivered a real-time recognition pipeline suitable for parking systems and traffic
                                monitoring.</p>
                        </div>
                    </div>
                </div>
                <!-- Project Card 5 -->
                <div class="project-card glass-effect rounded-lg overflow-hidden shadow-lg">
                    <img src="images/right.png" alt="Project 3" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">Virtual Mouse Using Hand Gestures | MediaPipe,
                            OpenCV, PyAutoGUI, Python</h3>
                        <a href="https://github.com/pravigowda18/hand-tracked-virtual-mouse" target="_blank"
                            rel="noopener noreferrer" class="text-blue-400 hover:underline font-semibold">View on GitHub
                            &rarr;</a>
                        <div class="project-details collapsible-content mt-4">
                            <p class="text-gray-300">Developed a Python-based virtual mouse that enables full cursor
                                control and click actions using real-time hand gestures, eliminating the need for a
                                physical mouse. <br>
                                Implemented MediaPipe Hands for precise landmark detection and mapped finger positions
                                to cursor movement, left-click, and right-click gestures. <br>
                                Integrated OpenCV for live webcam feed with visual overlays and applied gesture logic
                                with click cooldowns to prevent false triggers. <br>
                                Achieved smooth real-time performance with accurate tracking and gesture execution on
                                standard CPU hardware.</p>
                        </div>
                    </div>
                </div>
                <!-- Project Card 6 -->
                <div class="project-card glass-effect rounded-lg overflow-hidden shadow-lg">
                    <img src="images/catdog.png" alt="Project 3" class="w-full h-56 object-cover">
                    <div class="p-6">
                        <h3 class="text-xl font-bold text-white mb-2">Cat vs Dog Image Classification | TensorFlow, CNN,
                            Keras, OpenCV</h3>
                        <a href="https://github.com/pravigowda18/cat-vs-dog-prediction" target="_blank"
                            rel="noopener noreferrer" class="text-blue-400 hover:underline font-semibold">View on GitHub
                            &rarr;</a>
                        <div class="project-details collapsible-content mt-4">
                            <p class="text-gray-300">Built a deep learning model to classify images of cats and dogs
                                using a Convolutional Neural Network (CNN) trained on the Kaggle Dogs vs. Cats dataset.
                                <br>
                                Implemented data preprocessing and augmentation with TensorFlow/Keras to improve
                                generalization and reduce overfitting. <br>
                                Achieved ~90% classification accuracy on the test set with optimized CNN architecture.
                                Integrated OpenCV for image preprocessing and real-time image predictions. <br>
                                Designed the project with modular scripts for training, evaluation, and inference,
                                making it easily extendable to other image classification tasks.
                            </p>
                        </div>
                    </div>
                </div>

            </div>
        </section>

        <!-- Skills Section -->
        <Section class="py-20 md:mx-32 md:py-20 bg-gray-900">
            <div class="mt-16">
                <h3 class="text-3xl font-bold text-white text-center mb-12">My Skillset</h3>
                <div class="space-y-8">
                    <div>
                        <h4 class="text-2xl font-semibold text-white mb-4">Core Technologies & Programming</h4>
                        <div class="flex flex-wrap gap-3">
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Python</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Data Structures &
                                Algorithms</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Git</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">GitHub</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Object-Oriented
                                Programming</span>
                        </div>
                    </div>
                    <div>
                        <h4 class="text-2xl font-semibold text-white mb-4">Machine Learning & AI</h4>
                        <div class="flex flex-wrap gap-3">
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Supervised & Unsupervised
                                Learning</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Model Evaluation</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">PyTorch</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">TensorFlow</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">NumPy</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Pandas</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Matplotlib</span>
                        </div>
                    </div>
                    <div>
                        <h4 class="text-2xl font-semibold text-white mb-4">Generative AI</h4>
                        <div class="flex flex-wrap gap-3">
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Large Language Models</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">LangChain</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Embeddings & Vector
                                Databases</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Retrieval-Augmented
                                Generation</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">LangGraph</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Persistence</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Human-in-loop</span>
                        </div>
                    </div>
                    <div>
                        <h4 class="text-2xl font-semibold text-white mb-4">Backend Development</h4>
                        <div class="flex flex-wrap gap-3">
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">FastAPI</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">RESTful API</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">MySQL, PostgreSQL,
                                MongoDB</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Authentication & Authorization
                                (OAuth2, JWT)</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Docker</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">CI/CD (basic)</span>
                        </div>
                    </div>
                    <div>
                        <h4 class="text-2xl font-semibold text-white mb-4">Computer Vision</h4>
                        <div class="flex flex-wrap gap-3">
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">OpenCV</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">CNNs</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">YOLO</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Transfer Learning</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Object Detection</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Image Classification</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Segmentation</span>
                            <span class="bg-gray-700 text-gray-200 py-2 px-4 rounded-lg">Vision Transformers</span>
                        </div>
                    </div>
                </div>
            </div>
        </Section>

        <!-- Contact Section -->
        <section id="contact" class="py-20 md:py-20 text-center">
            <h2 class="text-4xl font-bold text-white mb-4">Get In Touch</h2>
            <p class="text-gray-400 max-w-2xl mx-auto mb-12">
                I'm currently open to new opportunities and collaborations. Whether you have a question or just want to
                say hi, feel free to reach out. I'll get back to you as soon as I can!
            </p>
            <div class="flex flex-col md:flex-row justify-center items-center gap-8">
                <a href="mailto:pravisb0002@gmail.com"
                    class="inline-flex items-center gap-3 bg-gray-700 hover:bg-gray-600 text-white font-semibold py-3 px-6 rounded-lg transition duration-300">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                        <path
                            d="M22 6c0-1.1-.9-2-2-2H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6zm-2 0l-8 5-8-5h16zm0 12H4V8l8 5 8-5v10z" />
                    </svg>
                    pravisb0002@gmail.com
                </a>
                <a href="tel:+919740654075"
                    class="inline-flex items-center gap-3 bg-gray-700 hover:bg-gray-600 text-white font-semibold py-3 px-6 rounded-lg transition duration-300">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                        <path
                            d="M6.62 10.79a15.053 15.053 0 006.59 6.59l2.2-2.2c.27-.27.67-.36 1.02-.24 1.12.37 2.33.57 3.57.57.55 0 1 .45 1 1V20c0 .55-.45 1-1 1-9.39 0-17-7.61-17-17 0-.55.45-1 1-1h3.5c.55 0 1 .45 1 1 0 1.25.2 2.45.57 3.57.11.35.02.74-.25 1.02l-2.2 2.2z" />
                    </svg>
                    +91 9740654075
                </a>
                <a href="https://github.com/pravigowda18"
                    class="inline-flex items-center gap-3 bg-gray-700 hover:bg-gray-600 text-white font-semibold py-3 px-6 rounded-lg transition duration-300">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                        <path
                            d="M12 2C6.477 2 2 6.477 2 12c0 4.418 2.865 8.165 6.839 9.489.5.092.682-.218.682-.482 0-.237-.009-.868-.014-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.031-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.03 1.595 1.03 2.688 0 3.848-2.338 4.695-4.566 4.942.359.308.678.92.678 1.852 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.001 10.001 0 0022 12c0-5.523-4.477-10-10-10z" />
                    </svg>
                    pravigowda18
                </a>
                <a href="https://www.linkedin.com/in/praveens182002"
                    class="inline-flex items-center gap-3 bg-gray-700 hover:bg-gray-600 text-white font-semibold py-3 px-6 rounded-lg transition duration-300">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                        <path
                            d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z" />
                    </svg>
                    praveens182002
                </a>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="border-t border-gray-800">
        <div
            class="container mx-auto px-6 py-8 flex flex-col md:flex-row justify-between items-center text-center md:text-left">
            <p class="text-gray-500">&copy; 2025 Praveen S. All Rights Reserved.</p>
            <div class="flex space-x-6 mt-4 md:mt-0">
                <a href="https://github.com/pravigowda18" target="_blank" rel="noopener noreferrer"
                    class="text-gray-400 hover:text-white transition">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                        <path fill-rule="evenodd"
                            d="M12 2C6.477 2 2 6.477 2 12c0 4.418 2.865 8.165 6.839 9.489.5.092.682-.218.682-.482 0-.237-.009-.868-.014-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.031-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.03 1.595 1.03 2.688 0 3.848-2.338 4.695-4.566 4.942.359.308.678.92.678 1.852 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.001 10.001 0 0022 12c0-5.523-4.477-10-10-10z"
                            clip-rule="evenodd" />
                    </svg>
                </a>
                <a href="https://www.linkedin.com/in/praveens182002" target="_blank" rel="noopener noreferrer"
                    class="text-gray-400 hover:text-white transition">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                        <path
                            d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z" />
                    </svg>
                </a>
                <a href="#" class="text-gray-400 hover:text-white transition">
                    <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                        <path
                            d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616v.064c0 2.298 1.634 4.212 3.793 4.649-.65.177-1.353.23-2.074.195.599 1.884 2.338 3.256 4.404 3.292-1.816 1.423-4.094 2.19-6.49 2.054 2.029 1.352 4.467 2.152 7.048 2.152 8.434 0 12.986-7.011 12.823-13.254 1.062-.765 1.875-1.725 2.484-2.848z" />
                    </svg>
                </a>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            // Typing effect
            const typingText = document.getElementById('typing-text');
            const words = ["AI/ML Engineer", "Computer Vision Specialist", "Python Developer", "Data Scientist", "Backend Developer"];
            let wordIndex = 0;
            let charIndex = 0;
            let isDeleting = false;

            function type() {
                const currentWord = words[wordIndex];
                if (isDeleting) {
                    typingText.textContent = currentWord.substring(0, charIndex - 1);
                    charIndex--;
                } else {
                    typingText.textContent = currentWord.substring(0, charIndex + 1);
                    charIndex++;
                }

                if (!isDeleting && charIndex === currentWord.length) {
                    setTimeout(() => isDeleting = true, 2000);
                } else if (isDeleting && charIndex === 0) {
                    isDeleting = false;
                    wordIndex = (wordIndex + 1) % words.length;
                }

                const typeSpeed = isDeleting ? 100 : 200;
                setTimeout(type, typeSpeed);
            }
            type();

            // Header scroll effect
            const header = document.getElementById('header');
            window.addEventListener('scroll', () => {
                if (window.scrollY > 50) {
                    header.classList.add('glass-effect', 'shadow-lg');
                } else {
                    header.classList.remove('glass-effect', 'shadow-lg');
                }
            });

            // Mobile menu toggle
            const mobileMenuBtn = document.getElementById('mobile-menu-btn');
            const mobileMenu = document.getElementById('mobile-menu');
            const mobileMenuLinks = document.querySelectorAll('.mobile-menu-link');

            mobileMenuBtn.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });

            mobileMenuLinks.forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });

            // Project card details toggle for desktop via mouseover
            const projectCards = document.querySelectorAll('.project-card');
            projectCards.forEach(card => {
                const details = card.querySelector('.project-details');
                if (details && window.innerWidth >= 768) { // 768px is md breakpoint
                    card.addEventListener('mouseenter', () => {
                        details.classList.add('expanded');
                    });
                    card.addEventListener('mouseleave', () => {
                        details.classList.remove('expanded');
                    });
                }
            });
        });
    </script>
</body>

</html>
