
<style>
@import url('https://fonts.googleapis.com/css2?family=Instrument+Serif:ital@0;1&family=Geist+Mono:wght@300;400;500&display=swap');

*{box-sizing:border-box;margin:0;padding:0}
:root{
  --ink:#0f0f0f;
  --ink2:#555;
  --ink3:#999;
  --rule:rgba(0,0,0,0.1);
  --bg:#fafaf8;
  --serif:'Instrument Serif',serif;
  --mono:'Geist Mono',monospace;
}
@media(prefers-color-scheme:dark){
  :root{--ink:#efefeb;--ink2:#aaa;--ink3:#666;--rule:rgba(255,255,255,0.1);--bg:#111}
}

body{background:var(--bg);color:var(--ink);font-family:var(--mono);padding:0}

.page{max-width:660px;margin:0 auto;padding:3rem 2rem 4rem}

.masthead{border-bottom:1px solid var(--ink);padding-bottom:1.5rem;margin-bottom:1.5rem}
.name-row{display:flex;align-items:baseline;justify-content:space-between;gap:1rem;flex-wrap:wrap}
.name{font-family:var(--serif);font-size:52px;line-height:1;letter-spacing:-1px;color:var(--ink)}
.name em{font-style:italic;color:var(--ink2)}
.location{font-size:11px;color:var(--ink3);letter-spacing:0.12em;text-transform:uppercase;align-self:flex-end;padding-bottom:4px}

.tagstrip{display:flex;gap:0;margin-top:1rem;border:1px solid var(--ink)}
.tag{flex:1;text-align:center;padding:6px 0;font-size:10px;letter-spacing:0.1em;text-transform:uppercase;color:var(--ink2);border-right:1px solid var(--ink)}
.tag:last-child{border-right:none}

.body-grid{display:grid;grid-template-columns:1fr 1fr;gap:0;border:1px solid var(--ink);margin-bottom:0}
.col{padding:1.5rem}
.col+.col{border-left:1px solid var(--ink)}

.col-label{font-size:9px;letter-spacing:0.18em;text-transform:uppercase;color:var(--ink3);margin-bottom:1rem;display:block}

.bio-line{display:flex;align-items:baseline;gap:0.5rem;margin-bottom:0.5rem}
.bio-key{font-size:10px;color:var(--ink3);min-width:56px;flex-shrink:0;letter-spacing:0.04em}
.bio-val{font-size:12px;color:var(--ink);line-height:1.5}
.bio-val a{color:inherit;text-decoration:none}

.stack-list{display:flex;flex-wrap:wrap;gap:6px}
.stk{font-size:10px;padding:3px 8px;border:1px solid var(--rule);color:var(--ink2);letter-spacing:0.03em}
.stk.hi{border-color:var(--ink);color:var(--ink)}

.projects-section{border:1px solid var(--ink);border-top:none}
.projects-head{display:flex;align-items:center;justify-content:space-between;padding:0.75rem 1.5rem;border-bottom:1px solid var(--ink)}
.projects-head span{font-size:9px;letter-spacing:0.18em;text-transform:uppercase;color:var(--ink3)}
.projects-head a{font-size:10px;color:var(--ink2);text-decoration:none;letter-spacing:0.06em}

.project-row{display:grid;grid-template-columns:1fr auto;align-items:start;gap:1rem;padding:1.1rem 1.5rem;border-bottom:1px solid var(--rule);cursor:pointer}
.project-row:last-child{border-bottom:none}
.project-row:hover .proj-name{text-decoration:underline;text-underline-offset:3px}
.proj-name{font-size:13px;font-weight:500;letter-spacing:0.01em;color:var(--ink);margin-bottom:3px}
.proj-desc{font-size:11px;color:var(--ink2);line-height:1.6}
.proj-tags{display:flex;gap:5px;margin-top:7px;flex-wrap:wrap}
.ptag{font-size:9px;letter-spacing:0.08em;text-transform:uppercase;color:var(--ink3);background:transparent;padding:0}
.ptag::before{content:'#'}
.proj-arrow{font-size:16px;color:var(--ink3);margin-top:1px;flex-shrink:0}

.footer-bar{display:flex;justify-content:space-between;align-items:center;border:1px solid var(--ink);border-top:none;padding:0.75rem 1.5rem}
.footer-left{font-size:10px;color:var(--ink3);letter-spacing:0.06em}
.footer-links{display:flex;gap:1.5rem}
.flink{font-size:10px;color:var(--ink2);text-decoration:none;letter-spacing:0.06em;cursor:pointer}
.flink:hover{color:var(--ink)}

@media(max-width:500px){
  .body-grid{grid-template-columns:1fr}
  .col+.col{border-left:none;border-top:1px solid var(--ink)}
  .name{font-size:38px}
  .tagstrip{flex-wrap:wrap}
  .tag{flex:none;width:50%;border-bottom:1px solid var(--ink)}
}
</style>

<div class="page">

  <div class="masthead">
    <div class="name-row">
      <div class="name">Yash <em>Gadia</em></div>
      <div class="location">Greater Noida, IN</div>
    </div>
    <div class="tagstrip">
      <div class="tag">Full-Stack Dev</div>
      <div class="tag">Co-founder @ Qlaa</div>
      <div class="tag">Intern @ SpeedoExpress</div>
      <div class="tag">B.Tech + M.Tech CS</div>
    </div>
  </div>

  <div class="body-grid">
    <div class="col">
      <span class="col-label">about</span>
      <div class="bio-line"><span class="bio-key">school</span><span class="bio-val">NIET, 2024–29</span></div>
      <div class="bio-line"><span class="bio-key">currently</span><span class="bio-val">building AI-powered tools & marketplace platforms</span></div>
      <div class="bio-line"><span class="bio-key">interests</span><span class="bio-val">web3, AI/ML, developer tooling</span></div>
      <div class="bio-line"><span class="bio-key">contact</span><span class="bio-val"><a onclick="openLink('mailto:yash113gadia@gmail.com')">yash113gadia@gmail.com</a></span></div>
    </div>
    <div class="col">
      <span class="col-label">technologies</span>
      <div class="stack-list">
        <span class="stk hi">TypeScript</span>
        <span class="stk hi">React</span>
        <span class="stk hi">Next.js</span>
        <span class="stk hi">Node.js</span>
        <span class="stk">Python</span>
        <span class="stk">FastAPI</span>
        <span class="stk">Three.js</span>
        <span class="stk">MongoDB</span>
        <span class="stk">Postgres</span>
        <span class="stk">Docker</span>
        <span class="stk">Solidity</span>
        <span class="stk">Firebase</span>
      </div>
    </div>
  </div>

  <div class="projects-section">
    <div class="projects-head">
      <span>selected projects</span>
      <a onclick="openLink('https://github.com/yash113gadia')">all repos →</a>
    </div>

    <div class="project-row" onclick="openLink('https://github.com/yash113gadia/codepilot')">
      <div>
        <div class="proj-name">codepilot</div>
        <div class="proj-desc">AI coding agent that runs in your terminal. Works with Anthropic, OpenAI, Google, and local Ollama models.</div>
        <div class="proj-tags"><span class="ptag">typescript</span><span class="ptag">cli</span><span class="ptag">ai</span></div>
      </div>
      <div class="proj-arrow">↗</div>
    </div>

    <div class="project-row" onclick="openLink('https://github.com/yash113gadia/attestr')">
      <div>
        <div class="proj-name">attestr</div>
        <div class="proj-desc">Decentralized media authenticator — steganographic watermarking with Ethereum blockchain verification.</div>
        <div class="proj-tags"><span class="ptag">solidity</span><span class="ptag">web3</span><span class="ptag">react</span></div>
      </div>
      <div class="proj-arrow">↗</div>
    </div>

    <div class="project-row" onclick="openLink('https://github.com/yash113gadia/FitTrack')">
      <div>
        <div class="proj-name">fittrack</div>
        <div class="proj-desc">AI nutrition tracker with barcode scanning, photo analysis, and Gemini-powered dietary advice. React Native + Expo.</div>
        <div class="proj-tags"><span class="ptag">react native</span><span class="ptag">expo</span><span class="ptag">gemini</span></div>
      </div>
      <div class="proj-arrow">↗</div>
    </div>

    <div class="project-row" onclick="openLink('https://github.com/yash113gadia/SyllabusAI')">
      <div>
        <div class="proj-name">syllabusai</div>
        <div class="proj-desc">Paste any syllabus, receive a personalised AI study plan with daily schedules.</div>
        <div class="proj-tags"><span class="ptag">typescript</span><span class="ptag">ai</span><span class="ptag">edtech</span></div>
      </div>
      <div class="proj-arrow">↗</div>
    </div>

    <div class="project-row" onclick="openLink('https://github.com/yash113gadia/AttendEase-Web')">
      <div>
        <div class="proj-name">attendease</div>
        <div class="proj-desc">Real-time attendance tracking for colleges. Teachers mark attendance live; students see updates instantly.</div>
        <div class="proj-tags"><span class="ptag">react</span><span class="ptag">node</span><span class="ptag">postgres</span></div>
      </div>
      <div class="proj-arrow">↗</div>
    </div>

    <div class="project-row" onclick="openLink('https://yashgadia.vercel.app')">
      <div>
        <div class="proj-name">portfolio ↗ live</div>
        <div class="proj-desc">3D animated site with custom cursor, scroll-driven animations, and grain overlays. React + Three.js.</div>
        <div class="proj-tags"><span class="ptag">three.js</span><span class="ptag">react</span><span class="ptag">animation</span></div>
      </div>
      <div class="proj-arrow">↗</div>
    </div>
  </div>

  <div class="footer-bar">
    <div class="footer-left">github.com/yash113gadia</div>
    <div class="footer-links">
      <span class="flink" onclick="openLink('https://yashgadia.vercel.app')">portfolio</span>
      <span class="flink" onclick="openLink('https://linkedin.com/in/yashgadia')">linkedin</span>
      <span class="flink" onclick="openLink('mailto:yash113gadia@gmail.com')">email</span>
    </div>
  </div>

</div>
