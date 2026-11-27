```aura width=860 height=400 link="https://github.com/ShravyaMalogi"
<div style={{
  width: '100%', height: '100%', background: '#08080c',
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 20,
  border: '1px solid rgba(110,80,220,0.18)'
}}>
  <style>{`
    @keyframes orb-a { 0%,100% { transform: translate(0px,0px); opacity: 0.8; } 50% { transform: translate(260px,70px); opacity: 1; } }
    @keyframes orb-b { 0%,100% { transform: translate(0px,0px); opacity: 0.75; } 50% { transform: translate(-240px,90px); opacity: 1; } }
    @keyframes orb-c { 0%,100% { transform: translate(0px,0px); opacity: 0.7; } 50% { transform: translate(220px,-90px); opacity: 1; } }
    @keyframes orb-d { 0%,100% { transform: translate(0px,0px); opacity: 0.75; } 50% { transform: translate(-200px,-80px); opacity: 1; } }
    @keyframes orb-pulse { 0%,100% { transform: scale(1); opacity: 0.85; } 50% { transform: scale(1.3); opacity: 0.45; } }
    #glow-1 { animation: orb-a 12s ease-in-out infinite; }
    #glow-2 { animation: orb-b 14s ease-in-out infinite; }
    #glow-3 { animation: orb-c 11s ease-in-out infinite; }
    #glow-4 { animation: orb-d 13s ease-in-out infinite; }
    #glow-5 { animation: orb-pulse 8s ease-in-out infinite; transform-box: fill-box; transform-origin: center; }
    #glow-6 { animation: orb-pulse 10s ease-in-out infinite reverse; transform-box: fill-box; transform-origin: center; }
  `}</style>

  <svg width="860" height="400" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110,20,210,0.55)" />
        <stop offset="45%" stopColor="rgba(90,15,180,0.25)" />
        <stop offset="70%" stopColor="rgba(90,15,180,0)" />
      </radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(40,60,255,0.5)" />
        <stop offset="45%" stopColor="rgba(30,50,200,0.2)" />
        <stop offset="70%" stopColor="rgba(30,50,200,0)" />
      </radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,170,230,0.38)" />
        <stop offset="70%" stopColor="rgba(0,170,230,0)" />
      </radialGradient>
      <radialGradient id="g4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(160,30,255,0.48)" />
        <stop offset="50%" stopColor="rgba(130,20,220,0.18)" />
        <stop offset="70%" stopColor="rgba(130,20,220,0)" />
      </radialGradient>
      <radialGradient id="g5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(100,50,240,0.42)" />
        <stop offset="70%" stopColor="rgba(100,50,240,0)" />
      </radialGradient>
      <radialGradient id="g6" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(30,90,255,0.4)" />
        <stop offset="70%" stopColor="rgba(30,90,255,0)" />
      </radialGradient>
    </defs>
    <ellipse id="glow-1" cx="150" cy="110" rx="250" ry="190" fill="url(#g1)" />
    <ellipse id="glow-2" cx="700" cy="90" rx="240" ry="180" fill="url(#g2)" />
    <ellipse id="glow-3" cx="260" cy="320" rx="230" ry="160" fill="url(#g3)" />
    <ellipse id="glow-4" cx="660" cy="320" rx="240" ry="170" fill="url(#g4)" />
    <ellipse id="glow-5" cx="430" cy="200" rx="200" ry="150" fill="url(#g5)" />
    <ellipse id="glow-6" cx="820" cy="210" rx="170" ry="140" fill="url(#g6)" />
  </svg>

  <div style={{ display: 'flex', fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px' }}>
    {github?.user?.login || 'ShravyaMalogi'}
  </div>
  <div style={{ display: 'flex', marginTop: 12, fontSize: 14, letterSpacing: 8, color: 'rgba(200,185,255,0.85)' }}>
    THOUGHTS · TRIALS · BREAKTHROUGHS
  </div>
  <div style={{ display: 'flex', marginTop: 28 }}>
    {['Artificial Intelligence', 'Machine Learning & Data', 'Workflow Automation'].map(function (tag, i) {
      return (
        <div key={tag + i} style={{
          display: 'flex', padding: '6px 18px', marginRight: 10, borderRadius: 999,
          background: 'rgba(80,40,220,0.22)', border: '1px solid rgba(100,70,240,0.38)',
          color: 'rgba(215,205,255,0.92)', fontSize: 12, fontWeight: 600
        }}>{tag}</div>
      );
    })}
  </div>
</div>
```

```aura width=860 height=250
<div style={{ display: 'flex', width: '100%', height: '100%', fontFamily: 'Inter' }}>
  <style>{`
    @keyframes drift-r { 0%,100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(240px); opacity: 1; } }
    @keyframes drift-l { 0%,100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-220px); opacity: 1; } }
    @keyframes pulse { 0%,100% { transform: scale(1); opacity: 0.85; } 50% { transform: scale(1.35); opacity: 0.4; } }
    @keyframes blink { 0%,100% { opacity: 1; } 50% { opacity: 0; } }
    @keyframes sweep { 0% { transform: translateX(0px); opacity: 0; } 15% { opacity: 1; } 85% { opacity: 1; } 100% { transform: translateX(370px); opacity: 0; } }
    #a-glow-1 { animation: drift-r 10s ease-in-out infinite; }
    #a-glow-2 { animation: drift-l 13s ease-in-out infinite; }
    #a-glow-3 { animation: pulse 8s ease-in-out infinite; transform-box: fill-box; transform-origin: center; }
    #c-glow-1 { animation: pulse 6s ease-in-out infinite; transform-box: fill-box; transform-origin: center; }
    #c-beam { animation: sweep 4s linear infinite; }
    #cursor { animation: blink 1s steps(1) infinite; }
  `}</style>

  <svg width="860" height="250" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <clipPath id="clip-b"><rect x="572" y="0" width="288" height="119" rx="20" /></clipPath>
      <clipPath id="clip-c"><rect x="572" y="131" width="288" height="119" rx="20" /></clipPath>
      <filter id="soft" filterUnits="userSpaceOnUse" x="572" y="0" width="288" height="119">
        <feGaussianBlur stdDeviation="6" />
      </filter>
      <radialGradient id="gb1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,130,255,0.5)" />
        <stop offset="50%" stopColor="rgba(0,100,220,0.2)" />
        <stop offset="70%" stopColor="rgba(0,100,220,0)" />
      </radialGradient>
      <linearGradient id="gbeam" x1="0" y1="0" x2="1" y2="0">
        <stop offset="0%" stopColor="rgba(120,180,255,0)" />
        <stop offset="50%" stopColor="rgba(120,180,255,0.3)" />
        <stop offset="100%" stopColor="rgba(120,180,255,0)" />
      </linearGradient>
    </defs>
    <rect x="572" y="0" width="288" height="119" rx="20" fill="#0b0c12" />
    <rect x="572" y="131" width="288" height="119" rx="20" fill="#0b0c12" />
    <g clipPath="url(#clip-b)">
      <g filter="url(#soft)">
        <circle cx="716" cy="60" r="7" fill="#c9a8ff">
          <animate attributeName="opacity" values="1;0.35;1" dur="2s" repeatCount="indefinite" />
        </circle>
        <circle cx="716" cy="60" r="8" fill="none" stroke="#a56bff" strokeWidth="3" opacity="0">
          <animate attributeName="r" from="8" to="130" dur="4s" repeatCount="indefinite" />
          <animate attributeName="opacity" from="0.8" to="0" dur="4s" repeatCount="indefinite" />
        </circle>
        <circle cx="716" cy="60" r="8" fill="none" stroke="#6f8cff" strokeWidth="3" opacity="0">
          <animate attributeName="r" from="8" to="130" dur="4s" begin="1.33s" repeatCount="indefinite" />
          <animate attributeName="opacity" from="0.8" to="0" dur="4s" begin="1.33s" repeatCount="indefinite" />
        </circle>
        <circle cx="716" cy="60" r="8" fill="none" stroke="#3ac8ff" strokeWidth="3" opacity="0">
          <animate attributeName="r" from="8" to="130" dur="4s" begin="2.66s" repeatCount="indefinite" />
          <animate attributeName="opacity" from="0.8" to="0" dur="4s" begin="2.66s" repeatCount="indefinite" />
        </circle>
      </g>
    </g>
    <g clipPath="url(#clip-c)">
      <ellipse id="c-glow-1" cx="716" cy="266" rx="150" ry="70" fill="url(#gb1)" />
      <rect id="c-beam" x="502" y="131" width="70" height="119" fill="url(#gbeam)" />
    </g>
  </svg>

  <div style={{
    display: 'flex', position: 'relative', overflow: 'hidden',
    width: 560, height: 250, marginRight: 12, borderRadius: 20,
    background: '#0b0c12', border: '1px solid rgba(110,80,220,0.18)'
  }}>
    <svg width="560" height="250" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="ga1" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(120,25,210,0.6)" />
          <stop offset="45%" stopColor="rgba(90,15,180,0.25)" />
          <stop offset="70%" stopColor="rgba(90,15,180,0)" />
        </radialGradient>
        <radialGradient id="ga2" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(40,60,255,0.5)" />
          <stop offset="50%" stopColor="rgba(30,50,200,0.2)" />
          <stop offset="70%" stopColor="rgba(30,50,200,0)" />
        </radialGradient>
        <radialGradient id="ga3" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(160,30,255,0.4)" />
          <stop offset="70%" stopColor="rgba(160,30,255,0)" />
        </radialGradient>
      </defs>
      <ellipse id="a-glow-1" cx="120" cy="270" rx="240" ry="150" fill="url(#ga1)" />
      <ellipse id="a-glow-2" cx="440" cy="280" rx="200" ry="130" fill="url(#ga2)" />
      <ellipse id="a-glow-3" cx="300" cy="270" rx="150" ry="100" fill="url(#ga3)" />
    </svg>
    <div style={{ display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: 36 }}>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#8a7fa8' }}>ABOUT</div>
      <div style={{ display: 'flex', fontSize: 30, fontWeight: 700, color: '#ffffff', marginTop: 8 }}>A little curiosity.</div>
      <div style={{ display: 'flex', fontSize: 30, fontWeight: 700, color: '#ffffff' }}>A lot of figuring things out.</div>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 16 }}>
        <div style={{ display: 'flex', fontSize: 13, color: '#9aa0ad' }}>&gt; open to collaborations _ </div>
        <svg width="8" height="16" style={{ marginLeft: 4 }}>
          <rect id="cursor" x="0" y="2" width="7" height="12" fill="#b9a8ff" />
        </svg>
      </div>
    </div>
  </div>

  <div style={{ display: 'flex', flexDirection: 'column', width: 288, height: 250 }}>
    <div style={{
      display: 'flex', alignItems: 'center', justifyContent: 'center',
      width: 288, height: 119, marginBottom: 12, borderRadius: 20,
      border: '1px solid rgba(110,80,220,0.18)'
    }}>
      <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
        <div style={{ display: 'flex', fontSize: 13, fontWeight: 700, letterSpacing: 3, color: '#ffffff' }}>WHAT IF?</div>
        <div style={{ display: 'flex', fontSize: 13, color: '#cbb6ff', marginTop: 8 }}>It starts with a question</div>
      </div>
    </div>
    <div style={{
      display: 'flex', alignItems: 'center', justifyContent: 'center',
      width: 288, height: 119, borderRadius: 20,
      border: '1px solid rgba(110,80,220,0.18)'
    }}>
      <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
        <div style={{ display: 'flex', fontSize: 13, fontWeight: 700, letterSpacing: 3, color: '#ffffff' }}>WHY NOT?</div>
        <div style={{ display: 'flex', fontSize: 13, color: '#cbb6ff', marginTop: 8 }}>It gets interesting from here</div>
      </div>
    </div>
  </div>
</div>
```

```aura width=860 height=190
<div style={{
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  width: '100%', height: '100%', position: 'relative', overflow: 'hidden',
  borderRadius: 20, background: '#0b0c12', border: '1px solid rgba(110,80,220,0.18)',
  fontFamily: 'Inter'
}}>
  <style>{`
    @keyframes orb-a { 0%,100% { transform: translate(0px,0px); opacity: 0.8; } 50% { transform: translate(240px,35px); opacity: 1; } }
    @keyframes orb-b { 0%,100% { transform: translate(0px,0px); opacity: 0.75; } 50% { transform: translate(-230px,40px); opacity: 1; } }
    @keyframes orb-c { 0%,100% { transform: translate(0px,0px); opacity: 0.7; } 50% { transform: translate(200px,-40px); opacity: 1; } }
    @keyframes orb-d { 0%,100% { transform: translate(0px,0px); opacity: 0.75; } 50% { transform: translate(-190px,-35px); opacity: 1; } }
    @keyframes orb-pulse { 0%,100% { transform: scale(1); opacity: 0.85; } 50% { transform: scale(1.3); opacity: 0.45; } }
    @keyframes twinkle { 0%,100% { opacity: 0.1; } 50% { opacity: 0.9; } }
    #s-glow-1 { animation: orb-a 12s ease-in-out infinite; }
    #s-glow-2 { animation: orb-b 14s ease-in-out infinite; }
    #s-glow-3 { animation: orb-c 11s ease-in-out infinite; }
    #s-glow-4 { animation: orb-d 13s ease-in-out infinite; }
    #s-glow-5 { animation: orb-pulse 8s ease-in-out infinite; transform-box: fill-box; transform-origin: center; }
    #tw-1 { animation: twinkle 3s ease-in-out infinite; }
    #tw-2 { animation: twinkle 4s ease-in-out infinite 1s; }
    #tw-3 { animation: twinkle 5s ease-in-out infinite 2s; }
    #tw-4 { animation: twinkle 3.5s ease-in-out infinite 0.5s; }
    #tw-5 { animation: twinkle 4.5s ease-in-out infinite 1.5s; }
    #tw-6 { animation: twinkle 3.2s ease-in-out infinite 2.5s; }
  `}</style>

  <svg width="860" height="190" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="gs1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110,20,210,0.22)" />
        <stop offset="50%" stopColor="rgba(90,15,180,0.08)" />
        <stop offset="70%" stopColor="rgba(90,15,180,0)" />
      </radialGradient>
      <radialGradient id="gs2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(40,80,255,0.20)" />
        <stop offset="50%" stopColor="rgba(30,60,200,0.07)" />
        <stop offset="70%" stopColor="rgba(30,60,200,0)" />
      </radialGradient>
      <radialGradient id="gs3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,170,230,0.14)" />
        <stop offset="70%" stopColor="rgba(0,170,230,0)" />
      </radialGradient>
      <radialGradient id="gs4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(160,30,255,0.20)" />
        <stop offset="50%" stopColor="rgba(130,20,220,0.07)" />
        <stop offset="70%" stopColor="rgba(130,20,220,0)" />
      </radialGradient>
      <radialGradient id="gs5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(100,50,240,0.16)" />
        <stop offset="70%" stopColor="rgba(100,50,240,0)" />
      </radialGradient>
    </defs>
    <ellipse id="s-glow-1" cx="140" cy="50" rx="220" ry="120" fill="url(#gs1)" />
    <ellipse id="s-glow-2" cx="720" cy="45" rx="210" ry="115" fill="url(#gs2)" />
    <ellipse id="s-glow-3" cx="280" cy="170" rx="200" ry="100" fill="url(#gs3)" />
    <ellipse id="s-glow-4" cx="620" cy="175" rx="210" ry="105" fill="url(#gs4)" />
    <ellipse id="s-glow-5" cx="430" cy="95" rx="170" ry="90" fill="url(#gs5)" />
    <circle id="tw-1" cx="90" cy="40" r="1.6" fill="#ffffff" />
    <circle id="tw-2" cx="250" cy="150" r="1.4" fill="#b9a8ff" />
    <circle id="tw-3" cx="300" cy="26" r="1.8" fill="#ffffff" />
    <circle id="tw-4" cx="600" cy="160" r="1.5" fill="#9fd3ff" />
    <circle id="tw-5" cx="760" cy="45" r="1.6" fill="#ffffff" />
    <circle id="tw-6" cx="820" cy="140" r="1.3" fill="#b9a8ff" />
  </svg>

  <div style={{ display: 'flex', fontSize: 15, fontWeight: 400, letterSpacing: 6, color: '#e4defa', marginBottom: 18 }}>STACK</div>
  <div style={{ display: 'flex', flexWrap: 'wrap', justifyContent: 'center', width: 640 }}>
    {['Python', 'Machine Learning', 'OpenCV', 'Deep Learning(CNNs)', 'TensorFlow', 'Google Sheets', 'SQL', 'n8n', 'RAG', 'Gen AI', 'LangChain', 'LLM APIs', 'REST APIs', 'MCP', 'Streamlit', 'FastAPI', 'Google Cloud (GCP)'].map(function (t, i) {
      return (
        <div key={t + i} style={{
          display: 'flex', padding: '6px 16px', margin: 5, borderRadius: 999,
          background: 'rgba(80,40,220,0.10)', border: '1px solid rgba(100,70,240,0.28)',
          color: '#b4bac6', fontSize: 12
        }}>{t}</div>
      );
    })}
  </div>
</div>
```

```aura width=130 height=44 link="https://shravyamalogi.github.io/portfolio/" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBmaWxsPSIjZmZmZmZmIiBkPSJNMTIgLjI5N2MtNi42MyAwLTEyIDUuMzczLTEyIDEyIDAgNS4zMDMgMy40MzggOS44IDguMjA1IDExLjM4NS42LjExMy44Mi0uMjU4LjgyLS41NzcgMC0uMjg1LS4wMS0xLjA0LS4wMTUtMi4wNC0zLjMzOC43MjQtNC4wNDItMS42MS00LjA0Mi0xLjYxQzQuNDIyIDE4LjA3IDMuNjMzIDE3LjcgMy42MzMgMTcuN2MtMS4wODctLjc0NC4wODQtLjcyOS4wODQtLjcyOSAxLjIwNS4wODQgMS44MzggMS4yMzYgMS44MzggMS4yMzYgMS4wNyAxLjgzNSAyLjgwOSAxLjMwNSAzLjQ5NS45OTguMTA4LS43NzYuNDE3LTEuMzA1Ljc2LTEuNjA1LTIuNjY1LS4zLTUuNDY2LTEuMzMyLTUuNDY2LTUuOTMgMC0xLjMxLjQ2NS0yLjM4IDEuMjM1LTMuMjItLjEzNS0uMzAzLS41NC0xLjUyMy4xMDUtMy4xNzYgMCAwIDEuMDA1LS4zMjIgMy4zIDEuMjMuOTYtLjI2NyAxLjk4LS4zOTkgMy0uNDA1IDEuMDIuMDA2IDIuMDQuMTM4IDMgLjQwNSAyLjI4LTEuNTUyIDMuMjg1LTEuMjMgMy4yODUtMS4yMy42NDUgMS42NTMuMjQgMi44NzMuMTIgMy4xNzYuNzY1Ljg0IDEuMjMgMS45MSAxLjIzIDMuMjIgMCA0LjYxLTIuODA1IDUuNjI1LTUuNDc1IDUuOTIuNDIuMzYuODEgMS4wOTYuODEgMi4yMiAwIDEuNjA2LS4wMTUgMi44OTYtLjAxNSAzLjI4NiAwIC4zMTUuMjEuNjkuODI1LjU3QzIwLjU2NSAyMi4wOTIgMjQgMTcuNTkyIDI0IDEyLjI5N2MwLTYuNjI3LTUuMzczLTEyLTEyLTEyIi8+PC9zdmc+"
  text="Portfolio" backgroundColor="#111111" width={130} height={44} iconSize="18" />
```

```aura width=130 height=44 link="https://linkedin.com/in/shravyamalogi" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHJlY3QgZmlsbD0iI2ZmZmZmZiIgeD0iMiIgeT0iOSIgd2lkdGg9IjQiIGhlaWdodD0iMTIiLz48Y2lyY2xlIGZpbGw9IiNmZmZmZmYiIGN4PSI0IiBjeT0iNC41IiByPSIyLjQiLz48cGF0aCBmaWxsPSIjZmZmZmZmIiBkPSJNOSA5aDMuOHYxLjdjLjYtMS4xIDItMiAzLjktMiAzLjYgMCA0LjMgMi40IDQuMyA1LjRWMjFoLTR2LTYuMWMwLTEuNSAwLTMuMS0xLjktMy4xcy0yLjEgMS40LTIuMSAzVjIxSDl6Ii8+PC9zdmc+"
  text="LinkedIn" backgroundColor="#0a1a2a" width={130} height={44} iconSize="18" />
```

```aura width=130 height=44 link="mailto:shravyamwork@gmail.com" inline align=center
<SocialMediaButton icon="data:image/svg+xml;base64,PHN2ZyByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cGF0aCBmaWxsPSIjZmZmZmZmIiBkPSJNMjQgNS40NTd2MTMuOTA5YzAgLjkwNC0uNzMyIDEuNjM2LTEuNjM2IDEuNjM2aC0zLjgxOVYxMS43M0wxMiAxNi42NGwtNi41NDUtNC45MXY5LjI3M0gxLjYzNkExLjYzNiAxLjYzNiAwIDAgMSAwIDE5LjM2NlY1LjQ1N2MwLTIuMDIzIDIuMzA5LTMuMTc4IDMuOTI3LTEuOTY0TDUuNDU1IDQuNjQgMTIgOS41NDhsNi41NDUtNC45MSAxLjUyOC0xLjE0NUMyMS42OSAyLjI4IDI0IDMuNDM0IDI0IDUuNDU3eiIvPjwvc3ZnPg=="
  text="Email" backgroundColor="#1a0a0a" width={130} height={44} iconSize="18" />
```