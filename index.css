<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Case Study: Tablet Formulation</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f7fa;
            color: #333;
            line-height: 1.6;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .presentation-container {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            margin-bottom: 30px;
        }
        
        .presentation-header {
            background: linear-gradient(135deg, #1a6baf 0%, #2a5298 100%);
            color: white;
            padding: 25px 30px;
            text-align: center;
        }
        
        .presentation-header h1 {
            font-size: 28px;
            margin-bottom: 10px;
            font-weight: 600;
        }
        
        .presentation-header .subtitle {
            font-size: 18px;
            opacity: 0.9;
            font-weight: 300;
        }
        
        .slide-container {
            position: relative;
            min-height: 500px;
        }
        
        .slide {
            padding: 30px;
            display: none;
            animation: fadeIn 0.5s ease;
        }
        
        .slide.active {
            display: block;
        }
        
        @keyframes fadeIn {
            from { opacity: 0.5; }
            to { opacity: 1; }
        }
        
        .slide-header {
            color: #2a5298;
            border-bottom: 2px solid #eaeaea;
            padding-bottom: 15px;
            margin-bottom: 25px;
            font-size: 24px;
            display: flex;
            align-items: center;
        }
        
        .slide-header i {
            margin-right: 15px;
            font-size: 28px;
        }
        
        .slide-content {
            font-size: 18px;
            margin-bottom: 20px;
        }
        
        .table-container {
            margin: 20px 0;
            overflow-x: auto;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 15px 0;
        }
        
        th {
            background-color: #2a5298;
            color: white;
            padding: 12px 15px;
            text-align: left;
        }
        
        td {
            padding: 12px 15px;
            border-bottom: 1px solid #eaeaea;
        }
        
        tr:nth-child(even) {
            background-color: #f8f9fa;
        }
        
        .diagram-container {
            display: flex;
            justify-content: center;
            margin: 25px 0;
        }
        
        .process-diagram {
            display: grid;
            grid-template-columns: repeat(6, 1fr);
            grid-gap: 15px;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .process-step {
            background-color: #eef5ff;
            border: 1px solid #c5d8ff;
            border-radius: 8px;
            padding: 15px;
            text-align: center;
            position: relative;
        }
        
        .process-step:not(:last-child)::after {
            content: "→";
            position: absolute;
            right: -20px;
            top: 50%;
            transform: translateY(-50%);
            color: #2a5298;
            font-weight: bold;
        }
        
        .step-number {
            background-color: #2a5298;
            color: white;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 10px;
            font-weight: bold;
        }
        
        .step-title {
            font-weight: 600;
            margin-bottom: 5px;
            color: #2a5298;
        }
        
        .challenge-box {
            background-color: #fff5f5;
            border-left: 4px solid #e74c3c;
            padding: 15px;
            margin: 15px 0;
        }
        
        .factor-box {
            background-color: #f0f9ff;
            border-left: 4px solid #3498db;
            padding: 15px;
            margin: 15px 0;
        }
        
        .navigation {
            display: flex;
            justify-content: space-between;
            padding: 20px 30px;
            border-top: 1px solid #eaeaea;
        }
        
        .nav-btn {
            background-color: #2a5298;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }
        
        .nav-btn:hover {
            background-color: #1a3a6d;
        }
        
        .nav-btn:disabled {
            background-color: #cccccc;
            cursor: not-allowed;
        }
        
        .slide-counter {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 5px;
        }
        
        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background-color: #ddd;
            display: inline-block;
            margin: 0 3px;
            cursor: pointer;
        }
        
        .dot.active {
            background-color: #2a5298;
        }
        
        .export-btn {
            background-color: #27ae60;
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            display: flex;
            align-items: center;
            gap: 8px;
            margin: 0 auto;
            transition: background-color 0.3s;
        }
        
        .export-btn:hover {
            background-color: #219653;
        }
        
        .footer {
            text-align: center;
            margin-top: 20px;
            color: #777;
            font-size: 14px;
        }
        
        @media print {
            body {
                padding: 0;
            }
            
            .navigation, .export-btn {
                display: none;
            }
            
            .slide {
                display: block !important;
                page-break-after: always;
                min-height: auto;
            }
            
            .presentation-container {
                box-shadow: none;
            }
        }
    </style>
</head>
<body>
    <div class="presentation-container">
        <div class="presentation-header">
            <h1>Case Study: Tablet Formulation</h1>
            <div class="subtitle">Formulation Process, Excipients, Stability Factors, and Challenges</div>
        </div>
        
        <div class="slide-container">
            <!-- Slide 1: Introduction -->
            <div class="slide active" id="slide1">
                <div class="slide-header">
                    <i class="fas fa-tablets"></i>
                    <h2>Tablet Formulation Overview</h2>
                </div>
                <div class="slide-content">
                    <p>Tablets are one of the most common oral solid dosage forms, accounting for approximately 60% of all pharmaceutical formulations. They offer advantages such as:</p>
                    <ul style="margin-left: 20px; margin-top: 10px;">
                        <li>Precise dosing and uniformity</li>
                        <li>Chemical and physical stability</li>
                        <li>Ease of administration and patient compliance</li>
                        <li>Cost-effective manufacturing</li>
                        <li>Flexibility in design (immediate release, sustained release, etc.)</li>
                    </ul>
                    <div class="diagram-container">
                        <div class="process-diagram">
                            <div class="process-step">
                                <div class="step-number">1</div>
                                <div class="step-title">API + Excipients</div>
                                <div class="step-desc">Active Pharmaceutical Ingredient with additives</div>
                            </div>
                            <div class="process-step">
                                <div class="step-number">2</div>
                                <div class="step-title">Mixing</div>
                                <div class="step-desc">Blending of components</div>
                            </div>
                            <div class="process-step">
                                <div class="step-number">3</div>
                                <div class="step-title">Granulation</div>
                                <div class="step-desc">Particle size enlargement</div>
                            </div>
                            <div class="process-step">
                                <div class="step-number">4</div>
                                <div class="step-title">Compression</div>
                                <div class="step-desc">Tablet formation</div>
                            </div>
                            <div class="process-step">
                                <div class="step-number">5</div>
                                <div class="step-title">Coating</div>
                                <div class="step-desc">Applying protective layer</div>
                            </div>
                            <div class="process-step">
                                <div class="step-number">6</div>
                                <div class="step-title">Packaging</div>
                                <div class="step-desc">Final product protection</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Slide 2: Formulation Process -->
            <div class="slide" id="slide2">
                <div class="slide-header">
                    <i class="fas fa-industry"></i>
                    <h2>Tablet Formulation Process</h2>
                </div>
                <div class="slide-content">
                    <p>The tablet manufacturing process involves several critical steps to ensure product quality, efficacy, and safety:</p>
                    
                    <div class="table-container">
                        <table>
                            <thead>
                                <tr>
                                    <th>Step</th>
                                    <th>Description</th>
                                    <th>Purpose</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>1. Material Dispensing</td>
                                    <td>Weighing API and excipients according to formula</td>
                                    <td>Ensure accurate composition</td>
                                </tr>
                                <tr>
                                    <td>2. Sizing & Milling</td>
                                    <td>Reducing particle size of materials</td>
                                    <td>Improve uniformity and dissolution</td>
                                </tr>
                                <tr>
                                    <td>3. Blending/Mixing</td>
                                    <td>Homogeneous mixing of all components</td>
                                    <td>Achieve content uniformity</td>
                                </tr>
                                <tr>
                                    <td>4. Granulation</td>
                                    <td>Wet or dry process to form granules</td>
                                    <td>Improve flow and compression properties</td>
                                </tr>
                                <tr>
                                    <td>5. Drying</td>
                                    <td>Removal of moisture (for wet granulation)</td>
                                    <td>Prevent stability issues</td>
                                </tr>
                                <tr>
                                    <td>6. Compression</td>
                                    <td>Forming tablets using punches and dies</td>
                                    <td>Create final tablet form</td>
                                </tr>
                                <tr>
                                    <td>7. Coating</td>
                                    <td>Applying polymer film (optional)</td>
                                    <td>Mask taste, protect, control release</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                    
                    <div class="factor-box">
                        <strong>Key Considerations:</strong> Flow properties, compressibility, particle size distribution, moisture content, and blend uniformity must be carefully controlled at each stage.
                    </div>
                </div>
            </div>
            
            <!-- Slide 3: Excipients -->
            <div class="slide" id="slide3">
                <div class="slide-header">
                    <i class="fas fa-flask"></i>
                    <h2>Excipients in Tablet Formulation</h2>
                </div>
                <div class="slide-content">
                    <p>Excipients are inactive ingredients that serve specific functions in tablet formulation:</p>
                    
                    <div class="table-container">
                        <table>
                            <thead>
                                <tr>
                                    <th>Excipient Type</th>
                                    <th>Function</th>
                                    <th>Common Examples</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>Diluents/Fillers</td>
                                    <td>Increase bulk for proper tablet size</td>
                                    <td>Lactose, microcrystalline cellulose, starch</td>
                                </tr>
                                <tr>
                                    <td>Binders</td>
                                    <td>Provide cohesive properties for granulation</td>
                                    <td>Povidone, hydroxypropyl methylcellulose, starch paste</td>
                                </tr>
                                <tr>
                                    <td>Disintegrants</td>
                                    <td>Promote tablet breakup in gastrointestinal fluid</td>
                                    <td>Croscarmellose sodium, sodium starch glycolate, crospovidone</td>
                                </tr>
                                <tr>
                                    <td>Lubricants</td>
                                    <td>Reduce friction during compression and ejection</td>
                                    <td>Magnesium stearate, stearic acid, sodium stearyl fumarate</td>
                                </tr>
                                <tr>
                                    <td>Glidants</td>
                                    <td>Improve powder flow properties</td>
                                    <td>Colloidal silicon dioxide, talc</td>
                                </tr>
                                <tr>
                                    <td>Colorants & Flavors</td>
                                    <td>Enhance appearance and palatability</td>
                                    <td>FD&C dyes, iron oxides, natural flavors</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                    
                    <p style="margin-top: 20px;"><strong>Formulation Example (Acetaminophen Tablet):</strong></p>
                    <ul style="margin-left: 20px;">
                        <li>Active Ingredient: Acetaminophen (500 mg)</li>
                        <li>Diluent: Microcrystalline cellulose (150 mg)</li>
                        <li>Binder: Povidone (20 mg)</li>
                        <li>Disintegrant: Sodium starch glycolate (25 mg)</li>
                        <li>Lubricant: Magnesium stearate (5 mg)</li>
                        <li>Total Tablet Weight: ~700 mg</li>
                    </ul>
                </div>
            </div>
            
            <!-- Slide 4: Stability Factors -->
            <div class="slide" id="slide4">
                <div class="slide-header">
                    <i class="fas fa-chart-line"></i>
                    <h2>Stability Factors in Tablet Formulation</h2>
                </div>
                <div class="slide-content">
                    <p>Tablet stability must be maintained throughout shelf life to ensure safety and efficacy:</p>
                    
                    <div class="factor-box">
                        <strong>1. Chemical Stability</strong>
                        <p>Prevention of API degradation through:</p>
                        <ul style="margin-left: 20px;">
                            <li>pH optimization in formulation</li>
                            <li>Use of antioxidants (e.g., ascorbic acid, BHT)</li>
                            <li>Protection from light (opaque packaging, colorants)</li>
                            <li>Moisture control (desiccants in packaging)</li>
                        </ul>
                    </div>
                    
                    <div class="factor-box">
                        <strong>2. Physical Stability</strong>
                        <p>Maintaining tablet integrity and performance:</p>
                        <ul style="margin-left: 20px;">
                            <li>Hardness and friability control</li>
                            <li>Prevention of capping and lamination</li>
                            <li>Dissolution profile consistency</li>
                            <li>Moisture barrier coatings</li>
                        </ul>
                    </div>
                    
                    <div class="table-container" style="margin-top: 20px;">
                        <table>
                            <thead>
                                <tr>
                                    <th>Stability Parameter</th>
                                    <th>Testing Method</th>
                                    <th>Acceptance Criteria</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>Chemical Purity</td>
                                    <td>HPLC/UV Spectroscopy</td>
                                    <td>Not less than 90% of labeled claim</td>
                                </tr>
                                <tr>
                                    <td>Dissolution</td>
                                    <td>USP Dissolution Apparatus</td>
                                    <td>Q ≥ 80% in 30 minutes</td>
                                </tr>
                                <tr>
                                    <td>Hardness</td>
                                    <td>Tablet Hardness Tester</td>
                                    <td>4-10 kg/cm² depending on formulation</td>
                                </tr>
                                <tr>
                                    <td>Friability</td>
                                    <td>Roche Friabilator</td>
                                    <td>Not more than 1% weight loss</td>
                                </tr>
                                <tr>
                                    <td>Moisture Content</td>
                                    <td>Karl Fischer Titration</td>
                                    <td>Not more than 5% w/w</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
            
            <!-- Slide 5: Challenges -->
            <div class="slide" id="slide5">
                <div class="slide-header">
                    <i class="fas fa-exclamation-triangle"></i>
                    <h2>Challenges in Tablet Formulation</h2>
                </div>
                <div class="slide-content">
                    <p>Tablet manufacturing faces several technical and regulatory challenges:</p>
                    
                    <div class="challenge-box">
                        <strong>1. Content Uniformity</strong>
                        <p>Ensuring each tablet contains the correct amount of API, especially for low-dose drugs (< 1 mg). This requires sophisticated mixing technology and validation.</p>
                    </div>
                    
                    <div class="challenge-box">
                        <strong>2. API Characteristics</strong>
                        <p>Poor solubility, low permeability, and instability of some APIs require specialized formulation approaches like solid dispersions or micronization.</p>
                    </div>
                    
                    <div class="challenge-box">
                        <strong>3. Scale-up Issues</strong>
                        <p>Process parameters that work at laboratory scale may not translate directly to commercial production, requiring extensive optimization.</p>
                    </div>
                    
                    <div class="challenge-box">
                        <strong>4. Regulatory Compliance</strong>
                        <p>Meeting strict guidelines from agencies like FDA, EMA for quality, stability, and bioequivalence. Current Good Manufacturing Practices (cGMP) must be followed.</p>
                    </div>
                    
                    <div class="challenge-box">
                        <strong>5. Stability Issues</strong>
                        <p>Chemical degradation (hydrolysis, oxidation), physical changes (polymorphic transitions), and excipient-API interactions must be minimized.</p>
                    </div>
                    
                    <div style="background-color: #f0fff0; border-left: 4px solid #27ae60; padding: 15px; margin-top: 20px;">
                        <strong>Mitigation Strategies:</strong>
                        <ul style="margin-left: 20px; margin-top: 5px;">
                            <li>Quality by Design (QbD) approach in formulation development</li>
                            <li>Robust process validation and control strategies</li>
                            <li>Accelerated stability studies to predict shelf life</li>
                            <li>Compatibility studies between API and excipients</li>
                        </ul>
                    </div>
                </div>
            </div>
            
            <!-- Slide 6: Summary -->
            <div class="slide" id="slide6">
                <div class="slide-header">
                    <i class="fas fa-clipboard-check"></i>
                    <h2>Summary & Key Takeaways</h2>
                </div>
                <div class="slide-content">
                    <p>Tablet formulation is a complex process requiring careful consideration of multiple factors:</p>
                    
                    <div style="display: flex; flex-wrap: wrap; gap: 20px; margin-top: 20px;">
                        <div style="flex: 1; min-width: 250px; background-color: #eef5ff; padding: 20px; border-radius: 8px;">
                            <h3 style="color: #2a5298; margin-bottom: 10px;">Formulation Process</h3>
                            <ul style="margin-left: 15px;">
                                <li>Multi-step process from material dispensing to packaging</li>
                                <li>Critical steps: granulation, compression, coating</li>
                                <li>Process parameters must be optimized for each formulation</li>
                            </ul>
                        </div>
                        
                        <div style="flex: 1; min-width: 250px; background-color: #f0f9ff; padding: 20px; border-radius: 8px;">
                            <h3 style="color: #2a5298; margin-bottom: 10px;">Excipients</h3>
                            <ul style="margin-left: 15px;">
                                <li>Serve specific functions in the formulation</li>
                                <li>Must be compatible with API and process</li>
                                <li>Selected based on functionality, not just cost</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div style="display: flex; flex-wrap: wrap; gap: 20px; margin-top: 20px;">
                        <div style="flex: 1; min-width: 250px; background-color: #f9f0ff; padding: 20px; border-radius: 8px;">
                            <h3 style="color: #2a5298; margin-bottom: 10px;">Stability</h3>
                            <ul style="margin-left: 15px;">
                                <li>Both chemical and physical stability must be ensured</li>
                                <li>Packaging plays a crucial role in stability maintenance</li>
                                <li>Accelerated stability testing predicts shelf life</li>
                            </ul>
                        </div>
                        
                        <div style="flex: 1; min-width: 250px; background-color: #fff0f5; padding: 20px; border-radius: 8px;">
                            <h3 style="color: #2a5298; margin-bottom: 10px;">Challenges</h3>
                            <ul style="margin-left: 15px;">
                                <li>Content uniformity, especially for low-dose drugs</li>
                                <li>API solubility and permeability limitations</li>
                                <li>Regulatory compliance and scale-up issues</li>
                            </ul>
                        </div>
                    </div>
                    
                    <div style="margin-top: 25px; padding: 20px; background-color: #f8f9fa; border-radius: 8px;">
                        <h3 style="color: #2a5298; margin-bottom: 10px;">Future Directions</h3>
                        <p>Emerging trends in tablet formulation include:</p>
                        <ul style="margin-left: 20px; margin-top: 5px;">
                            <li>3D printed tablets for personalized dosing</li>
                            <li>Orally disintegrating tablets for pediatric/geriatric use</li>
                            <li>Sustained-release formulations for better compliance</li>
                            <li>Continuous manufacturing processes</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="navigation">
            <button class="nav-btn" id="prevBtn" disabled>
                <i class="fas fa-arrow-left"></i> Previous
            </button>
            
            <div class="slide-counter">
                <span class="dot active" data-slide="1"></span>
                <span class="dot" data-slide="2"></span>
                <span class="dot" data-slide="3"></span>
                <span class="dot" data-slide="4"></span>
                <span class="dot" data-slide="5"></span>
                <span class="dot" data-slide="6"></span>
            </div>
            
            <button class="nav-btn" id="nextBtn">
                Next <i class="fas fa-arrow-right"></i>
            </button>
        </div>
    </div>
    
    <button class="export-btn" id="exportBtn">
        <i class="fas fa-file-pdf"></i> Save as PDF/Print
    </button>
    
    <div class="footer">
        <p>Case Study: Tablet Formulation | For Educational Purposes | Created for Pharmaceutical Sciences</p>
        <p>Data sources: USP, FDA Guidelines, Pharmaceutical Formulation textbooks</p>
    </div>

    <script>
        // Slide navigation functionality
        const slides = document.querySelectorAll('.slide');
        const dots = document.querySelectorAll('.dot');
        const prevBtn = document.getElementById('prevBtn');
        const nextBtn = document.getElementById('nextBtn');
        const exportBtn = document.getElementById('exportBtn');
        let currentSlide = 1;
        const totalSlides = slides.length;
        
        // Initialize slides
        showSlide(currentSlide);
        
        // Next button click
        nextBtn.addEventListener('click', () => {
            if (currentSlide < totalSlides) {
                currentSlide++;
                showSlide(currentSlide);
            }
        });
        
        // Previous button click
        prevBtn.addEventListener('click', () => {
            if (currentSlide > 1) {
                currentSlide--;
                showSlide(currentSlide);
            }
        });
        
        // Dot click
        dots.forEach(dot => {
            dot.addEventListener('click', () => {
                const slideNumber = parseInt(dot.getAttribute('data-slide'));
                currentSlide = slideNumber;
                showSlide(currentSlide);
            });
        });
        
        // Export/Print button
        exportBtn.addEventListener('click', () => {
            window.print();
        });
        
        // Show specific slide
        function showSlide(slideNumber) {
            // Hide all slides
            slides.forEach(slide => {
                slide.classList.remove('active');
            });
            
            // Remove active class from all dots
            dots.forEach(dot => {
                dot.classList.remove('active');
            });
            
            // Show current slide
            document.getElementById(`slide${slideNumber}`).classList.add('active');
            
            // Activate current dot
            dots[slideNumber - 1].classList.add('active');
            
            // Update button states
            prevBtn.disabled = slideNumber === 1;
            nextBtn.disabled = slideNumber === totalSlides;
            
            // Update button text on last slide
            if (slideNumber === totalSlides) {
                nextBtn.innerHTML = 'Finish <i class="fas fa-check"></i>';
            } else {
                nextBtn.innerHTML = 'Next <i class="fas fa-arrow-right"></i>';
            }
        }
        
        // Keyboard navigation
        document.addEventListener('keydown', (e) => {
            if (e.key === 'ArrowRight' || e.key === ' ') {
                if (currentSlide < totalSlides) {
                    currentSlide++;
                    showSlide(currentSlide);
                }
            } else if (e.key === 'ArrowLeft') {
                if (currentSlide > 1) {
                    currentSlide--;
                    showSlide(currentSlide);
                }
            }
        });
    </script>
</body>
</html>