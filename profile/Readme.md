# About
라온아크테크 스마트건축팀


<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart AX Team GitHub Banner (Light Mode)</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&family=Inter:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            background-color: #F1F5F9; /* Slate 100 */
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            margin: 0;
            font-family: 'Inter', sans-serif;
        }
        /* GitHub README Standard Width Container */
        .banner-container {
            width: 850px;
            height: 350px;
            /* Light Background: Subtle Gradient from White to Light Blue-Grey */
            background: radial-gradient(circle at top left, #FFFFFF 0%, #F8FAFC 100%);
            border-radius: 16px;
            position: relative;
            overflow: hidden;
            border: 1px solid #E2E8F0; /* Light Grey Border */
            /* Soft Shadow instead of Glow */
            box-shadow: 0 20px 40px -10px rgba(15, 23, 42, 0.05);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .grid-bg {
            background-image: 
                linear-gradient(rgba(148, 163, 184, 0.1) 1px, transparent 1px),
                linear-gradient(90deg, rgba(148, 163, 184, 0.1) 1px, transparent 1px);
            background-size: 30px 30px;
            position: absolute;
            inset: 0;
        }
        .font-mono {
            font-family: 'JetBrains Mono', monospace;
        }
    </style>
</head>
<body>

    <!-- 
      [업데이트 사항]
      1. 로고 외곽: 회색(Gray) 처리
      2. 내부 큐브: 선 색상 검은색(Black) 처리
      3. 윗면: 분할선 제거 (깔끔한 Rhombus 형태)
      4. 하이라이트: 8시 방향(왼쪽 면)으로 이동
    -->
    <div class="banner-container">
        <!-- Background Effects -->
        <div class="grid-bg"></div>
        <!-- Right Side Subtle Blue Wash -->
        <div class="absolute top-0 right-0 w-2/3 h-full bg-gradient-to-l from-blue-50/50 to-transparent pointer-events-none"></div>
        
        <div class="flex items-center space-x-12 z-10">
            
            <!-- Graphic: Refined Logo Version -->
            <div class="relative transform scale-125">
                <svg width="140" height="140" viewBox="0 0 100 100" fill="none" class="drop-shadow-lg">
                    <!-- 1. Outer Hexagon: More Transparent & Thinner (Background Element) -->
                    <!-- Changed stroke color to rgba for transparency, reduced stroke-width to 0.8 -->
                    <path d="M50 15 L85 35 V75 L50 95 L15 75 V35 L50 15 Z" stroke="rgba(148, 163, 184, 0.4)" stroke-width="0.8" stroke-linejoin="round"/>
                    
                    <!-- 2. Core Cube Outline: Transparent Fill to show grid -->
                    <!-- Reduced stroke-width from 2 to 1.2 -->
                    <path d="M50 25 L75 40 V70 L50 85 L25 70 V40 L50 25 Z" fill="rgba(248, 250, 252, 0.3)" stroke="#000000" stroke-width="1.2" stroke-linejoin="round"/>
                    
                    <!-- 3. Internal Y-Lines: Black (Removed Top Vertical Line 'M50 25 V55') -->
                    <!-- Reduced stroke-width from 2 to 1.2 -->
                    <path d="M25 40 L50 55 L75 40 M50 55 V85" stroke="#000000" stroke-width="1.2" stroke-linejoin="round"/>
                    
                    <!-- 4. Highlight: Moved to 8 o'clock face (Bottom-Left Face) -->
                    <!-- Vertices: Center(50,55) -> Top-Left(25,40) -> Bottom-Left(25,70) -> Bottom(50,85) -->
                    <path d="M50 55 L25 40 V70 L50 85 Z" fill="#0EA5E9" opacity="0.1">
                        <animate attributeName="opacity" values="0.1;0.4;0.1" dur="3s" repeatCount="indefinite" />
                    </path>
                    
                    <!-- Active Nodes -->
                    <circle cx="25" cy="40" r="3" fill="#0891B2" stroke="#FFFFFF" stroke-width="1">
                        <animate attributeName="r" values="3;5;3" dur="2s" repeatCount="indefinite" />
                    </circle>
                    <circle cx="75" cy="40" r="2.5" fill="#94A3B8" stroke="#FFFFFF" stroke-width="1"/>
                    <circle cx="50" cy="85" r="2.5" fill="#94A3B8" stroke="#FFFFFF" stroke-width="1"/>
                    
                    <!-- Scan Line Animation -->
                    <line x1="15" y1="50" x2="85" y2="50" stroke="#0891B2" stroke-width="1.5" stroke-dasharray="3 3">
                        <animate attributeName="y1" values="35;75;35" dur="4s" repeatCount="indefinite" />
                        <animate attributeName="y2" values="35;75;35" dur="4s" repeatCount="indefinite" />
                        <animate attributeName="opacity" values="0;1;0" dur="4s" repeatCount="indefinite" />
                    </line>
                </svg>
            </div>

            <!-- Text Content -->
            <div class="flex flex-col justify-center">
                <div class="flex items-center space-x-2 mb-2">
                    <span class="w-2 h-2 rounded-full bg-cyan-600 animate-pulse"></span>
                    <span class="text-cyan-700 text-xs font-bold tracking-widest uppercase font-mono">Laon ArcTec Computational Div.</span>
                </div>
                
                <h1 class="text-5xl font-black text-slate-900 tracking-tight mb-2">
                    SMART <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-600 to-blue-700">AX</span> TEAM
                </h1>
                
                <p class="text-slate-500 text-sm tracking-wide font-light border-l-2 border-slate-300 pl-3">
                    Construction-Technology: Contech Platform<br>
                    <span class="text-slate-600 font-medium">DX (Data Transformation) &bull; AX (AI Transformation)</span>
                </p>

                <!-- Badge Area -->
                <div class="flex space-x-2 mt-5 opacity-90">
                    <div class="h-1.5 w-8 bg-blue-700 rounded-full"></div>
                    <div class="h-1.5 w-8 bg-cyan-600 rounded-full"></div>
                    <div class="h-1.5 w-8 bg-slate-400 rounded-full"></div>
                </div>
            </div>
        </div>
        
        <!-- Decoration Corner -->
        <div class="absolute bottom-4 right-6 text-right">
            <div class="text-[10px] text-slate-400 font-mono">Group family: NAMKWANG-KUKDONG</div>
            <div class="text-[10px] text-slate-400 font-mono">STATUS: <span class="text-green-600 font-bold">ONLINE</span></div>
        </div>
    </div>

</body>
</html>
