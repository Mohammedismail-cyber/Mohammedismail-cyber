

<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&display=swap');

  .pixel-wrap {
    background: #0d0d12;
    padding: 40px 24px 36px;
    border-radius: 16px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0;
    font-family: 'Space Mono', monospace;
  }

  .pixel-word {
    display: flex;
    gap: 8px;
    justify-content: center;
  }

  .pixel-word + .pixel-word {
    margin-top: 10px;
  }

  .pixel-letter {
    display: grid;
    gap: 3px;
  }

  .px {
    width: 14px;
    height: 14px;
    border-radius: 2px;
  }

  .px.on {
    background: #a78bfa;
    box-shadow: inset 0 0 0 1.5px #7c3aed;
  }

  .px.off {
    background: transparent;
  }

  .tagline {
    margin-top: 22px;
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    color: #6d5fa8;
    letter-spacing: 0.2em;
    text-transform: uppercase;
  }

  .version-badge {
    margin-top: 10px;
    font-family: 'Space Mono', monospace;
    font-size: 10px;
    color: #4c1d95;
    background: #1e1533;
    padding: 4px 14px;
    border-radius: 20px;
    border: 1px solid #3b0764;
    letter-spacing: 0.15em;
  }
</style>

<div class="pixel-wrap">

<script>
const FONT = {
  M: [
    [1,0,0,0,1],
    [1,1,0,1,1],
    [1,0,1,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
  ],
  O: [
    [0,1,1,1,0],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [0,1,1,1,0],
  ],
  H: [
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,1,1,1,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
  ],
  A: [
    [0,1,1,1,0],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,1,1,1,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
  ],
  E: [
    [1,1,1,1,1],
    [1,0,0,0,0],
    [1,0,0,0,0],
    [1,1,1,1,0],
    [1,0,0,0,0],
    [1,0,0,0,0],
    [1,1,1,1,1],
  ],
  D: [
    [1,1,1,0,0],
    [1,0,0,1,0],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,1,0],
    [1,1,1,0,0],
  ],
  S: [
    [0,1,1,1,1],
    [1,0,0,0,0],
    [1,0,0,0,0],
    [0,1,1,1,0],
    [0,0,0,0,1],
    [0,0,0,0,1],
    [1,1,1,1,0],
  ],
  N: [
    [1,0,0,0,1],
    [1,1,0,0,1],
    [1,0,1,0,1],
    [1,0,0,1,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
    [1,0,0,0,1],
  ],
};

function renderWord(letters) {
  const wrap = document.createElement('div');
  wrap.className = 'pixel-word';
  for (const ch of letters) {
    const grid = FONT[ch];
    const letterDiv = document.createElement('div');
    letterDiv.className = 'pixel-letter';
    letterDiv.style.gridTemplateColumns = `repeat(${grid[0].length}, 14px)`;
    letterDiv.style.gridTemplateRows = `repeat(${grid.length}, 14px)`;
    for (const row of grid) {
      for (const cell of row) {
        const px = document.createElement('div');
        px.className = 'px ' + (cell ? 'on' : 'off');
        letterDiv.appendChild(px);
      }
    }
    wrap.appendChild(letterDiv);
  }
  return wrap;
}

const container = document.currentScript.parentElement;

container.appendChild(renderWord(['M','O','H','A','M','M','E','D']));
container.appendChild(renderWord(['O','S','M','A','N']));

const tag = document.createElement('div');
tag.className = 'tagline';
tag.textContent = 'Full-Stack Developer · Creative Technologist';
container.appendChild(tag);

const badge = document.createElement('div');
badge.className = 'version-badge';
badge.textContent = 'v2025.NAIROBI';
container.appendChild(badge);
</script>

</div>


[![Typing SVG](https://readme-typing-svg.demolab.com?font=Space+Mono&size=16&duration=3000&pause=800&color=63B3FF&center=true&vCenter=true&multiline=true&repeat=true&width=600&height=80&lines=Full-Stack+Developer+%E2%80%A2+Creative+Technologist;Building+world-class+digital+experiences+%F0%9F%9A%80)](https://git.io/typing-svg)

</div>

---

<div align="center">

### `> whoami`

</div>

```yaml
name:        Mohamed Osman
location:    Nairobi, Kenya 🌍
role:        Full-Stack Developer & Creative Technologist
status:      Building • Shipping • Scaling
philosophy:  Design should feel expensive.
             Systems should feel invisible.
             Technology should feel cinematic.
```

---

<div align="center">

### `> ls -la ./expertise`

</div>

| Domain | Focus |
|--------|-------|
| ⚡ **Full-Stack Development** | End-to-end web & mobile systems |
| 🎨 **Modern UI/UX Engineering** | Motion-rich, premium interfaces |
| ☁️ **Cloud & DevOps** | Scalable infrastructure, Docker, Linux |
| 🤖 **AI-Powered Applications** | Intelligent, automated digital products |
| 🏠 **Real Estate Media** | Drone, 360° tours, immersive platforms |
| 🎬 **Cinematic Content** | Video editing, brand identity, YouTube |

---

<div align="center">

### `> cat ./stack.json`

</div>

**Frontend**

![React](https://img.shields.io/badge/React-0B1022?style=for-the-badge&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-1E3A8A?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-111827?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-082F49?style=for-the-badge&logo=tailwindcss&logoColor=38BDF8)
![GSAP](https://img.shields.io/badge/GSAP-111827?style=for-the-badge&logo=greensock&logoColor=88CE02)

**Backend & APIs**

![Node.js](https://img.shields.io/badge/Node.js-0F172A?style=for-the-badge&logo=nodedotjs&logoColor=6DA55F)
![Express](https://img.shields.io/badge/Express-111827?style=for-the-badge&logo=express&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-111827?style=for-the-badge&logo=laravel&logoColor=FF2D20)
![PHP](https://img.shields.io/badge/PHP-1E293B?style=for-the-badge&logo=php&logoColor=777BB4)
![Python](https://img.shields.io/badge/Python-0B1022?style=for-the-badge&logo=python&logoColor=3776AB)
![REST API](https://img.shields.io/badge/REST_API-111827?style=for-the-badge&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-111827?style=for-the-badge&logo=postgresql&logoColor=4169E1)
![MySQL](https://img.shields.io/badge/MySQL-0F172A?style=for-the-badge&logo=mysql&logoColor=4479A1)
![Supabase](https://img.shields.io/badge/Supabase-111827?style=for-the-badge&logo=supabase&logoColor=3ECF8E)
![SQLite](https://img.shields.io/badge/SQLite-0B1022?style=for-the-badge&logo=sqlite&logoColor=003B57)

**DevOps & Infrastructure**

![Docker](https://img.shields.io/badge/Docker-0B1022?style=for-the-badge&logo=docker&logoColor=2496ED)
![Linux](https://img.shields.io/badge/Linux-111827?style=for-the-badge&logo=linux&logoColor=FCC624)
![Git](https://img.shields.io/badge/Git-0F172A?style=for-the-badge&logo=git&logoColor=F05032)
![GitHub](https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-111827?style=for-the-badge&logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-0B1022?style=for-the-badge&logo=netlify&logoColor=00C7B7)

---

<div align="center">

### `> ./projects --status=active`

</div>

```
┌─────────────────────────────────────────────────────────────┐
│  🚀  AI-powered website systems         [IN PROGRESS]       │
│  🌊  Smart water delivery platform      [IN PROGRESS]       │
│  🏢  Real estate immersive media        [IN PROGRESS]       │
│  🧠  Advanced dashboard architectures  [IN PROGRESS]       │
│  ⚡  Modern SaaS-style client systems   [IN PROGRESS]       │
│  🎨  Premium UI motion systems (GSAP)   [IN PROGRESS]       │
│  🛠️  Website-to-HTML conversion tools   [IN PROGRESS]       │
└─────────────────────────────────────────────────────────────┘
```

---

<div align="center">

### `> cat ./creative_stack.md`

</div>

> 📸 Professional Photography &nbsp;·&nbsp; 🎬 Cinematic Video Editing &nbsp;·&nbsp; 🚁 Drone Content Production
>
> 🏠 Real Estate Digital Marketing &nbsp;·&nbsp; 🌍 360° Virtual Tours &nbsp;·&nbsp; 🎥 YouTube Content Production
>
> ✨ Premium Brand Identity Systems

---

<div align="center">

### `> git log --oneline --learning`

</div>

```diff
+ AI Infrastructure
+ Automation Systems
+ Advanced DevOps
+ Scalable Backend Architectures
+ High-Performance Frontend Systems
~ Quantum Computing Concepts  [exploring]
```

---

<div align="center">

### `> npm run stats`

</div>

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Mohammedismail-cyber&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=63b3ff&icon_color=00ffa3&text_color=8899aa)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Mohammedismail-cyber&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=63b3ff&text_color=8899aa)

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=Mohammedismail-cyber&theme=tokyonight&hide_border=true&background=0d1117&stroke=63b3ff&ring=00ffa3&fire=fbbf24&currStreakLabel=63b3ff&sideLabels=8899aa&dates=8899aa)

</div>

---

<div align="center">

### `> echo $PHILOSOPHY`

</div>

```
  "Design should feel expensive."
  "Systems should feel invisible."
  "Technology should feel cinematic."
                                        — Mohamed Osman
```

---

<div align="center">

**`> ping Mohamed`**

💼 Open to collaborations &nbsp;·&nbsp; 🌍 Nairobi, Kenya &nbsp;·&nbsp; 🚀 Building world-class digital experiences

---

*Turning ideas into scalable digital experiences — one commit at a time.*

![Profile Views](https://komarev.com/ghpvc/?username=Mohammedismail-cyber&color=63b3ff&style=flat-square&label=PROFILE+VIEWS)

</div>
