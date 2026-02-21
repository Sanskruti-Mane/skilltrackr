# SkillTrackr 🚀

SkillTrackr is a collaborative web project built using modern frontend tools.  
This repository is open for contributions and follows a clean Git workflow to keep the code stable and organized.

---

## Branch Strategy (Very Important)

We follow this branching model:

- **main** → Stable / production-ready code (protected)
- **dev** → Active development branch
- **feature/*** → Individual feature branches

### Workflow
feature/* → dev → main


### Rules
- ❌ Do NOT push directly to `main`
- ❌ Do NOT push directly to `dev`
- ✅ Always create a `feature/*` branch
- ✅ Raise a Pull Request to `dev`

Only the repository owner merges `dev` → `main`.

---

## Prerequisites

Make sure the following are installed on your system:

- Git
- Node.js (LTS recommended)
- npm

Check versions:

```bash
git --version
node -v
npm -v
```