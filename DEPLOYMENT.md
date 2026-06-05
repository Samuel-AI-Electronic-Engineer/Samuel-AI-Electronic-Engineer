# GitHub Profile README — Deployment Guide
## Samuel Alarcón Hernández · AI Systems Engineer

---

## FOLDER STRUCTURE

```
samuel-alarcon/          ← Repository name must match your GitHub username
├── README.md            ← Main profile file (rendered on your GitHub profile)
└── assets/
    └── banner.svg       ← Custom SVG hero banner
```

---

## DEPLOYMENT INSTRUCTIONS

### Step 1 — Create the special profile repository
1. Go to https://github.com/new
2. Set repository name **exactly equal to your GitHub username**  
   (e.g. if your username is `samuel-alarcon`, the repo must be `samuel-alarcon`)
3. Check ✅ **Public**
4. Check ✅ **Add a README file**
5. Click **Create repository**

### Step 2 — Upload the files
```bash
# Clone the new repository
git clone https://github.com/YOUR-USERNAME/YOUR-USERNAME.git
cd YOUR-USERNAME

# Copy the files
cp /path/to/README.md ./README.md
mkdir -p assets
cp /path/to/assets/banner.svg ./assets/banner.svg

# Commit and push
git add .
git commit -m "feat: deploy mission control profile"
git push origin main
```

### Step 3 — Update your links
Replace these placeholders in `README.md` before pushing:

| Placeholder | Replace with |
|---|---|
| `samuel-alarcon` | Your actual GitHub username |
| `samuel.alarcon@email.com` | Your real email |
| `linkedin.com/in/samuel-alarcon` | Your real LinkedIn URL |

### Step 4 — Verify
Go to `https://github.com/YOUR-USERNAME` — your profile now renders the full README.

---

## GITHUB STATS SETUP

The stats cards use [github-readme-stats](https://github.com/anuraghazra/github-readme-stats).

They work automatically with your username. For private repo stats, deploy your own instance:
```
https://github.com/anuraghazra/github-readme-stats#deploy-on-your-own
```

---

## RECOMMENDED FUTURE IMPROVEMENTS

### Phase 1 · Quick Wins (1–2 weeks)
- [ ] Add a `GitHub Activity Graph` using `https://github-readme-activity-graph.vercel.app`
- [ ] Add `GitHub Streak Stats` via `https://github-readme-streak-stats.herokuapp.com`
- [ ] Pin your top 6 repositories on your profile page (Settings → Pinned)
- [ ] Add real project links once repos go public

### Phase 2 · Content Upgrades (1 month)
- [ ] Create a short demo GIF for SmartInventoryAI and embed it in the README
- [ ] Add a `PROJECTS.md` with detailed architecture diagrams for each project
- [ ] Set up GitHub Actions to auto-update "Last active" timestamp in the README
- [ ] Write a `RESEARCH.md` documenting your technical explorations

### Phase 3 · Advanced Features (2–3 months)
- [ ] Deploy a personal portfolio site (Vercel/GitHub Pages) and link it from profile
- [ ] Publish technical articles on Dev.to or Medium and display them via RSS widget
- [ ] Add a GitHub Action that auto-generates a "Latest Blog Posts" section
- [ ] Create a WakaTime integration to show live coding activity stats

### Phase 4 · Brand Amplification
- [ ] Add your GitHub profile link to your LinkedIn, CV, and email signature
- [ ] Record a 60-second video walkthrough of SmartInventoryAI for LinkedIn
- [ ] Engage in open source AI/IoT projects to grow your follower base
- [ ] Submit your profile to GitHub Profile README galleries and communities

---

## NOTES ON GITHUB MARKDOWN LIMITATIONS

GitHub README renders HTML but with restrictions:
- ✅ `<div>`, `<table>`, `<img>`, `<br>` are supported
- ✅ `align` attribute on `<div>` and `<td>` works
- ✅ SVG images render correctly
- ❌ `<style>` tags are stripped (use inline attributes or badge services)
- ❌ JavaScript is never executed
- ❌ CSS animations in SVG work only when SVG is loaded as `<img>` (which GitHub does)

The SVG banner uses native SVG `<animate>` elements — these render and animate correctly in GitHub's image renderer.

---

*Profile engineered for Samuel Alarcón Hernández · Electronic Engineer · Colombia 🇨🇴*
