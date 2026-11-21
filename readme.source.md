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

```aura width=560 height=230 inline
<div style={{
  display: 'flex', flexDirection: 'column', justifyContent: 'center',
  width: '100%', height: '100%', padding: 36, borderRadius: 20,
  background: 'linear-gradient(135deg, #2a0f3a, #0b0c12)',
  border: '1px solid rgba(110,80,220,0.18)'
}}>
  <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#7a6f94' }}>ABOUT</div>
  <div style={{ display: 'flex', fontSize: 30, fontWeight: 700, color: '#ffffff', marginTop: 8 }}>Your headline line one</div>
  <div style={{ display: 'flex', fontSize: 30, fontWeight: 700, color: '#ffffff' }}>your headline line two.</div>
  <div style={{ display: 'flex', fontSize: 13, color: '#8b8f9a', marginTop: 16 }}>&gt; your short status line_</div>
</div>
```

```aura width=290 height=230 inline
<div style={{ display: 'flex', flexDirection: 'column', width: '100%', height: '100%' }}>
  <div style={{
    display: 'flex', alignItems: 'center', justifyContent: 'center', flex: 1,
    marginBottom: 10, borderRadius: 20, background: 'linear-gradient(135deg,#1a2a4a,#0b0c12)',
    border: '1px solid rgba(110,80,220,0.18)',
    color: '#9aa0ad', fontSize: 12, letterSpacing: 3
  }}>LABEL ONE</div>
  <div style={{
    display: 'flex', alignItems: 'center', justifyContent: 'center', flex: 1,
    borderRadius: 20, background: 'linear-gradient(135deg,#1a1f4a,#0b0c12)',
    border: '1px solid rgba(110,80,220,0.18)',
    color: '#9aa0ad', fontSize: 12, letterSpacing: 3
  }}>LABEL TWO</div>
</div>
```

```aura width=860 height=190
<div style={{
  display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center',
  width: '100%', height: '100%', borderRadius: 20, background: '#0b0c12',
  border: '1px solid rgba(110,80,220,0.18)'
}}>
  <div style={{ display: 'flex', fontSize: 12, letterSpacing: 4, color: '#555a66', marginBottom: 18 }}>STACK</div>
  <div style={{ display: 'flex', flexWrap: 'wrap', justifyContent: 'center', width: 640 }}>
    {['Skill 1', 'Skill 2', 'Skill 3', 'Skill 4', 'Skill 5', 'Skill 6', 'Skill 7', 'Skill 8'].map(function (t, i) {
      return (
        <div key={t + i} style={{
          display: 'flex', padding: '6px 16px', margin: 5, borderRadius: 999,
          border: '1px solid #2a2d38', color: '#9aa0ad', fontSize: 12
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