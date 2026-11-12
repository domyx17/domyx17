<svg xmlns="http://www.w3.org/2000/svg" width="900" height="720" viewBox="0 0 900 720">
  <defs>
    <!-- Farbverlauf für die Berge: Schnee oben, tiefblau unten -->
    <linearGradient id="mtn" gradientUnits="userSpaceOnUse" x1="0" y1="125" x2="0" y2="310">
      <stop offset="0" stop-color="#e6f4ff"/>
      <stop offset="0.35" stop-color="#79c0ff"/>
      <stop offset="0.7" stop-color="#388bfd"/>
      <stop offset="1" stop-color="#1f3b73"/>
    </linearGradient>
    <!-- Linien oben/unten -->
    <linearGradient id="line" x1="0" x2="1">
      <stop offset="0" stop-color="#58a6ff" stop-opacity="0"/>
      <stop offset="0.5" stop-color="#1f6feb"/>
      <stop offset="1" stop-color="#a5d6ff"/>
    </linearGradient>
    <!-- Skill-Balken -->
    <linearGradient id="barFill" x1="0" x2="1">
      <stop offset="0" stop-color="#1f3b73"/>
      <stop offset="0.6" stop-color="#388bfd"/>
      <stop offset="1" stop-color="#a5d6ff"/>
    </linearGradient>
    <!-- Segmente für die Balken -->
    <pattern id="seg" width="8" height="20" patternUnits="userSpaceOnUse">
      <rect width="6" height="20" fill="#fff"/>
    </pattern>
    <mask id="segs" maskUnits="userSpaceOnUse" x="0" y="0" width="900" height="720">
      <rect width="900" height="720" fill="url(#seg)"/>
    </mask>

    <style>
      text { font-family: ui-monospace, SFMono-Regular, Consolas, "Liberation Mono", Menlo, monospace; }
      .mtn   { font-size: 14px; white-space: pre; }

      .star  { fill: #cae8ff; font-size: 12px; animation: twinkle 4s ease-in-out infinite; }
      @keyframes twinkle { 0%,100% { opacity: .15 } 50% { opacity: 1 } }

      .flake { fill: #cae8ff; font-size: 13px; opacity: 0; animation: fall 10s linear infinite; }
      @keyframes fall {
        0%   { transform: translate(0, 0);        opacity: 0 }
        10%  { opacity: .9 }
        85%  { opacity: .6 }
        100% { transform: translate(-30px, 270px); opacity: 0 }
      }

      .cloud { fill: #79c0ff; opacity: .35; font-size: 12px; white-space: pre;
               animation: drift 60s linear infinite; }
      @keyframes drift { from { transform: translateX(-250px) } to { transform: translateX(1000px) } }

      .wave  { fill: #388bfd; font-size: 12px; white-space: pre;
               animation: wave 4s ease-in-out infinite alternate; }
      @keyframes wave { from { transform: translateX(-6px); opacity: .3 } to { transform: translateX(6px); opacity: .8 } }

      .moon  { animation: glow 6s ease-in-out infinite; }
      @keyframes glow { 0%,100% { opacity: .7 } 50% { opacity: 1 } }

      .hello { fill: #8b949e; font-size: 13px; text-anchor: middle; }
      .title { fill: #79c0ff; font-size: 14px; letter-spacing: 1px; }
      .label { fill: #cae8ff; font-size: 14px; }
      .pct   { fill: #58a6ff; font-size: 14px; text-anchor: end; }

      .bar   { transform-box: fill-box; transform-origin: left center;
               animation: grow 1.8s cubic-bezier(.2,.8,.2,1) both; }
      @keyframes grow { from { transform: scaleX(0) } to { transform: scaleX(1) } }

      .dot   { fill: #58a6ff; font-size: 13px; text-anchor: middle; animation: twinkle 3s ease-in-out infinite; }
    </style>
  </defs>

  <!-- Hintergrund -->
  <rect width="900" height="720" rx="12" fill="#0d1117"/>
  <rect x="40" y="24" width="820" height="4" fill="url(#line)"/>

  <!-- Sterne -->
  <text class="star" x="120" y="60">+</text>
  <text class="star" x="210" y="95"  style="animation-delay:-1s">·</text>
  <text class="star" x="300" y="55"  style="animation-delay:-2.5s">*</text>
  <text class="star" x="390" y="110" style="animation-delay:-0.5s">·</text>
  <text class="star" x="520" y="65"  style="animation-delay:-3s">+</text>
  <text class="star" x="610" y="100" style="animation-delay:-1.8s">·</text>
  <text class="star" x="680" y="50"  style="animation-delay:-2s">*</text>
  <text class="star" x="840" y="115" style="animation-delay:-0.8s">·</text>
  <text class="star" x="160" y="125" style="animation-delay:-3.4s">·</text>

  <!-- Mond -->
  <g class="moon">
    <circle cx="770" cy="75" r="32" fill="#58a6ff" opacity=".08"/>
    <circle cx="770" cy="75" r="16" fill="#cae8ff"/>
    <circle cx="777" cy="70" r="14" fill="#0d1117"/>
  </g>

  <!-- Wolken -->
  <g class="cloud" style="animation-delay:-20s">
    <text x="0" y="70">   .--.</text>
    <text x="0" y="84">.-(    ).</text>
    <text x="0" y="98">(___.__)__)</text>
  </g>
  <g class="cloud" style="animation-duration:85s; animation-delay:-60s; opacity:.22">
    <text x="0" y="110">  .-~~-.</text>
    <text x="0" y="124">(__.___)_)</text>
  </g>

  <!-- Berge -->
  <g class="mtn" fill="url(#mtn)" xml:space="preserve">
    <text x="80" y="140" textLength="378"   lengthAdjust="spacingAndGlyphs">                                           /\</text>
    <text x="80" y="155" textLength="386.4" lengthAdjust="spacingAndGlyphs">                                          /░░\</text>
    <text x="80" y="170" textLength="579.6" lengthAdjust="spacingAndGlyphs">                                         /░░░░\                    /\</text>
    <text x="80" y="185" textLength="588"   lengthAdjust="spacingAndGlyphs">                   /\                   /▒▒▒▒▒▒\                  /░░\</text>
    <text x="80" y="200" textLength="596.4" lengthAdjust="spacingAndGlyphs">                  /░░\                 /▒▒▒▒▒▒▒▒\                /░░░░\</text>
    <text x="80" y="215" textLength="604.8" lengthAdjust="spacingAndGlyphs">                 /░░░░\               /▒▒▒▒▒▒▒▒▒▒\      /\      /▒▒▒▒▒▒\</text>
    <text x="80" y="230" textLength="613.2" lengthAdjust="spacingAndGlyphs">                /▒▒▒▒▒▒\      /\     /▓▓▓▓▓▓▓▓▓▓▓▓\    /░░\    /▒▒▒▒▒▒▒▒\</text>
    <text x="80" y="245" textLength="705.6" lengthAdjust="spacingAndGlyphs">               /▒▒▒▒▒▒▒▒\    /░░\   /▓▓▓▓▓▓▓▓▓▓▓▓▓▓\  /░░░░\  /▒▒▒▒▒▒▒▒▒▒\        /\</text>
    <text x="80" y="260" textLength="714"   lengthAdjust="spacingAndGlyphs">    /\        /▒▒▒▒▒▒▒▒▒▒\  /░░░░\ /▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓\/▒▒▒▒▒▒\/▓▓▓▓▓▓▓▓▓▓▓▓\      /░░\</text>
    <text x="80" y="275" textLength="722.4" lengthAdjust="spacingAndGlyphs">   /░░\      /▓▓▓▓▓▓▓▓▓▓▓▓\/▒▒▒▒▒▒\▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓/▒▒▒▒▒▒▒▒\▓▓▓▓▓▓▓▓▓▓▓▓▓\    /░░░░\</text>
    <text x="80" y="290" textLength="730.8" lengthAdjust="spacingAndGlyphs">  /░░░░\    /▓▓▓▓▓▓▓▓▓▓▓▓▓/▒▒▒▒▒▒▒▒\▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓/▒▒▒▒▒▒▒▒▒▒\▓▓▓▓▓▓▓▓▓▓▓▓▓\  /▒▒▒▒▒▒\</text>
    <text x="80" y="305" textLength="739.2" lengthAdjust="spacingAndGlyphs"> /▒▒▒▒▒▒\  /▓▓▓▓▓▓▓▓▓▓▓▓▓/▒▒▒▒▒▒▒▒▒▒\▓▓▓▓▓▓▓▓▓▓▓▓▓/▓▓▓▓▓▓▓▓▓▓▓▓\▓▓▓▓▓▓▓▓▓▓▓▓▓\/▒▒▒▒▒▒▒▒\</text>
  </g>

  <!-- Schneeflocken (negative Delays = schon beim Laden verteilt) -->
  <text class="flake" x="110" y="40">·</text>
  <text class="flake" x="170" y="40" style="animation-delay:-3s; animation-duration:12s">*</text>
  <text class="flake" x="240" y="40" style="animation-delay:-6s">·</text>
  <text class="flake" x="310" y="40" style="animation-delay:-1.5s; animation-duration:9s">·</text>
  <text class="flake" x="380" y="40" style="animation-delay:-8s; animation-duration:13s">*</text>
  <text class="flake" x="450" y="40" style="animation-delay:-4.5s">·</text>
  <text class="flake" x="520" y="40" style="animation-delay:-2s; animation-duration:11s">·</text>
  <text class="flake" x="590" y="40" style="animation-delay:-7s">*</text>
  <text class="flake" x="660" y="40" style="animation-delay:-5s; animation-duration:9s">·</text>
  <text class="flake" x="730" y="40" style="animation-delay:-9s; animation-duration:12s">·</text>
  <text class="flake" x="800" y="40" style="animation-delay:-3.5s">*</text>
  <text class="flake" x="850" y="40" style="animation-delay:-6.5s; animation-duration:11s">·</text>

  <!-- Boden + Bergsee -->
  <line x1="60" y1="315" x2="840" y2="315" stroke="#388bfd" stroke-opacity=".6"/>
  <g xml:space="preserve">
    <text class="wave" x="80" y="333">  ~~   ~    ~~~   ~   ~~    ~   ~~~    ~  ~~   ~    ~~~  ~    ~~   ~  ~~~   ~    ~~</text>
    <text class="wave" x="80" y="349" style="animation-delay:-2s">     ~    ~~   ~    ~~~   ~   ~~    ~    ~~   ~   ~~~    ~   ~~    ~    ~~~   ~</text>
  </g>

  <text class="hello" x="450" y="390">hoi, ich bin dominic · applikationsentwickler in ausbildung</text>

  <!-- Skills -->
  <text class="title" x="90" y="440">the stack</text>
  <line x1="190" y1="436" x2="840" y2="436" stroke="#1f6feb" stroke-opacity=".5" stroke-dasharray="4 4"/>

  <text class="label" x="90" y="480">HTML</text>
  <text class="label" x="90" y="510">CSS</text>
  <text class="label" x="90" y="540">JavaScript</text>
  <text class="label" x="90" y="570">Vue</text>
  <text class="label" x="90" y="600">Git</text>

  <g mask="url(#segs)">
    <!-- Hintergrund-Spuren -->
    <rect x="210" y="466" width="560" height="18" fill="#1a2433"/>
    <rect x="210" y="496" width="560" height="18" fill="#1a2433"/>
    <rect x="210" y="526" width="560" height="18" fill="#1a2433"/>
    <rect x="210" y="556" width="560" height="18" fill="#1a2433"/>
    <rect x="210" y="586" width="560" height="18" fill="#1a2433"/>
    <!-- Balken: width = 560 * Prozent -->
    <rect class="bar" x="210" y="466" width="476" height="18" fill="url(#barFill)"/>
    <rect class="bar" x
