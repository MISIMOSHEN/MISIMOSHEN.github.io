<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Misimoshen | Movement Ecology Researcher</title>
    <style>
        :root {
            --primary: #2D5D4B;  /* Forest Green */
            --secondary: #6B8F71; /* Moss Green */
            --accent: #A4C3B2;    /* Mist Green */
            --text: #36453B;      /* Charcoal Green */
            --background: #F8F9FA;
        }

        body {
            font-family: 'Segoe UI', system-ui;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
            background: var(--background);
            color: var(--text);
        }

        .section {
            max-width: 800px;
            margin: 40px auto;
            padding: 25px;
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .experience-card {
            border-left: 4px solid var(--primary);
            padding-left: 20px;
            margin: 25px 0;
            transition: transform 0.3s;
        }

        .experience-card:hover {
            transform: translateX(10px);
        }

        .skill-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .skill-card {
            background: var(--accent);
            padding: 12px;
            border-radius: 8px;
            text-align: center;
            font-size: 0.9em;
        }

        h2 {
            color: var(--primary);
            border-bottom: 2px solid var(--secondary);
            padding-bottom: 5px;
        }

        .timeline {
            color: #666;
            font-size: 0.9em;
            font-style: italic;
        }
    </style>
</head>
<body>
    <div class="section">
        <h1>🐾 Misimoshen</h1>
        <p>👋 Movement Ecologist | Wildlife Conservation Technologist</p>
    </div>

    <div class="section">
        <h2>🔬 Research Experience</h2>
        
        <div class="experience-card">
            <h3>Field Research Assistant · Longkou Forest Farm</h3>
            <div class="timeline">Nov 2022 - Harbin, China</div>
            <ul>
                <li>Implemented Hidden Markov Models for wild boar movement pattern validation</li>
                <li>Developed behavioral recognition algorithms improving study accuracy by 15%</li>
            </ul>
        </div>

        <div class="experience-card">
            <h3>Wildlife Rescue Volunteer · Hunchun City</h3>
            <ul>
                <li>Executed full-cycle wildlife collar deployment (GPS hybrid systems)</li>
                <li>Collected 200+ hours of movement data for ungulate behavior analysis</li>
                <li>Performed post-release monitoring using Argos satellite system</li>
            </ul>
        </div>

        <div class="experience-card">
            <h3>Taipinggou Nature Reserve · 2023</h3>
            <ul>
                <li>Conducted UAV-based sika deer population surveys</li>
                <li>Designed 10km transect sampling protocols</li>
                <li>Developed species distribution models (AUC = 0.92)</li>
            </ul>
        </div>
    </div>

    <div class="section">
        <h2>🛠️ Technical Competencies</h2>
        <div class="skill-grid">
            <div class="skill-card">Home Range Analysis</div>
            <div class="skill-card">Movement Trajectory Visualization</div>
            <div class="skill-card">Utilization Distribution Modeling</div>
            <div class="skill-card">Movement Data Cleaning</div>
            <div class="skill-card">Behavioral Pattern Recognition</div>
            <div class="skill-card">Range Overlap Analysis</div>
        </div>
    </div>

    <div class="section">
        <h2>📬 Collaboration Opportunities</h2>
        <p>Seeking partnerships in:</p>
        <ul>
            <li>Wildlife tracking technology optimization</li>
            <li>Protected area management analytics</li>
            <li>Animal behavior modeling</li>
        </ul>
        <p>📧 Contact: [your.email@domain]</p>
        <div style="margin-top:15px">
            <img src="https://img.shields.io/badge/ORCID-0000-0000-0000-0000-a6ce39?style=flat&logo=orcid" alt="ORCID">
            <img src="https://img.shields.io/badge/ResearchGate-00CCBB?style=flat&logo=researchgate&logoColor=white" alt="ResearchGate">
        </div>
    </div>
</body>
</html>
