# Kubebuilder Auto-Update PoC

## 🎯 Objective
Automatically run `kubebuilder alpha generate` and create PRs when scaffolded files change — paving the way for AI-based conflict resolution.

## ⚙️ How It Works
- A GitHub Action runs `kubebuilder alpha generate` inside `user-defined-project/`
- If there are changes, it creates a PR with updated scaffolding

## 🧪 How to Test Locally
```bash
cd user-defined-project
kubebuilder alpha generate
# then git diff to see changes
