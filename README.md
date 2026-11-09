import pypandoc

content = r'''<div align="center">

# 👋 Hi, I'm Dũngkon

### `Frontend Developer` · `Creative Builder` · `Tech Enthusiast`

**Turning ideas into clean interfaces and useful digital experiences.**

[![GitHub followers](https://img.shields.io/github/followers/dungkon2002?style=for-the-badge&logo=github&label=Followers&color=181717)](https://github.com/dungkon2002)
[![Profile views](https://komarev.com/ghpvc/?username=dungkon2002&style=for-the-badge&color=0ea5e9)](https://github.com/dungkon2002)
[![Website](https://img.shields.io/badge/Website-dungkon.com-0ea5e9?style=for-the-badge&logo=googlechrome&logoColor=white)](https://dungkon.com)

<br />

<a href="https://github.com/dungkon2002">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=38BDF8&center=true&vCenter=true&width=650&lines=Building+for+the+web+%F0%9F%8C%90;Learning%2C+creating%2C+improving+every+day;React+%7C+TypeScript+%7C+Node.js;The+future+is+built+one+commit+at+a+time." alt="Typing SVG" />
</a>

</div>

---

## 🚀 About Me

```js
const dungkon = {
  name: "Nguyễn Đinh Tiến Dũng",
  nickname: "Dũngkon",
  role: "Frontend Developer",
  focus: ["React", "TypeScript", "JavaScript", "Node.js"],
  currentlyLearning: ["Modern Frontend", "UI/UX", "Backend Development"],
  mindset: "Learn continuously. Build consistently. Improve relentlessly.",
  website: "https://dungkon.com",
  github: "https://github.com/dungkon2002"
};
```

- 💻 I enjoy building websites, APIs, and practical tools.
- 🎨 I care about clean UI, smooth interactions, and maintainable code.
- 🌱 I'm continuously improving my skills in the JavaScript ecosystem.
- ⚡ I like turning real-world ideas into working products.
- 🎯 My goal: grow into a professional developer and build products people love.

## 🧰 Tech Stack

<div align="center">

### Frontend
<img src="https://skillicons.dev/icons?i=html,css,js,ts,react,vite,tailwind" alt="Frontend skills" />

### Backend & Database
<img src="https://skillicons.dev/icons?i=nodejs,express,java,spring,sqlite,mysql" alt="Backend skills" />

### Tools & Workflow
<img src="https://skillicons.dev/icons?i=git,github,vscode,figma,postman,cloudflare,linux" alt="Tools" />

</div>

## 📌 Featured Projects

> A few projects and experiments from my development journey.

| Project | Description | Stack |
|---|---|---|
| **Dũngkon API** | A collection of useful APIs and developer utilities. | Node.js · Express |
| **Thùng Phim** | A web project focused on movie discovery and shared viewing experiences. | Node.js · EJS |
| **TikTok Live Temple RPC** | An interactive livestream experience driven by real-time events. | Node.js · WebSocket |
| **DKTool** | Tools and automation experiments for practical workflows. | JavaScript · Node.js |

Explore more on **[my repositories](https://github.com/dungkon2002?tab=repositories)**.

## 📊 GitHub Overview

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=dungkon2002&show_icons=true&hide_border=true&rank_icon=github&theme=transparent&title_color=38bdf8&icon_color=38bdf8" alt="GitHub stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=dungkon2002&layout=compact&hide_border=true&theme=transparent&title_color=38bdf8" alt="Top languages" />

<br />

<img width="95%" src="https://streak-stats.demolab.com?user=dungkon2002&hide_border=true&theme=transparent&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8" alt="GitHub streak" />

</div>

## 🐍 Contribution Journey

<div align="center">

<img src="https://raw.githubusercontent.com/dungkon2002/dungkon2002/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake animation" />

</div>

<details>
<summary><b>Enable the contribution snake animation</b></summary>

Create `.github/workflows/snake.yml` in your profile repository and add:

```yml
name: Generate contribution snake

on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

permissions:
  contents: write

jobs:
  generate:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
      - uses: crazy-max/ghaction-github-pages@v4
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

</details>

## 🌐 Find Me Around the Web

<div align="center">

[![GitHub](https://img.shields.io/badge/GitHub-dungkon2002-181717?style=for-the-badge&logo=github)](https://github.com/dungkon2002)
[![Website](https://img.shields.io/badge/Website-dungkon.com-0ea5e9?style=for-the-badge&logo=googlechrome&logoColor=white)](https://dungkon.com)
[![Facebook](https://img.shields.io/badge/Facebook-dungkon2002-0866FF?style=for-the-badge&logo=facebook&logoColor=white)](https://facebook.com/dungkon2002)
[![TikTok](https://img.shields.io/badge/TikTok-@dungkon2002-000000?style=for-the-badge&logo=tiktok)](https://www.tiktok.com/@dungkon2002)
[![YouTube](https://img.shields.io/badge/YouTube-@dungkon-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtube.com/@dungkon)

</div>

---

<div align="center">

### ✨ Keep building. Keep learning. Keep moving forward.

*“Great things are built one small improvement at a time.”*

<sub>© Dũngkon · Designed with curiosity and a little bit of code.</sub>

</div>
'''

output_path = "/mnt/data/README.md"
pypandoc.convert_text(content, "md", format="md", outputfile=output_path, extra_args=["--standalone"])
print(output_path)
