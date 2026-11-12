<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 840 670" width="840" height="670">
  <defs>
    <linearGradient id="line" x1="0" x2="1">
      <stop offset="0" stop-color="#0d1117"/>
      <stop offset="0.5" stop-color="#1d4ed8"/>
      <stop offset="1" stop-color="#93c5fd"/>
    </linearGradient>
    <radialGradient id="glow">
      <stop offset="0" stop-color="#93c5fd" stop-opacity="0.45"/>
      <stop offset="1" stop-color="#93c5fd" stop-opacity="0"/>
    </radialGradient>
  </defs>

  <rect width="840" height="670" rx="8" fill="#0d1117"/>
  <rect x="40" y="34" width="760" height="4" fill="url(#line)"/>

  <g font-family="ui-monospace, SFMono-Regular, Menlo, Consolas, monospace" font-size="14" xml:space="preserve">

    <!-- Mond -->
    <circle cx="610" cy="92" r="46" fill="url(#glow)"/>
    <circle cx="610" cy="92" r="18" fill="#dbeafe"/>
    <circle cx="617" cy="86" r="16" fill="#0d1117"/>

    <!-- Sterne -->
    <text fill="#93c5fd">
      <tspan x="140" y="80">      *               .                 +              .        </tspan>
      <animate attributeName="opacity" values="1;0.3;1" dur="3s" repeatCount="indefinite"/>
    </text>
    <text fill="#bfdbfe">
      <tspan x="140" y="100">  .            +            *                    .           *  </tspan>
      <animate attributeName="opacity" values="0.4;1;0.4" dur="4s" repeatCount="indefinite"/>
    </text>
    <text fill="#60a5fa">
      <tspan x="140" y="120">            .                     .        *                    </tspan>
      <animate attributeName="opacity" values="1;0.5;1" dur="5s" repeatCount="indefinite"/>
    </text>

    <!-- Berge -->
    <text fill="#3b82f6">
      <tspan x="140" y="150">                           /\                                     </tspan>
      <tspan x="140" y="168">              /\          /  \               /\                   </tspan>
      <tspan x="140" y="186">             /  \   /\   /    \             /  \    /\            </tspan>
      <tspan x="140" y="204">            /    \ /  \ /      \    /\     /    \  /  \           </tspan>
      <tspan x="140" y="222">     /\    /      /    \        \  /  \   /      \/    \    /\    </tspan>
      <tspan x="140" y="240">    /  \  /      /      \        \/    \ /              \  /  \   </tspan>
      <tspan x="140" y="258">___/    \/                              /                \/    \__</tspan>
    </text>

    <!-- Wasser -->
    <text fill="#2563eb">
      <tspan x="140" y="278">~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</tspan>
    </text>
    <text fill="#60a5fa">
      <tspan x="140" y="296">  ~  ~~   ~~~  ~   ~~ ~    ~~~   ~  ~~    ~   ~~~  ~   ~~  ~  ~   </tspan>
      <animate attributeName="opacity" values="1;0.35;1" dur="3.5s" repeatCount="indefinite"/>
    </text>
    <text fill="#1e40af">
      <tspan x="140" y="314">     ~   ~~    ~     ~~~    ~    ~~     ~~    ~     ~~~    ~      </tspan>
      <animate attributeName="opacity" values="0.35;1;0.35" dur="3.5s" repeatCount="indefinite"/>
    </text>
  </g>

  <line x1="100" y1="340" x2="740" y2="340" stroke="#1e3a8a" stroke-width="1"/>

  <!-- The craft -->
  <g font-family="ui-monospace, SFMono-Regular, Menlo, Consolas, monospace" font-size="15">
    <text x="120" y="385" fill="#93c5fd">the craft</text>
    <line x1="215" y1="380" x2="720" y2="380" stroke="#1e3a8a" stroke-dasharray="4 4"/>

    <rect x="120" y="413" width="10" height="10" fill="#1d4ed8"/>
    <text x="142" y="423" fill="#dbeafe">HTML</text>
    <line x1="260" y1="418" x2="580" y2="418" stroke="#1e3a8a" stroke-dasharray="2 6"/>
    <text x="720" y="423" fill="#60a5fa" text-anchor="end">markup</text>

    <rect x="120" y="443" width="10" height="10" fill="#2563eb"/>
    <text x="142" y="453" fill="#dbeafe">CSS</text>
    <line x1="260" y1="448" x2="580" y2="448" stroke="#1e3a8a" stroke-dasharray="2 6"/>
    <text x="720" y="453" fill="#60a5fa" text-anchor="end">styling</text>

    <rect x="120" y="473" width="10" height="10" fill="#3b82f6"/>
    <text x="142" y="483" fill="#dbeafe">JavaScript</text>
    <line x1="260" y1="478" x2="580" y2="478" stroke="#1e3a8a" stroke-dasharray="2 6"/>
    <text x="720" y="483" fill="#60a5fa" text-anchor="end">logic</text>

    <rect x="120" y="503" width="10" height="10" fill="#60a5fa"/>
    <text x="142" y="513" fill="#dbeafe">Vue.js</text>
    <line x1="260" y1="508" x2="580" y2="508" stroke="#1e3a8a" stroke-dasharray="2 6"/>
    <text x="720" y="513" fill="#60a5fa" text-anchor="end">framework</text>

    <rect x="120" y="533" width="10" height="10" fill="#93c5fd"/>
    <text x="142" y="543" fill="#dbeafe">Git</text>
    <line x1="260" y1="538" x2="560" y2="538" stroke="#1e3a8a" stroke-dasharray="2 6"/>
    <text x="720" y="543" fill="#60a5fa" text-anchor="end">version control</text>
  </g>

  <line x1="100" y1="572" x2="740" y2="572" stroke="#1e3a8a" stroke-width="1"/>

  <text x="420" y="608" font-family="ui-monospace, SFMono-Regular, Menlo, Consolas, monospace"
        font-size="12" fill="#3b82f6" text-anchor="middle" letter-spacing="2">
    · ~ · ALWAYS LEARNING · ~ · ALWAYS BUILDING · ~ ·
  </text>

  <rect x="40" y="632" width="760" height="4" fill="url(#line)"/>
</svg>
