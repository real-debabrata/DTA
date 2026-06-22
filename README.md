<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DTA - Deb Test Agency Documentation</title>
    <style>
        :root {
            --bg-color: #f8fafc;
            --container-bg: #ffffff;
            --text-main: #1e293b;
            --text-muted: #64748b;
            --primary: #2563eb;
            --primary-hover: #1d4ed8;
            --accent: #0f172a;
            --border: #e2e8f0;
            --code-bg: #f1f5f9;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            margin: 0;
            padding: 0;
        }

        .container {
            max-width: 900px;
            margin: 40px auto;
            padding: 40px;
            background: var(--container-bg);
            border-radius: 12px;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.05), 0 2px 4px -2px rgb(0 0 0 / 0.05);
            border: 1px solid var(--border);
        }

        header {
            border-bottom: 2px solid var(--border);
            padding-bottom: 24px;
            margin-bottom: 32px;
            text-align: center;
        }

        .logo-area h1 {
            font-size: 2.5rem;
            color: var(--accent);
            margin: 0 0 8px 0;
            font-weight: 800;
            letter-spacing: -0.05em;
        }

        .badge {
            display: inline-block;
            background: var(--code-bg);
            color: var(--primary);
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            border: 1px solid var(--border);
        }

        h2 {
            font-size: 1.75rem;
            color: var(--accent);
            margin-top: 40px;
            margin-bottom: 16px;
            border-bottom: 1px solid var(--border);
            padding-bottom: 8px;
        }

        h3 {
            font-size: 1.25rem;
            color: var(--accent);
            margin-top: 24px;
        }

        p {
            margin-top: 0;
            margin-bottom: 16px;
            color: var(--text-main);
        }

        blockquote {
            margin: 24px 0;
            padding: 16px 24px;
            background-color: #eff6ff;
            border-left: 4px solid var(--primary);
            color: #1e3a8a;
            border-radius: 0 8px 8px 0;
        }

        blockquote p {
            margin: 0;
            font-weight: 500;
        }

        ul {
            padding-left: 24px;
            margin-bottom: 24px;
        }

        li {
            margin-bottom: 8px;
        }

        .grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 16px;
            margin: 24px 0;
        }

        .card {
            border: 1px solid var(--border);
            padding: 20px;
            border-radius: 8px;
            background: var(--bg-color);
        }

        .card h4 {
            margin: 0 0 8px 0;
            color: var(--primary);
            font-size: 1.1rem;
        }

        .card p {
            margin: 0;
            font-size: 0.95rem;
            color: var(--text-muted);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 24px 0;
            font-size: 0.95rem;
        }

        th, td {
            text-align: left;
            padding: 12px 16px;
            border-bottom: 1px solid var(--border);
        }

        th {
            background-color: var(--bg-color);
            color: var(--accent);
            font-weight: 600;
        }

        tr:hover {
            background-color: #f8fafc;
        }

        code {
            font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
            background-color: var(--code-bg);
            padding: 2px 6px;
            border-radius: 4px;
            font-size: 0.9em;
            color: #0f172a;
        }

        pre {
            font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;
            background-color: var(--accent);
            color: #f8fafc;
            padding: 16px;
            border-radius: 8px;
            overflow-x: auto;
            font-size: 0.9rem;
            margin: 24px 0;
        }

        pre code {
            background: transparent;
            color: inherit;
            padding: 0;
        }

        .footer {
            margin-top: 50px;
            padding-top: 20px;
            border-top: 1px solid var(--border);
            text-align: center;
            font-size: 0.85rem;
            color: var(--text-muted);
        }

        @media (max-width: 768px) {
            .grid {
                grid-template-columns: 1fr;
            }
            .container {
                padding: 20px;
                margin: 10px;
            }
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <div class="logo-area">
            <h1>DTA</h1>
            <p style="color: var(--text-muted); font-size: 1.2rem; margin-bottom: 12px;">Deb Test Agency Assessment Portal</p>
            <span class="badge">v1.0.0</span>
            <span class="badge" style="margin-left: 5px;">Client-Side Engine</span>
        </div>
    </header>

    <section id="overview">
        <h2>Overview</h2>
        <p><strong>DTA (Deb Test Agency)</strong> is a lightweight, responsive, browser-based examination and quiz engine designed to run instantly without complex backend configurations. It acts as an interactive portal built primarily to deliver highly focused academic and professional assessments in <strong>Commerce, Accountancy, and Tally Prime core frameworks</strong>.</p>
        
        <blockquote>
            <p>Target Audience: Ideal for students preparing for competitive entrance examinations (like CUET UG) and individuals training for accounting or software-specific technical interviews.</p>
        </blockquote>
    </section>

    <section id="key-features">
        <h2>Key Features</h2>
        <div class="grid">
            <div class="card">
                <h4>Dynamic JSON Loading</h4>
                <p>Loads standard assessment modules directly via structured JSON datasets natively, enabling effortless exam curation.</p>
            </div>
            <div class="card">
                <h4>Zero Dependencies</h4>
                <p>Pure client-side rendering engine architecture. No external database, Node.js environment, or installation required.</p>
            </div>
            <div class="card">
                <h4>Optimized UI</h4>
                <p>Clean layout constructed to keep user focus directed strictly toward question retention, option tracking, and metrics evaluation.</p>
            </div>
            <div class="card">
                <h4>Instant Performance Check</h4>
                <p>Immediate performance responses upon evaluation to support structured, rapid study iterations.</p>
            </div>
        </div>
    </section>

    <section id="repository-structure">
        <h2>Repository Architecture</h2>
        <p>The system maintains an explicitly flat layout for optimal portability:</p>
        <pre><code>DTA-main/
├── index.html          # Core interface engine & interactive web application
├── LICENSE             # Project licensing configurations
├── README.md           # Repository text summary file
└── questions/          # Structured JSON data module repository
    ├── CUET UG ACCOUNTANCY PYQ 2025 (50Q).json
    ├── Demo Test.json
    ├── Tally Interview Questions MCQ Test(45Q).json
    ├── Tally Ledgers and Groups Quiz.json
    └── Tally Prime Core Functionalities TEST (60Q).json</code></pre>
    </section>

    <section id="question-banks">
        <h2>Available Assessment Modules</h2>
        <p>The following pre-configured evaluation matrices are populated directly inside the <code>questions/</code> directory:</p>
        
        <table>
            <thead>
                <tr>
                    <th>Module Dataset Title</th>
                    <th>Question Count</th>
                    <th>Focus Core Objective</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td><code>CUET UG ACCOUNTANCY PYQ 2025</code></td>
                    <td>50 Questions</td>
                    <td>Academic evaluation matrix tracking Previous Year Questions for undergraduate entry.</td>
                </tr>
                <tr>
                    <td><code>Tally Prime Core Functionalities TEST</code></td>
                    <td>60 Questions</td>
                    <td>Deep dive assessment evaluating advanced transactional execution pathways within Tally Prime.</td>
                </tr>
                <tr>
                    <td><code>Tally Interview Questions MCQ Test</code></td>
                    <td>45 Questions</td>
                    <td>Industry technical vetting mock exam emphasizing rapid accounting placement benchmarks.</td>
                </tr>
                <tr>
                    <td><code>Tally Ledgers and Groups Quiz</code></td>
                    <td>Dynamic</td>
                    <td>Focused compliance test emphasizing accurate group structuring and ledger assignments.</td>
                </tr>
                <tr>
                    <td><code>Demo Test</code></td>
                    <td>Varies</td>
                    <td>Diagnostic blueprint environment designed to verify structural integrity of JSON variations.</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section id="getting-started">
        <h2>Quick Start Guide</h2>
        
        <h3>Method 1: Local Launch (Direct)</h3>
        <p>Because the portal is entirely browser-native, you do not need a compilation sequence. Simply look into the folder and open it:</p>
        <ul>
            <li>Navigate to your local directory setup and double-click <code>index.html</code> to open it in any modern browser (Chrome, Edge, Firefox, Safari).</li>
        </ul>

        <h3>Method 2: Static HTTP Server (Recommended)</h3>
        <p>To avoid security sandboxing mechanisms (CORS constraints) when fetching JSON arrays locally via script extensions, launching through a local loopback server is optimal:</p>
        <pre><code># Navigate into the project folder
cd DTA-main

# Spin up a lightweight Python web server instance
python -m http.server 8000</code></pre>
        <p>Once active, target your address block pointer to: <code>http://localhost:8000</code></p>
    </section>

    <section id="customization">
        <h2>Expanding the Tests</h2>
        <p>To register new exam components to the system, formatting must comply with the internal structural parsing schema. Add target files using this strict structure:</p>
        <pre><code>[
  {
    "question": "What is the default group for Stock-in-Hand in Tally Prime?",
    "options": ["Current Assets", "Current Liabilities", "Fixed Assets", "Direct Expenses"],
    "answer": "Current Assets"
  }
]</code></pre>
    </section>

    <footer class="footer">
        <p>DTA (Deb Test Agency) — Open Source Utility. Distributed under project LICENSE parameters.</p>
    </footer>
</div>

</body>
</html>
