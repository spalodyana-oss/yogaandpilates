<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LODYana Spa - Signature Yoga Pilates Packages</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- New Attractive Palette: Deep Teal & Soft Coral --><!-- Application Structure Plan: Retained the single vertical flow with an interactive tab system. Header -> Introduction -> Interactive Controls (Tabs) -> Dynamic Content Area (Package Cards) -> New "Contact Us" Button (WhatsApp Link) -> Comparative Visualization (Chart) -> Terms & Conditions Button (New Modal) -> Footer. --><script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            bg: '#fbfcfd', // Very light, almost white background
                            text: '#2c3e50', // Darker, professional text (deep charcoal/blue-grey)
                            primary: '#1abc9c', // Deep Teal - Main accent
                            'primary-light': '#a1e4d5', // Lighter Teal for inactive elements/hover
                            secondary: '#e74c3c', // Soft Coral - for attention, e.g., chart highlight, potentially hover
                            muted: '#e0e6ea', // Light grey for borders, inactive chart bars
                            card: '#ffffff',
                            border: '#e0e6ea', // Light grey border
                        }
                    }
                }
            }
        }
    </script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #fbfcfd;
            color: #2c3e50;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 250px;
            max-height: 300px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 300px;
            }
        }
        .tab-button {
            transition: all 0.3s ease;
            border: 2px solid transparent;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05); /* Softer shadow for buttons */
        }
        /* New attractive tab style */
        .tab-button.active {
            background-color: #1abc9c; /* Deep Teal */
            color: #ffffff;
            box-shadow: 0 4px 15px rgba(26, 188, 156, 0.4); /* Stronger shadow for active */
        }
        .tab-button:not(.active) {
            background-color: #ffffff; /* White background for inactive */
            color: #2c3e50;
        }
        .tab-button:not(.active):hover {
            background-color: #f0f4f7; /* Very light grey on hover */
            color: #1abc9c; /* Teal text on hover */
            border-color: #a1e4d5; /* Light teal border on hover */
        }
        .package-card {
            transition: opacity 0.4s ease-in-out, transform 0.4s ease-in-out;
            will-change: opacity, transform;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08); /* More prominent shadow for cards */
        }
        .package-card.hidden {
            opacity: 0;
            transform: scale(0.98);
            pointer-events: none;
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
        }
    </style>
</head>
<body class="bg-brand-bg text-brand-text">

    <div class="container mx-auto p-4 md:p-8 max-w-4xl">
        
        <header class="text-center mb-6 md:mb-12">
            <!-- UPDATED TITLE -->
            <h1 class="text-3xl md:text-5xl font-bold text-brand-primary">Special YOGA Pilates Membership Packages</h1>
            <p class="text-xl md:text-2xl font-light text-brand-text mt-1 md:mt-2">UNVEIL YOUR STRENGTH. CULTIVATE YOUR PEACE.</p>
            <p class="text-base font-light text-brand-text/70 mt-1">“Achieve Flexibility and Strength”</p>
        </header>

        <main>
            <section id="intro" class="text-center max-w-2xl mx-auto mb-6 md:mb-10">
                <!-- UPDATED INTRO CONTENT -->
                <p class="text-base md:text-lg text-brand-text/90">
                    At LODYana Spa, we believe true beauty radiates from within. Our exclusive Yoga Pilates packages are meticulously designed to harmonize your body and mind, blending ancient practices with modern wellness.
                </p>
            </section>

            <section id="package-explorer">
                <div class="flex justify-center flex-wrap gap-2 md:gap-4 my-6">
                    <button id="btn-3" data-pkg="pkg-3" class="tab-button active text-sm md:text-lg font-semibold py-2 px-4 md:py-3 md:px-10 rounded-full">
                        3 Months
                    </button>
                    <button id="btn-6" data-pkg="pkg-6" class="tab-button text-sm md:text-lg font-semibold py-2 px-4 md:py-3 md:px-10 rounded-full">
                        6 Months
                    </button>
                    <button id="btn-12" data-pkg="pkg-12" class="tab-button text-sm md:text-lg font-semibold py-2 px-4 md:py-3 md:px-10 rounded-full">
                        12 Months
                    </button>
                </div>

                <div id="package-details" class="relative min-h-[400px] md:min-h-[380px]">
                    
                    <!-- UPDATED 3-MONTH PACKAGE -->
                    <div id="pkg-3" class="package-card bg-brand-card rounded-xl p-4 md:p-8 border border-brand-border">
                        <h2 class="text-xl md:text-3xl font-bold text-brand-primary mb-3">The 3-Month Transformation</h2>
                        <p class="text-base md:text-xl font-semibold text-brand-text/80 mb-2">3 sessions per week (Private or Group)</p>
                        <p class="text-3xl md:text-4xl font-bold text-brand-text mb-4">د.إ 2299 <span class="text-base font-normal">dhs</span></p>
                        <h3 class="text-lg md:text-xl font-bold text-brand-secondary mb-3">Package Includes:</h3>
                        <ul class="space-y-2 text-sm md:text-lg text-brand-text/90 list-disc pl-5">
                            <li><strong class="text-brand-text">3 months</strong> of personalized sessions</li>
                            <li><strong class="text-brand-secondary font-bold">BONUS:</strong> 1 FREE Signature Madero treatment</li>
                        </ul>
                    </div>
                    
                    <!-- UPDATED 6-MONTH PACKAGE -->
                    <div id="pkg-6" class="package-card hidden bg-brand-card rounded-xl p-4 md:p-8 border border-brand-border">
                        <h2 class="text-xl md:text-3xl font-bold text-brand-primary mb-3">The 6-Month Radiance</h2>
                        <p class="text-base md:text-xl font-semibold text-brand-text/80 mb-2">3 sessions per week (Private or Group)</p>
                        <p class="text-3xl md:text-4xl font-bold text-brand-text mb-4">د.إ 2599 <span class="text-base font-normal">dhs</span></p>
                        <h3 class="text-lg md:text-xl font-bold text-brand-secondary mb-3">Package Includes:</h3>
                        <ul class="space-y-2 text-sm md:text-lg text-brand-text/90 list-disc pl-5">
                            <li><strong class="text-brand-text">6 months</strong> of dedicated practice</li>
                            <li><strong class="text-brand-secondary font-bold">BONUS:</strong> FREE Madero and EMS treatment</li>
                        </ul>
                    </div>

                    <!-- UPDATED 12-MONTH PACKAGE WITH REVISED BONUS -->
                    <div id="pkg-12" class="package-card hidden bg-brand-card rounded-xl p-4 md:p-8 border border-brand-border">
                        <h2 class="text-xl md:text-3xl font-bold text-brand-primary mb-3">The 12-Month Harmony</h2>
                        <p class="text-base md:text-xl font-semibold text-brand-text/80 mb-2">3 sessions per week (Private or Group)</p>
                        <p class="text-3xl md:text-4xl font-bold text-brand-text mb-4">د.إ 3999 <span class="text-base font-normal">dhs</span></p>
                        <h3 class="text-lg md:text-xl font-bold text-brand-secondary mb-3">Package Includes:</h3>
                        <ul class="space-y-2 text-sm md:text-lg text-brand-text/90 list-disc pl-5">
                            <li><strong class="text-brand-text">12 months</strong> of continuous wellness</li>
                            <li><strong class="text-brand-secondary font-bold">BONUS:</strong> Healthy program follow-up & weight management</li>
                            <li><strong class="text-brand-secondary font-bold">BONUS:</strong> FREE LODYana Signature (with Kizhi) and Moxa Tui-Na Therapy</li>
                        </ul>
                    </div>

                </div>
            </section>

            <!-- Contact Button -->
            <section id="learn-more" class="text-center mt-8 md:mt-16">
                <a id="btn-learn-more" href="https://wa.me/971529353900" target="_blank" class="inline-block bg-white text-brand-primary font-semibold py-3 px-8 border-2 border-brand-primary rounded-full text-base md:text-lg shadow-md hover:bg-brand-primary hover:text-white transition-all duration-300 ease-in-out">
                    To know more about Yoga Pilates Contact Us
                </a>
            </section>

            <section id="visualization" class="mt-8 md:mt-16">
                <h2 class="text-xl md:text-3xl font-bold text-center text-brand-text">
                    Package Value Comparison
                </h2>
                <p class="text-center text-sm md:text-lg text-brand-text/80 max-w-xl mx-auto mt-2 mb-4 md:mb-6">
                    This chart illustrates the average cost per session. Longer-term packages provide greater value by reducing your per-session investment.
                </p>
                <div class="chart-container">
                    <canvas id="valueChart"></canvas>
                </div>
            </section>

            <!-- Terms & Conditions Button -->
            <section id="terms-section" class="text-center mt-6 md:mt-8">
                <button id="btn-terms" class="inline-block bg-white text-brand-text font-semibold py-2 px-6 border border-brand-muted rounded-full text-sm md:text-base hover:bg-brand-muted transition-all duration-300 ease-in-out">
                    View Full Terms & Conditions
                </button>
            </section>

        </main>

        <footer class="text-center mt-8 md:mt-16 pt-6 md:pt-8 border-t border-brand-border">
            <p class="text-xs md:text-base text-brand-text/70">
                Freeze Policy Note: All package freeze periods can be used together or separately to accommodate your schedule.
            </p>
            <p class="text-base md:text-lg font-semibold text-brand-primary mt-3 md:mt-4">
                Please Contact LODYana Healing and Wellness Center
            </p>
            <!-- UPDATED: Reduced font size and refined alignment -->
            <div class="flex flex-col md:flex-row justify-center items-center gap-3 mt-2 md:mt-3 text-sm md:text-base">
                <!-- WhatsApp Link -->
                <a href="https://wa.me/971529353900" target="_blank" class="inline-flex items-center space-x-1 font-semibold text-brand-text hover:text-brand-primary transition duration-300">
                    <span class="text-lg text-brand-primary">&#x1F4F1;</span>
                    <span>WhatsApp: +971 52 935 3900</span>
                </a>

                <!-- Separator (hidden on mobile) -->
                <span class="hidden md:inline-block text-brand-muted">|</span>

                <!-- Location Link -->
                <a href="https://maps.app.goo.gl/Xhzyor6M8dm4yDxf6" target="_blank" class="inline-flex items-center space-x-1 font-semibold text-brand-text hover:text-brand-primary transition duration-300">
                    <span class="text-lg text-brand-primary">&#x1F4CD;</span> <!-- Map Pin Emoji -->
                    <span>Al Sahel Towers, Corniche Abu Dhabi</span>
                </a>
            </div>
        </footer>

    </div>

    <!-- Learn More Modal - I've kept the original content here as it still discusses the benefits of your wellness approach. -->
    <div id="infoModal" class="fixed inset-0 z-50 hidden bg-brand-text/80 backdrop-blur-sm overflow-y-auto p-2 md:p-4 transition-opacity duration-300">
        <!-- Max width set to w-full for mobile, smaller margin top/bottom on mobile (my-4) -->
        <div class="relative bg-brand-card rounded-xl shadow-2xl w-full max-w-md md:max-w-3xl mx-auto my-4 md:my-10 p-4 md:p-10">
            <button id="closeModalBtn" class="absolute top-3 right-3 md:top-4 md:right-4 text-brand-text hover:text-brand-secondary text-4xl font-light transition leading-none">
                &times;
            </button>
            <h2 class="text-xl md:text-3xl font-bold text-brand-primary mb-4 border-b pb-2 border-brand-primary/30">The Transformative Power of Yoga Pilates</h2>
            
            <div class="space-y-4 md:space-y-6 text-sm md:text-lg text-brand-text/90">
                <p>At LODYana Healing and Wellness Center, we harness the profound synergy of **Yoga and Pilates**—a fusion proven to restore core strength, flexibility, and mind-body connection. This practice views true beauty as an expression of internal harmony and physical grace.</p>

                <h3 class="text-lg md:text-xl font-semibold text-brand-text border-l-4 border-brand-primary pl-3">Achieve Core Strength and Toning</h3>
                <p>By focusing on **deep core engagement** (a Pilates principle), combined with the **flexibility and flow** of Yoga, our sessions promote long, lean muscle definition and improved posture. This process enhances stability and reduces the risk of injury.</p>

                <h3 class="text-lg md:text-xl font-semibold text-brand-text border-l-4 border-brand-primary pl-3">Stress Mastery Through Breath</h3>
                <p>The core of this combined practice is the intentional regulation of the nervous system using advanced **breathing techniques**. This dramatically lowers levels of **Cortisol**, the primary aging and weight-gaining hormone, leading to a state of profound calm.</p>

                <h3 class="text-lg md:text-xl font-semibold text-brand-text border-l-4 border-brand-primary pl-3">Enhanced Vitality and Focus</h3>
                <p>This deep internal reset clears mental fatigue and confusion, leading to superior **mental clarity** and a tangible boost in energy. Our high-profile clients benefit from this heightened focus, which translates directly to better performance in their demanding lives.</p>
            
                <h2 class="text-xl md:text-2xl font-bold text-brand-primary pt-4 md:pt-6 border-t mt-4 md:mt-6 border-brand-primary/30">LODYana Healing and Wellness Center: The Power of Inside Out Beauty</h2>
                <p>Our core belief is **Inside Out Beauty**. We understand that true radiance is a reflection of internal health. Our philosophy is rooted in the powerful synergy of ancient wisdom and modern cosmetic science, addressing both your physical appearance and your essential well-being.</p>

                <h3 class="text-base md:text-xl font-semibold text-brand-text border-l-4 border-brand-primary pl-3">The Tree of Life: Our Transformative Journey</h3>
                <p>The **Tree of Life** symbolizes your LODYana journey. The roots represent your **inner soul and well-being**, which we nourish through our focused relaxation sessions. The strong trunk is your **body**, expertly refined and toned by our luxurious manual and cutting-edge machine treatments. The branches and leaves are your **outward manifestation**—the flawless skin, revitalized hair, and contoured body. Our treatments ensure that this brilliance is not temporary, but is robustly supported from the inside out.</p>

                <h3 class="text-base md:text-xl font-semibold text-brand-text border-l-4 border-brand-primary pl-3">A Unique Blend of Luxury and Healing</h3>
                <p>We distinguish ourselves by seamlessly integrating these deeply centering practices into your exclusive spa experience. Every luxurious treatment, from our advanced facials to our bespoke body contouring, is preceded by a personalized session designed to immediately **calm the nervous system**. This intentional blend prepares your muscles, skin, and mind for **maximum therapeutic benefit**, ensuring you absorb the full, luxurious potential of the service. You leave not only looking exquisite but feeling profoundly centered, vital, and transformed.</p>
            </div>
        </div>
    </div>
    <!-- End Learn More Modal -->

    <!-- Terms & Conditions Modal -->
    <div id="termsModal" class="fixed inset-0 z-50 hidden bg-brand-text/80 backdrop-blur-sm overflow-y-auto p-2 md:p-4 transition-opacity duration-300">
        <div class="relative bg-brand-card rounded-xl shadow-2xl w-full max-w-md md:max-w-3xl mx-auto my-4 md:my-10 p-4 md:p-10">
            <button id="closeTermsModalBtn" class="absolute top-3 right-3 md:top-4 md:right-4 text-brand-text hover:text-brand-secondary text-4xl font-light transition leading-none">
                &times;
            </button>
            <h2 class="text-xl md:text-3xl font-bold text-brand-secondary mb-4 border-b pb-2 border-brand-secondary/30">Package Terms & Conditions</h2>
            
            <div class="space-y-4 md:space-y-5 text-sm md:text-base text-brand-text/90">
                
                <p><strong class="font-semibold text-brand-text">Non-Transferable & Non-Refundable:</strong> All package purchases are final, non-refundable, and non-transferable to any other person or account.</p>

                <p><strong class="font-semibold text-brand-text">Activation:</strong> The package validity begins on the date of purchase or the date of the first class attended, whichever comes sooner.</p>
                
                <p><strong class="font-semibold text-brand-text">Usage:</strong> The package entitles the member to a maximum of 3 classes per week. Unused sessions from one week or month will not roll over to the next period.</p>

                <p><strong class="font-semibold text-brand-text">Expiration:</strong> All package benefits expire automatically at the end of the stated duration.</p>

                <p><strong class="font-semibold text-brand-text">Strict Adherence (Freeze Policy):</strong> Any attempt to extend the package or delay beyond the maximum allowed freeze time (2 weeks for 3/6-month packages, 4 weeks for 12-month packages) will result in the immediate forfeiture of all remaining classes and benefits.</p>

                <p><strong class="font-semibold text-brand-text">Bonus Treatments:</strong> All complimentary treatments (Madero, EMS, LODYana Signature, Moxa Tui-Na, etc.) must be booked and utilized within the package's active, un-frozen validity period. They cannot be exchanged for cash, credit, or package extensions if unused.</p>

                <p><strong class="font-semibold text-brand-text">Pre-Booking:</strong> All classes must be pre-booked.</p>
            </div>
        </div>
    </div>
    <!-- End Terms & Conditions Modal -->

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            
            const buttons = document.querySelectorAll('.tab-button');
            const cards = document.querySelectorAll('.package-card');
            const ctx = document.getElementById('valueChart').getContext('2d');

            // Modal elements
            const learnMoreButton = document.getElementById('btn-learn-more');
            const infoModal = document.getElementById('infoModal');
            const closeModalBtn = document.getElementById('closeModalBtn');
            
            // Terms Modal elements
            const termsButton = document.getElementById('btn-terms');
            const termsModal = document.getElementById('termsModal');
            const closeTermsModalBtn = document.getElementById('closeTermsModalBtn');

            // Updated chart colors for attractive theme
            const chartColors = {
                active: '#1abc9c', // Deep Teal
                inactive: '#e0e6ea' // Light grey
            };

            // Calculate sessions: 3 sessions/week * weeks/package
            // 3 Months: ~13 weeks = 39 sessions. Price: 2299. Avg Cost: 2299 / 39 = 58.95
            // 6 Months: ~26 weeks = 78 sessions. Price: 2599. Avg Cost: 2599 / 78 = 33.32
            // 12 Months: ~52 weeks = 156 sessions. Price: 3999. Avg Cost: 3999 / 156 = 25.63
            const chartData = {
                'pkg-3': 58.95, 
                'pkg-6': 33.32, 
                'pkg-12': 25.63 
            };
            
            const valueChart = new Chart(ctx, {
                type: 'bar',
                data: {
                    labels: ['3 Months', '6 Months', '12 Months'],
                    datasets: [{
                        label: 'Avg. Cost per Session (Dhs)',
                        data: [chartData['pkg-3'], chartData['pkg-6'], chartData['pkg-12']],
                        backgroundColor: [
                            chartColors.active, 
                            chartColors.inactive, 
                            chartColors.inactive
                        ],
                        borderColor: '#ffffff',
                        borderWidth: 2,
                        borderRadius: 4
                    }]
                },
                options: {
                    indexAxis: 'y',
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        legend: {
                            display: false
                        },
                        tooltip: {
                            callbacks: {
                                label: function(context) {
                                    return ` ${context.dataset.label}: ${context.raw.toFixed(2)} Dhs`;
                                }
                            }
                        }
                    },
                    scales: {
                        x: {
                            beginAtZero: true,
                            title: {
                                display: true,
                                text: 'Avg. Cost per Session (Dhs)',
                                font: {
                                    size: 14
                                },
                                color: '#555555'
                            },
                            grid: {
                                display: true,
                                color: '#eeeeee'
                            },
                            ticks: {
                                color: '#555555'
                            }
                        },
                        y: {
                            grid: {
                                display: false
                            },
                            ticks: {
                                font: {
                                    size: 14,
                                    weight: '500'
                                },
                                color: '#333333'
                            }
                        }
                    }
                }
            });

            function updateTabs(activeButton) {
                buttons.forEach(button => {
                    button.classList.remove('active');
                });
                activeButton.classList.add('active');
            }

            function updateCards(selectedPkgId) {
                cards.forEach(card => {
                    if (card.id === selectedPkgId) {
                        card.classList.remove('hidden');
                    } else {
                        card.classList.add('hidden');
                    }
                });
            }

            function updateChartHighlight(selectedPkgId) {
                const newColors = [
                    selectedPkgId === 'pkg-3' ? chartColors.active : chartColors.inactive,
                    selectedPkgId === 'pkg-6' ? chartColors.active : chartColors.inactive,
                    selectedPkgId === 'pkg-12' ? chartColors.active : chartColors.inactive,
                ];
                valueChart.data.datasets[0].backgroundColor = newColors;
                valueChart.update();
            }

            buttons.forEach(button => {
                button.addEventListener('click', () => {
                    const selectedPkg = button.dataset.pkg;
                    
                    updateTabs(button);
                    updateCards(selectedPkg);
                    updateChartHighlight(selectedPkg);
                });
            });

            // Modal Logic (Learn More)
            learnMoreButton.addEventListener('click', (e) => {
                // Since the new button is a WhatsApp link, we don't open the modal by default.
                // If you wish to show the modal AND link to WhatsApp, you will need to add a separate modal button.
                // For now, I'm prioritizing the WhatsApp link.
                // e.preventDefault(); 
                // infoModal.classList.remove('hidden');
            });

            closeModalBtn.addEventListener('click', () => {
                infoModal.classList.add('hidden');
            });

            infoModal.addEventListener('click', (e) => {
                if (e.target === infoModal) {
                    infoModal.classList.add('hidden');
                }
            });

            // Modal Logic (Terms & Conditions)
            termsButton.addEventListener('click', () => {
                termsModal.classList.remove('hidden');
            });

            closeTermsModalBtn.addEventListener('click', () => {
                termsModal.classList.add('hidden');
            });

            termsModal.addEventListener('click', (e) => {
                if (e.target === termsModal) {
                    termsModal.classList.add('hidden');
                }
            });

        });
    </script>

</body>
</html>
