```aura width=860 height=320 link="https://github.com/YOUR_USERNAME"
<div style={{
  width: '100%', height: '100%', background: '#08080c',
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 20,
  border: '1px solid rgba(110,80,220,0.18)'
}}>
  <style>{`
    @keyframes float-slow { 0%,100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(300px); opacity: 1; } }
    @keyframes float-medium { 0%,100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-250px); opacity: 1; } }
    @keyframes float-pulse { 0%,100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.3); opacity: 0.4; } }
    #glow-1 { animation: float-slow 9s ease-in-out infinite; }
    #glow-2 { animation: float-medium 12s ease-in-out infinite; }
    #glow-3 { animation: float-slow 11s ease-in-out infinite reverse; }
    #glow-4 { animation: float-pulse 7s ease-in-out infinite; }
  `}</style>

  <svg width="860" height="320" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(110,20,210,0.65)" />
        <stop offset="40%" stopColor="rgba(90,15,180,0.3)" />
        <stop offset="70%" stopColor="rgba(90,15,180,0)" />
      </radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(40,60,255,0.55)" />
        <stop offset="45%" stopColor="rgba(30,50,200,0.22)" />
        <stop offset="70%" stopColor="rgba(30,50,200,0)" />
      </radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,190,230,0.3)" />
        <stop offset="70%" stopColor="rgba(0,190,230,0)" />
      </radialGradient>
      <radialGradient id="g4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(160,30,255,0.5)" />
        <stop offset="70%" stopColor="rgba(130,20,220,0)" />
      </radialGradient>
    </defs>
    <ellipse id="glow-1" cx="200" cy="330" rx="260" ry="190" fill="url(#g1)" />
    <ellipse id="glow-2" cx="420" cy="340" rx="220" ry="160" fill="url(#g2)" />
    <ellipse id="glow-3" cx="620" cy="340" rx="180" ry="140" fill="url(#g3)" />
    <ellipse id="glow-4" cx="450" cy="330" rx="150" ry="120" fill="url(#g4)" />
  </svg>

  <div style={{ display: 'flex', fontSize: 64, fontWeight: 800, color: '#ffffff', letterSpacing: '-1px', zIndex: 10 }}>
    {github?.user?.login || 'YOUR_USERNAME'}
  </div>
  <div style={{ display: 'flex', marginTop: 10, fontSize: 14, letterSpacing: 8, color: 'rgba(180,165,255,0.7)', zIndex: 10 }}>
    WORD ONE · WORD TWO · WORD THREE
  </div>
  <div style={{ display: 'flex', marginTop: 24, zIndex: 10 }}>
    {['tag one', 'tag two', 'tag three'].map(function (tag, i) {
      return (
        <div key={tag + i} style={{
          display: 'flex', padding: '6px 18px', marginRight: 10, borderRadius: 999,
          background: 'rgba(80,40,220,0.18)', border: '1px solid rgba(100,70,240,0.32)',
          color: 'rgba(205,195,255,0.85)', fontSize: 12, fontWeight: 600
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
    #a-glow-1 { animation: drift-r 10s ease-in-out infinite; }
    #a-glow-2 { animation: drift-l 13s ease-in-out infinite; }
    #a-glow-3 { animation: pulse 8s ease-in-out infinite; transform-box: fill-box; transform-origin: center; }
    #b-glow-1 { animation: drift-r 9s ease-in-out infinite; }
    #b-glow-2 { animation: pulse 6s ease-in-out infinite; transform-box: fill-box; transform-origin: center; }
    #c-glow-1 { animation: drift-l 11s ease-in-out infinite; }
    #c-glow-2 { animation: pulse 7s ease-in-out infinite; transform-box: fill-box; transform-origin: center; }
    #cursor { animation: blink 1s steps(1) infinite; }
  `}</style>

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
    <div style={{ display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: 36, zIndex: 10 }}>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#8a7fa8' }}>ABOUT</div>
      <div style={{ display: 'flex', fontSize: 30, fontWeight: 700, color: '#ffffff', marginTop: 8 }}>Your headline line one</div>
      <div style={{ display: 'flex', fontSize: 30, fontWeight: 700, color: '#ffffff' }}>your headline line two.</div>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 16 }}>
        <div style={{ display: 'flex', fontSize: 13, color: '#9aa0ad' }}>&gt; your short status line</div>
        <svg width="8" height="16" style={{ marginLeft: 4 }}>
          <rect id="cursor" x="0" y="2" width="7" height="12" fill="#b9a8ff" />
        </svg>
      </div>
    </div>
  </div>

  <div style={{ display: 'flex', flexDirection: 'column', width: 288, height: 250 }}>
    <div style={{
      display: 'flex', position: 'relative', overflow: 'hidden', alignItems: 'center', justifyContent: 'center',
      width: 288, height: 119, marginBottom: 12, borderRadius: 20,
      background: '#0b0c12', border: '1px solid rgba(110,80,220,0.18)'
    }}>
      <svg width="288" height="119" style={{ position: 'absolute', top: 0, left: 0 }}>
        <defs>
          <radialGradient id="gb1" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(0,130,255,0.5)" />
            <stop offset="50%" stopColor="rgba(0,100,220,0.2)" />
            <stop offset="70%" stopColor="rgba(0,100,220,0)" />
          </radialGradient>
          <radialGradient id="gb2" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(0,190,230,0.35)" />
            <stop offset="70%" stopColor="rgba(0,190,230,0)" />
          </radialGradient>
        </defs>
        <ellipse id="b-glow-1" cx="60" cy="130" rx="150" ry="80" fill="url(#gb1)" />
        <ellipse id="b-glow-2" cx="200" cy="120" rx="90" ry="60" fill="url(#gb2)" />
      </svg>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: '#b4bac6', zIndex: 10 }}>LABEL ONE</div>
    </div>

    <div style={{
      display: 'flex', position: 'relative', overflow: 'hidden', alignItems: 'center', justifyContent: 'center',
      width: 288, height: 119, borderRadius: 20,
      background: '#0b0c12', border: '1px solid rgba(110,80,220,0.18)'
    }}>
      <svg width="288" height="119" style={{ position: 'absolute', top: 0, left: 0 }}>
        <defs>
          <radialGradient id="gc1" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(110,40,240,0.5)" />
            <stop offset="50%" stopColor="rgba(90,30,200,0.2)" />
            <stop offset="70%" stopColor="rgba(90,30,200,0)" />
          </radialGradient>
          <radialGradient id="gc2" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(160,30,255,0.4)" />
            <stop offset="70%" stopColor="rgba(160,30,255,0)" />
          </radialGradient>
        </defs>
        <ellipse id="c-glow-1" cx="230" cy="130" rx="150" ry="80" fill="url(#gc1)" />
        <ellipse id="c-glow-2" cx="90" cy="125" rx="90" ry="60" fill="url(#gc2)" />
      </svg>
      <div style={{ display: 'flex', fontSize: 12, letterSpacing: 3, color: '#b4bac6', zIndex: 10 }}>LABEL TWO</div>
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
    @keyframes drift-r { 0%,100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(300px); opacity: 1; } }
    @keyframes drift-l { 0%,100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-300px); opacity: 1; } }
    @keyframes twinkle { 0%,100% { opacity: 0.1; } 50% { opacity: 0.9; } }
    #s-glow-1 { animation: drift-r 12s ease-in-out infinite; }
    #s-glow-2 { animation: drift-l 15s ease-in-out infinite; }
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
        <stop offset="0%" stopColor="rgba(110,20,210,0.4)" />
        <stop offset="50%" stopColor="rgba(90,15,180,0.15)" />
        <stop offset="70%" stopColor="rgba(90,15,180,0)" />
      </radialGradient>
      <radialGradient id="gs2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(40,80,255,0.35)" />
        <stop offset="50%" stopColor="rgba(30,60,200,0.12)" />
        <stop offset="70%" stopColor="rgba(30,60,200,0)" />
      </radialGradient>
    </defs>
    <ellipse id="s-glow-1" cx="200" cy="200" rx="260" ry="110" fill="url(#gs1)" />
    <ellipse id="s-glow-2" cx="660" cy="205" rx="240" ry="100" fill="url(#gs2)" />
    <circle id="tw-1" cx="90" cy="40" r="1.6" fill="#ffffff" />
    <circle id="tw-2" cx="250" cy="150" r="1.4" fill="#b9a8ff" />
    <circle id="tw-3" cx="420" cy="30" r="1.8" fill="#ffffff" />
    <circle id="tw-4" cx="600" cy="160" r="1.5" fill="#9fd3ff" />
    <circle id="tw-5" cx="760" cy="45" r="1.6" fill="#ffffff" />
    <circle id="tw-6" cx="820" cy="140" r="1.3" fill="#b9a8ff" />
  </svg>

  <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#6b7080', marginBottom: 18, zIndex: 10 }}>STACK</div>
  <div style={{ display: 'flex', flexWrap: 'wrap', justifyContent: 'center', width: 640, zIndex: 10 }}>
    {['Skill 1', 'Skill 2', 'Skill 3', 'Skill 4', 'Skill 5', 'Skill 6', 'Skill 7', 'Skill 8'].map(function (t, i) {
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

```aura width=130 height=44 link="https://github.com/YOUR_USERNAME" inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/github/white" text="GitHub"
  backgroundColor="#111111" width={130} height={44} iconSize="18" />
```

```aura width=130 height=44 link="https://linkedin.com/in/YOUR_LINKEDIN" inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/linkedin/white" text="LinkedIn"
  backgroundColor="#0a1a2a" width={130} height={44} iconSize="18" />
```

```aura width=130 height=44 link="mailto:YOUR_EMAIL@example.com" inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/gmail/white" text="Email"
  backgroundColor="#1a0a0a" width={130} height={44} iconSize="18" />
```