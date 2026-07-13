<div align="center">
  <svg 
    width="100%" 
    height="450" 
    viewBox="0 0 1200 450" 
    xmlns="http://www.w3.org/2000/svg"
  >
    <defs>
      <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#0D1117" />
        <stop offset="25%" stop-color="#11161D" />
        <stop offset="50%" stop-color="#141923" />
        <stop offset="75%" stop-color="#11161D" />
        <stop offset="100%" stop-color="#0D1117" />
      </linearGradient>
      
      <linearGradient id="neonBlue" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#00F5FF" />
        <stop offset="50%" stop-color="#3A86FF" />
        <stop offset="100%" stop-color="#7B61FF" />
      </linearGradient>
      
      <linearGradient id="neonPink" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#FF00FF" />
        <stop offset="50%" stop-color="#FF007F" />
        <stop offset="100%" stop-color="#7B61FF" />
      </linearGradient>
      
      <linearGradient id="neonGreen" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#00FF9D" />
        <stop offset="100%" stop-color="#00F5FF" />
      </linearGradient>

      <filter id="glowBlue" x="-30%" y="-30%" width="160%" height="160%">
        <feGaussianBlur stdDeviation="10" result="blur" />
        <feComposite in="SourceGraphic" in2="blur" operator="over" />
      </filter>
      
      <filter id="glowPink" x="-30%" y="-30%" width="160%" height="160%">
        <feGaussianBlur stdDeviation="10" result="blur" />
        <feComposite in="SourceGraphic" in2="blur" operator="over" />
      </filter>

      <filter id="glowGreen" x="-30%" y="-30%" width="160%" height="160%">
        <feGaussianBlur stdDeviation="8" result="blur" />
        <feComposite in="SourceGraphic" in2="blur" operator="over" />
      </filter>

      <pattern id="grid" width="60" height="60" patternUnits="userSpaceOnUse">
        <path d="M 60 0 L 0 0 0 60" fill="none" stroke="#7B61FF" stroke-width="0.5" stroke-opacity="0.15" />
        <path d="M 30 0 L 30 60 M 0 30 L 60 30" fill="none" stroke="#00F5FF" stroke-width="0.2" stroke-opacity="0.1" />
      </pattern>

      <style>
        .title { 
          font-family: 'Courier New', monospace; 
          font-weight: 900; 
          font-size: 64px; 
          fill: #ffffff; 
          letter-spacing: 6px;
        }
        .subtitle { 
          font-family: 'Courier New', monospace; 
          font-weight: 700; 
          font-size: 28px; 
          fill: #00F5FF; 
          letter-spacing: 3px;
        }
        .code { 
          font-family: 'Courier New', monospace; 
          font-size: 18px; 
          fill: #FF00FF; 
          letter-spacing: 2px;
          font-weight: bold;
        }
        .tagline {
          font-family: 'Courier New', monospace; 
          font-size: 16px; 
          fill: #00FF9D; 
          opacity: 0.9;
          letter-spacing: 1px;
        }
        @keyframes pulse { 
          0% { opacity: 0.5; transform: scale(1); } 
          50% { opacity: 1; transform: scale(1.03); } 
          100% { opacity: 0.5; transform: scale(1); } 
        }
        @keyframes float { 
          0% { transform: translateY(0px); } 
          50% { transform: translateY(-15px); } 
          100% { transform: translateY(0px); } 
        }
        @keyframes dash { 
          to { stroke-dashoffset: -200; } 
        }
        @keyframes scanline { 
          0% { transform: translateY(-450px); } 
          100% { transform: translateY(450px); } 
        }
        .animated-pulse { animation: pulse 4s infinite; }
        .animated-float { animation: float 6s ease-in-out infinite; }
        .animated-path { animation: dash 12s linear infinite; }
        .animated-path-reverse { animation: dash 12s linear infinite reverse; }
      </style>
    </defs>
    
    <rect width="100%" height="100%" fill="url(#bgGrad)" />
    <rect width="100%" height="100%" fill="url(#grid)" />
    
    <rect width="100%" height="15" fill="#00F5FF" opacity="0.04">
      <animate attributeName="y" values="-15;450" dur="5s" repeatCount="indefinite" />
    </rect>
    <rect width="100%" height="8" fill="#FF00FF" opacity="0.03">
      <animate attributeName="y" values="-8;450" dur="3.5s" repeatCount="indefinite" />
    </rect>

    <g opacity="0.6">
      <circle cx="80" cy="80" r="2" fill="#ffffff" />
      <circle cx="150" cy="220" r="1.5" fill="#ffffff" />
      <circle cx="1050" cy="120" r="2.5" fill="#ffffff" />
      <circle cx="1120" cy="380" r="1.5" fill="#ffffff" />
      <circle cx="250" cy="400" r="2" fill="#ffffff" />
      <circle cx="850" cy="300" r="1.5" fill="#ffffff" />
      <circle cx="450" cy="100" r="1" fill="#ffffff" />
      <circle cx="750" cy="150" r="2" fill="#ffffff" />
      <circle cx="950" cy="80" r="1.5" fill="#ffffff" />
      <circle cx="350" cy="320" r="2" fill="#ffffff" />
    </g>

    <g class="animated-float" filter="url(#glowBlue)">
      <circle cx="180" cy="120" r="6" fill="#00F5FF" />
      <circle cx="280" cy="240" r="8" fill="#00F5FF" />
      <circle cx="120" cy="340" r="7" fill="#00F5FF" />
      <circle cx="240" cy="320" r="5" fill="#00F5FF" />
      <circle cx="100" cy="200" r="4" fill="#00F5FF" />
      <circle cx="320" cy="160" r="5" fill="#00F5FF" />
      
      <path class="animated-path" d="M 180 120 L 280 240 L 240 320 L 120 340 L 100 200 Z" fill="none" stroke="url(#neonBlue)" stroke-width="2.5" stroke-dasharray="10 5" />
      <path class="animated-path" d="M 180 120 L 100 200 L 280 240" fill="none" stroke="url(#neonBlue)" stroke-width="1.5" stroke-dasharray="5 5" opacity="0.6" />
      <path class="animated-path" d="M 320 160 L 280 240 L 120 340" fill="none" stroke="url(#neonBlue)" stroke-width="1" stroke-dasharray="3 6" opacity="0.4" />
    </g>
    
    <g class="animated-pulse" filter="url(#glowPink)">
      <circle cx="1020" cy="110" r="7" fill="#FF00FF" />
      <circle cx="920" cy="260" r="6" fill="#FF00FF" />
      <circle cx="1080" cy="350" r="8" fill="#FF00FF" />
      <circle cx="960" cy="370" r="5" fill="#FF00FF" />
      <circle cx="1100" cy="220" r="6" fill="#FF00FF" />
      <circle cx="880" cy="180" r="5" fill="#FF00FF" />
      
      <path class="animated-path-reverse" d="M 1020 110 L 920 260 L 960 370 L 1080 350 L 1100 220 Z" fill="none" stroke="url(#neonPink)" stroke-width="2.5" stroke-dasharray="10 5" />
      <path class="animated-path-reverse" d="M 1020 110 L 1100 220 L 920 260" fill="none" stroke="url(#neonPink)" stroke-width="1.5" stroke-dasharray="5 5" opacity="0.6" />
      <path class="animated-path-reverse" d="M 880 180 L 920 260 L 1080 350" fill="none" stroke="url(#neonPink)" stroke-width="1" stroke-dasharray="3 6" opacity="0.4" />
    </g>

    <g filter="url(#glowGreen)">
      <rect x="60" y="60" width="50" height="5" fill="#00FF9D" />
      <rect x="60" y="75" width="30" height="5" fill="#00FF9D" />
      <rect x="60" y="90" width="15" height="5" fill="#00FF9D" />
    </g>
    
    <g filter="url(#glowPink)">
      <rect x="1090" y="60" width="50" height="5" fill="#FF00FF" />
      <rect x="1110" y="75" width="30" height="5" fill="#FF00FF" />
      <rect x="1125" y="90" width="15" height="5" fill="#FF00FF" />
    </g>

    <path d="M 0 420 L 350 420 L 380 405 L 820 405 L 850 420 L 1200 420" fill="none" stroke="#7B61FF" stroke-width="4" stroke-opacity="0.7" filter="url(#glowBlue)" />
    <path d="M 0 430 L 1200 430" fill="none" stroke="#00F5FF" stroke-width="1.5" stroke-opacity="0.9" />
    <path d="M 0 440 L 1200 440" fill="none" stroke="#FF00FF" stroke-width="0.5" stroke-opacity="0.5" />
    
    <g class="animated-pulse" transform="translate(600, 220)">
      <polygon points="0,-150 130,-75 130,75 0,150 -130,75 -130,-75" fill="none" stroke="#7B61FF" stroke-width="1.5" opacity="0.4" />
      <polygon points="0,-170 147,-85 147,85 0,170 -147,85 -147,-85" fill="none" stroke="#00F5FF" stroke-width="0.75" opacity="0.25" />
      <polygon points="0,-130 112,-65 112,65 0,130 -112,65 -112,-65" fill="none" stroke="#FF00FF" stroke-width="0.5" opacity="0.2" />
    </g>

    <g class="animated-float">
      <text x="600" y="190" text-anchor="middle" class="title" filter="url(#glowBlue)">RAKESH CHOURASIA</text>
      <text x="600" y="245" text-anchor="middle" class="subtitle">FULL STACK MERN DEVELOPER</text>
      <text x="600" y="295" text-anchor="middle" class="code">&lt; METCONNECT INFOTECH PVT LTD /&gt;</text>
      <text x="600" y="340" text-anchor="middle" class="tagline">System Design • AI Integration • Backend Architecture</text>
    </g>
  </svg>
</div>

<br>
<br>

<div align="center">
  <a href="https://rakeshchourasia-portfolio.vercel.app/">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=3500&pause=1000&color=00F5FF&center=true&vCenter=true&width=1200&height=60&lines=Architecting+Scalable+Backend+Systems;Crafting+Next-Gen+MERN+Stack+Applications;Integrating+AI+%26+Real-Time+Web+Sockets;Designing+Premium+Glassmorphism+Interfaces;Executing+Complex+System+Designs" alt="Typing SVG" />
  </a>
</div>

<br>
<br>

<div align="center">
  <a href="https://github.com/Rakeshchourasia">
    <img src="https://img.shields.io/badge/GitHub-0D1117?style=for-the-badge&logo=github&logoColor=00F5FF&borderColor=7B61FF" alt="GitHub" />
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://linkedin.com/in/rakesh-chourasia-3a4b3825b">
    <img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=00F5FF&borderColor=7B61FF" alt="LinkedIn" />
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://rakeshchourasia-portfolio.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-0D1117?style=for-the-badge&logo=vercel&logoColor=00F5FF&borderColor=7B61FF" alt="Portfolio" />
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="mailto:rakesh@example.com">
    <img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logo=gmail&logoColor=00F5FF&borderColor=7B61FF" alt="Email" />
  </a>
</div>

<br>
<br>

<div align="center">
  <a href="https://github.com/Rakeshchourasia">
    <img src="https://komarev.com/ghpvc/?username=Rakeshchourasia&label=PROFILE+VIEWS&color=00F5FF&style=for-the-badge" alt="Profile Views" />
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://github.com/Rakeshchourasia?tab=followers">
    <img src="https://img.shields.io/github/followers/Rakeshchourasia?label=FOLLOWERS&style=for-the-badge&color=7B61FF&logo=github" alt="Followers" />
  </a>
  &nbsp;&nbsp;&nbsp;
  <a href="https://github.com/Rakeshchourasia?tab=stars">
    <img src="https://img.shields.io/github/stars/Rakeshchourasia?label=STARS&style=for-the-badge&color=FF00FF&logo=github" alt="Stars" />
  </a>
</div>

<br>
<br>

<div align="center">
  <svg width="1000" height="30" xmlns="http://www.w3.org/2000/svg">
    <line x1="0" y1="15" x2="1000" y2="15" stroke="#7B61FF" stroke-width="2" stroke-dasharray="15 10" />
    <circle cx="500" cy="15" r="8" fill="#00F5FF" />
    <circle cx="475" cy="15" r="5" fill="#FF00FF" />
    <circle cx="525" cy="15" r="5" fill="#FF00FF" />
  </svg>
</div>

<br>
<br>

```text
 ╭───────────────────────────────────────────────────────────────────────────────╮
 │  user@rakesh:~$ ./initialize_developer_profile.sh                             │
 │                                                                               │
 │  [INFO] Booting neural network...                                             │
 │  [INFO] Bypassing security protocols... [OK]                                  │
 │  [INFO] Loading core dependencies... ██████████████████████████████ 100%      │
 │                                                                               │
 │  [>] IDENTIFICATION MATRIX:                                                   │
 │      NAME       : Rakesh Chourasia                                            │
 │      ROLE       : Full Stack MERN Developer                                   │
 │      COMPANY    : Metconnect Infotech Pvt Ltd                                 │
 │      EDUCATION  : B.Tech Computer Science Engineering                         │
 │      LOCATION   : Hyderabad, India                                            │
 │                                                                               │
 │  [>] CORE TECHNICAL STACK:                                                    │
 │      BACKEND    : Node.js, Express.js, PostgreSQL, MongoDB, Redis, BullMQ     │
 │      FRONTEND   : React, Next.js, Tailwind, Framer Motion, Glassmorphism      │
 │      REALTIME   : Socket.IO, WebRTC, Firebase Firestore                       │
 │      INFRA      : Docker, REST APIs, JSON Web Tokens (JWT)                    │
 │                                                                               │
 │  [>] ACTIVE DIRECTIVES:                                                       │
 │      LEARNING   : Microservices Architecture, Advanced Docker Deployments     │
 │      MISSION    : Architecting high-performance, AI-integrated ecosystems     │
 │                                                                               │
 │  [>] SYSTEM STATUS: ONLINE. AWAITING INPUT.                                   │
 │                                                                               │
 │  user@rakesh:~$ _ █                                                           │
 ╰───────────────────────────────────────────────────────────────────────────────╯
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
    <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
    <br><br>
    <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
    <img src="https://img.shields.io/badge/Framer_Motion-0055FF?style=for-the-badge&logo=framer&logoColor=white" />
  </td>
  
  <td 
    align="center" 
    width="500" 
    bgcolor="#0D1117" 
    style="border: 2px solid #00F5FF; border-radius: 20px; padding: 35px; transition: transform 0.3s;"
  >
    <h3 style="color: #00F5FF; font-family: 'Courier New', monospace; font-size: 26px; margin-bottom: 25px;">Backend</h3>
    
    <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
    <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" />
    <br><br>
    <img src="https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socketdotio&logoColor=white" />
    <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white" />
  </td>
</tr>

<tr>
  <td 
    align="center" 
    width="500" 
    bgcolor="#0D1117" 
    style="border: 2px solid #7B61FF; border-radius: 20px; padding: 35px; transition: transform 0.3s;"
  >
    <h3 style="color: #7B61FF; font-family: 'Courier New', monospace; font-size: 26px; margin-bottom: 25px;">Database</h3>
    
    <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" />
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
    <br><br>
    <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
    <img src="https://img.shields.io/badge/BullMQ-FF4081?style=for-the-badge&logo=bullmq&logoColor=white" />
  </td>
  
  <td 
    align="center" 
    width="500" 
    bgcolor="#0D1117" 
    style="border: 2px solid #00FF9D; border-radius: 20px; padding: 35px; transition: transform 0.3s;"
  >
    <h3 style="color: #00FF9D; font-family: 'Courier New', monospace; font-size: 26px; margin-bottom: 25px;">DevOps</h3>
    
    <img src="https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white" />
    <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
    <br><br>
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
    <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" />
  </td>
</tr>

<tr>
  <td 
    align="center" 
    colspan="2" 
    bgcolor="#0D1117" 
    style="border: 2px solid #FF00FF; border-radius: 20px; padding: 40px; transition: transform 0.3s;"
  >
    <h3 style="color: #FF00FF; font-family: 'Courier New', monospace; font-size: 26px; margin-bottom: 25px;">Testing, AI & Architecture</h3>
    
    <img src="https://img.shields.io/badge/System_Design-0D1117?style=for-the-badge&borderColor=00F5FF&logo=architecture&logoColor=00F5FF" />
    <img src="https://img.shields.io/badge/AI_Integration-0D1117?style=for-the-badge&borderColor=FF00FF&logo=openai&logoColor=FF00FF" />
    <img src="https://img.shields.io/badge/Prompt_Engineering-0D1117?style=for-the-badge&borderColor=7B61FF&logo=robot&logoColor=7B61FF" />
    <img src="https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white" />
  </td>
</tr>
Plaintext
 ╭────────────────────────────────────────────╮  ╭────────────────────────────────────────────╮
 │ 🤖 Prompt Optimizer                        │  │ 🏢 HR Management System                    │
 │ AI Prompt Management Platform              │  │ Enterprise Resource Planning               │
 │                                            │  │                                            │
 │ ⚡ Rich Markdown Rendering                 │  │ ⚡ Employee Analytics Dashboards           │
 │ ⚡ Deep AI Integration                     │  │ ⚡ Automated Payroll Management            │
 │ ⚡ Complete Version Control                │  │ ⚡ Real-Time Attendance Tracking           │
 │ ⚡ Advanced Search & Filtering             │  │ ⚡ Strict Role-Based Access Control        │
 │ ⚡ Shareable Prompt Collections            │  │ ⚡ Exportable Analytics Reports            │
 │                                            │  │                                            │
 │ [React] [Node.js] [MongoDB] [OpenAI API]   │  │ [Next.js] [PostgreSQL] [Express] [Redis]   │
 │                                            │  │                                            │
 │ 🔗 Live Demo  |  💻 GitHub                 │  │ 🔗 Live Demo  |  💻 GitHub                 │
 ╰────────────────────────────────────────────╯  ╰────────────────────────────────────────────╯

 ╭────────────────────────────────────────────╮  ╭────────────────────────────────────────────╮
 │ 🎓 Brilliant Bihar                         │  │ 🏘️ Property Listing Portal               │
 │ Comprehensive LMS Platform                 │  │ Real Estate Discovery Platform             │
 │                                            │  │                                            │
 │ ⚡ Live Concurrent Video Streaming         │  │ ⚡ Advanced Geospatial Radius Search       │
 │ ⚡ Automated Secure Admit Cards            │  │ ⚡ Interactive Mapbox Integration          │
 │ ⚡ Robust Timed Test Series Modules        │  │ ⚡ Immersive Virtual 3D Tours              │
 │ ⚡ Dynamic Gamified Student Leaderboards   │  │ ⚡ Highly Secure Agent Control Portals     │
 │ ⚡ Bulletproof Device Fingerprinting       │  │ ⚡ Encrypted Stripe Secure Payments        │
 │                                            │  │                                            │
 │ [MERN] [Socket.IO] [Firebase] [Tailwind]   │  │ [React] [Node] [MongoDB] [Stripe API]      │
 │                                            │  │                                            │
 │ 🔗 Live Demo  |  💻 GitHub                 │  │ 🔗 Live Demo  |  💻 GitHub                 │
 ╰────────────────────────────────────────────╯  ╰────────────────────────────────────────────╯

 ╭────────────────────────────────────────────╮  ╭────────────────────────────────────────────╮
 │ 💬 Real Time Chat Application              │  │ 📊 Zomato Sales Analysis                   │
 │ Instant Messaging & Community Hub          │  │ Massive Data Visualization & Analytics     │
 │                                            │  │                                            │
 │ ⚡ Complex Multi-Role Channels             │  │ ⚡ Highly Interactive PowerBI Dashboards   │
 │ ⚡ E2E Protocol Encryption Ready           │  │ ⚡ Predictive Trend & Sales Forecasting    │
 │ ⚡ Heavy Media Sharing Optimization        │  │ ⚡ Dynamic Real-Time Revenue Tracking      │
 │ ⚡ Sub-millisecond Typing Indicators       │  │ ⚡ Deep Segmented Geographic Insights      │
 │ ⚡ Live WebRTC Presence Tracking           │  │ ⚡ Automated Scheduled Custom Reporting    │
 │                                            │  │                                            │
 │ [React] [Socket.IO] [Node] [Redis Cache]   │  │ [React] [PowerBI] [SQL] [Node Backend]     │
 │                                            │  │                                            │
 │ 🔗 Live Demo  |  💻 GitHub                 │  │ 🔗 Live Demo  |  💻 GitHub                 │
 ╰────────────────────────────────────────────╯  ╰────────────────────────────────────────────╯

 ╭────────────────────────────────────────────╮  ╭────────────────────────────────────────────╮
 │ 🌍 Land Portal                             │  │ 🌌 Portfolio Website                       │
 │ Specialized Terrain & Land Booking         │  │ Cyberpunk Developer Showcase               │
 │                                            │  │                                            │
 │ ⚡ Real-Time Heavy Geo-location Mapping    │  │ ⚡ Premium Intensive Glassmorphism UI      │
 │ ⚡ Immutable Blockchain Deed Verification  │  │ ⚡ Custom Optimized 3D WebGL Visualization │
 │ ⚡ Secure Automated Escrow Payment System  │  │ ⚡ Silky Smooth Framer Motion Animations   │
 │ ⚡ AI-Driven Dynamic Area Pricing          │  │ ⚡ Ultra Responsive Fluid Mobile Layout    │
 │ ⚡ Comprehensive Master Admin Dashboard    │  │ ⚡ Fully Animated HTML Terminal Emulator   │
 │                                            │  │                                            │
 │ [MERN] [Mapbox API] [Express] [JWT Auth]   │  │ [React] [Tailwind] [Three.js] [Vercel]     │
 │                                            │  │                                            │
 │ 🔗 Live Demo  |  💻 GitHub                 │  │ 🔗 Live Demo  |  💻 GitHub                 │
 ╰────────────────────────────────────────────╯  ╰────────────────────────────────────────────╯
    <strong style="color: #7B61FF; font-family: 'Courier New', monospace; font-size: 20px;">Backend Architecture & Extreme Scale</strong><br>
    <img src="https://progress-bar.dev/90/?scale=100&title=Advanced&width=850&color=7B61FF&suffix=%" alt="Backend" /><br><br>
    
    <strong style="color: #FF00FF; font-family: 'Courier New', monospace; font-size: 20px;">Redis & BullMQ Asynchronous Data Flows</strong><br>
    <img src="https://progress-bar.dev/85/?scale=100&title=Intermediate&width=850&color=FF00FF&suffix=%" alt="Redis" /><br><br>
    
    <strong style="color: #00FF9D; font-family: 'Courier New', monospace; font-size: 20px;">Docker Micro-Containerization</strong><br>
    <img src="https://progress-bar.dev/75/?scale=100&title=Learning&width=850&color=00FF9D&suffix=%" alt="Docker" /><br><br>
    
    <strong style="color: #00F5FF; font-family: 'Courier New', monospace; font-size: 20px;">Complex Highly Available System Design</strong><br>
    <img src="https://progress-bar.dev/80/?scale=100&title=Deep_Dive&width=850&color=00F5FF&suffix=%" alt="System Design" /><br><br>
    
    <strong style="color: #7B61FF; font-family: 'Courier New', monospace; font-size: 20px;">AI Integration & Dynamic Prompting Pipelines</strong><br>
    <img src="https://progress-bar.dev/85/?scale=100&title=Applied&width=850&color=7B61FF&suffix=%" alt="AI" /><br><br>
    
    <strong style="color: #FF00FF; font-family: 'Courier New', monospace; font-size: 20px;">Open Source Ecosystem Expansion</strong><br>
    <img src="https://progress-bar.dev/40/?scale=100&title=Initiating&width=850&color=FF00FF&suffix=%" alt="Open Source" />
  </td>
</tr>
Plaintext
  > FACT_01 : I can accurately debug and reconstruct a deeply complex, massively nested MongoDB aggregation pipeline faster than I can physically decide what to eat for lunch on any given Tuesday.
  
  > FACT_02 : I view frontend UI/UX design not merely as applying pretty CSS styling, but rather as deep, deliberate, and highly calculated psychological user engineering.
  
  > FACT_03 : My personal ZSH terminal environment is so heavily, obsessively customized and extensively script-automated that to the untrained eye, it legitimately looks like a raw data feed pulled straight from a hacker scene in The Matrix.
  <linearGradient id="bgWave" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="#00FF9D" stop-opacity="0.3" />
    <stop offset="100%" stop-color="#00F5FF" stop-opacity="0.3" />
  </linearGradient>

  <filter id="glowWave" x="-20%" y="-20%" width="140%" height="140%">
    <feGaussianBlur stdDeviation="8" result="blur" />
    <feComposite in="SourceGraphic" in2="blur" operator="over" />
  </filter>

  <style>
    @keyframes waveAnim1 { 
      0% { transform: translateX(0); } 
      100% { transform: translateX(-1200px); } 
    }
    @keyframes waveAnim2 { 
      0% { transform: translateX(0); } 
      100% { transform: translateX(1200px); } 
    }
    .wave1 { animation: waveAnim1 20s linear infinite; }
    .wave2 { animation: waveAnim2 25s linear infinite reverse; }
    .wave3 { animation: waveAnim1 15s linear infinite; }
    .footer-text { 
      font-family: 'Courier New', monospace; 
      font-size: 18px; 
      fill: #00F5FF; 
      font-weight: 900; 
      letter-spacing: 4px; 
    }
    .pulse-node { animation: pulse 3s infinite; }
  </style>
</defs>

<rect width="100%" height="100%" fill="#0D1117" />

<g class="wave2">
  <path d="M -1200 150 Q -900 200 -600 150 T 0 150 T 600 150 T 1200 150 T 1800 150 T 2400 150 L 2400 250 L -1200 250 Z" fill="url(#bgWave)" />
</g>

<g filter="url(#glowWave)">
  <path class="wave1" d="M 0 120 Q 300 50 600 120 T 1200 120 T 1800 120 T 2400 120 L 2400 250 L 0 250 Z" fill="none" stroke="url(#waveGrad)" stroke-width="5" />
  <path class="wave3" d="M 0 160 Q 300 200 600 160 T 1200 160 T 1800 160 T 2400 160 L 2400 250 L 0 250 Z" fill="none" stroke="#00F5FF" stroke-width="2" stroke-opacity="0.8" />
</g>

<circle cx="200" cy="110" r="4" fill="#00FF9D" class="pulse-node">
  <animate attributeName="cy" values="110;95;110" dur="3.5s" repeatCount="indefinite"/>
</circle>
<circle cx="1000" cy="130" r="5" fill="#FF00FF" class="pulse-node">
  <animate attributeName="cy" values="130;110;130" dur="4.5s" repeatCount="indefinite"/>
</circle>
<circle cx="600" cy="140" r="3" fill="#00F5FF" class="pulse-node">
  <animate attributeName="cy" values="140;125;140" dur="2.5s" repeatCount="indefinite"/>
</circle>
<circle cx="800" cy="170" r="4" fill="#7B61FF" class="pulse-node">
  <animate attributeName="cy" values="170;155;170" dur="5s" repeatCount="indefinite"/>
</circle>

<text x="600" y="220" text-anchor="middle" class="footer-text">DESIGNED & ENGINEERED BY RAKESH CHOURASIA © 2026</text>
