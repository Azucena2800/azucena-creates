# azucena-creates
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web Development Portfolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            text-align: center;
            padding: 60px 0;
            color: white;
            margin-bottom: 40px;
        }
        
        h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            animation: fadeInUp 1s ease-out;
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            animation: fadeInUp 1s ease-out 0.2s both;
        }
        
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }
        
        .project-card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            animation: fadeInUp 0.8s ease-out;
            backdrop-filter: blur(10px);
        }
        
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 30px 60px rgba(0,0,0,0.2);
        }
        
        .project-header {
            background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
            padding: 25px;
            color: white;
        }
        
        .project-card:nth-child(2n) .project-header {
            background: linear-gradient(135deg, #fa709a 0%, #fee140 100%);
        }
        
        .project-card:nth-child(3n) .project-header {
            background: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%);
            color: #333;
        }
        
        .project-card:nth-child(4n) .project-header {
            background: linear-gradient(135deg, #ff9a9e 0%, #fecfef 100%);
            color: #333;
        }
        
        .project-card:nth-child(5n) .project-header {
            background: linear-gradient(135deg, #96fbc4 0%, #f9f047 100%);
            color: #333;
        }
        
        .project-title {
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 8px;
        }
        
        .project-type {
            font-size: 0.9rem;
            opacity: 0.8;
        }
        
        .project-content {
            padding: 25px;
        }
        
        .project-description {
            margin-bottom: 20px;
            color: #666;
            line-height: 1.5;
        }
        
        .project-features {
            margin-bottom: 20px;
        }
        
        .feature-tag {
            display: inline-block;
            background: #f0f8ff;
            color: #4682b4;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            margin: 2px;
            border: 1px solid #e6f3ff;
        }
        
        .project-link {
            display: inline-flex;
            align-items: center;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            text-decoration: none;
            padding: 12px 24px;
            border-radius: 25px;
            transition: all 0.3s ease;
            font-weight: 500;
        }
        
        .project-link:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(102, 126, 234, 0.3);
        }
        
        .special-note {
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            border-radius: 15px;
            margin-top: 20px;
            border-left: 4px solid #4facfe;
        }
        
        .comparison-link {
            color: #667eea;
            text-decoration: none;
            font-weight: 500;
        }
        
        .comparison-link:hover {
            text-decoration: underline;
        }
        
        footer {
            text-align: center;
            color: white;
            padding: 40px 0;
            opacity: 0.8;
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @media (max-width: 768px) {
            .portfolio-grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .container {
                padding: 15px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Web Development Portfolio</h1>
            <p class="subtitle">Professional websites and pages built for NHMA (National Hispanic Medical Association)</p>
        </header>
        
        <div class="portfolio-grid">
            <div class="project-card">
                <div class="project-header">
                    <h3 class="project-title">Events Page</h3>
                    <p class="project-type">Event Management & Information Hub</p>
                </div>
                <div class="project-content">
                    <p class="project-description">
                        Comprehensive events showcase featuring upcoming NHMA activities, conferences, and professional development opportunities for medical professionals.
                    </p>
                    <div class="project-features">
                        <span class="feature-tag">Event Listings</span>
                        <span class="feature-tag">Date Management</span>
                        <span class="feature-tag">Information Architecture</span>
                    </div>
                    <a href="https://www.nhmamd.org/events" class="project-link" target="_blank">View Live Site →</a>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-header">
                    <h3 class="project-title">Respiratory Illness Resource</h3>
                    <p class="project-type">Medical Information Portal</p>
                </div>
                <div class="project-content">
                    <p class="project-description">
                        Educational resource page providing crucial information about respiratory illnesses, designed for healthcare professionals and the community.
                    </p>
                    <div class="project-features">
                        <span class="feature-tag">Medical Content</span>
                        <span class="feature-tag">Resource Hub</span>
                        <span class="feature-tag">Professional Layout</span>
                    </div>
                    <a href="https://nhma.memberclicks.net/respiratory-illness" class="project-link" target="_blank">View Live Site →</a>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-header">
                    <h3 class="project-title">Government Affairs</h3>
                    <p class="project-type">Policy & Advocacy Platform</p>
                </div>
                <div class="project-content">
                    <p class="project-description">
                        Strategic government affairs section highlighting NHMA's advocacy efforts, policy positions, and legislative initiatives affecting Hispanic healthcare.
                    </p>
                    <div class="project-features">
                        <span class="feature-tag">Policy Content</span>
                        <span class="feature-tag">Advocacy Focus</span>
                        <span class="feature-tag">Government Relations</span>
                    </div>
                    <a href="https://www.nhmamd.org/gov-affairs" class="project-link" target="_blank">View Live Site →</a>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-header">
                    <h3 class="project-title">NHMA Policy Hub</h3>
                    <p class="project-type">Policy Resource Center</p>
                </div>
                <div class="project-content">
                    <p class="project-description">
                        Centralized policy hub providing access to NHMA's official positions, research, and policy documents for members and stakeholders.
                    </p>
                    <div class="project-features">
                        <span class="feature-tag">Policy Repository</span>
                        <span class="feature-tag">Document Management</span>
                        <span class="feature-tag">Member Resources</span>
                    </div>
                    <a href="https://nhma.memberclicks.net/nhma-policy-hub" class="project-link" target="_blank">View Live Site →</a>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-header">
                    <h3 class="project-title">Stories That Matter</h3>
                    <p class="project-type">Content & Storytelling Platform</p>
                </div>
                <div class="project-content">
                    <p class="project-description">
                        Engaging storytelling platform showcasing impactful narratives from the Hispanic medical community, highlighting achievements and experiences.
                    </p>
                    <div class="project-features">
                        <span class="feature-tag">Content Curation</span>
                        <span class="feature-tag">Community Stories</span>
                        <span class="feature-tag">Narrative Design</span>
                    </div>
                    <a href="https://nhma.memberclicks.net/stories-that-matter" class="project-link" target="_blank">View Live Site →</a>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-header">
                    <h3 class="project-title">Membership Page 2025</h3>
                    <p class="project-type">Membership Management System</p>
                </div>
                <div class="project-content">
                    <p class="project-description">
                        Redesigned membership page for 2025, streamlining the joining process and improving user experience for new and existing members.
                    </p>
                    <div class="project-features">
                        <span class="feature-tag">UX Design</span>
                        <span class="feature-tag">Conversion Optimization</span>
                        <span class="feature-tag">2025 Redesign</span>
                    </div>
                    <a href="https://nhma.memberclicks.net/membership-page----draft-2025" class="project-link" target="_blank">View Live Site →</a>
                    <div class="special-note">
                        <strong>Before & After:</strong> Compare with the 
                        <a href="https://nhma.memberclicks.net/nhma-membership" class="comparison-link" target="_blank">original membership page</a> 
                        to see the improvements made.
                    </div>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-header">
                    <h3 class="project-title">FAQs Page</h3>
                    <p class="project-type">Information & Support Hub</p>
                </div>
                <div class="project-content">
                    <p class="project-description">
                        Comprehensive FAQ section addressing common member questions, providing clear and accessible information about NHMA services and policies.
                    </p>
                    <div class="project-features">
                        <span class="feature-tag">Information Architecture</span>
                        <span class="feature-tag">User Support</span>
                        <span class="feature-tag">Accessibility</span>
                    </div>
                    <a href="https://nhma.memberclicks.net/faqs" class="project-link" target="_blank">View Live Site →</a>
                </div>
            </div>
        </div>
        
        <footer>
            <p>Professional web development showcasing modern design, user experience, and functionality for healthcare organizations.</p>
        </footer>
    </div>
</body>
</html>
