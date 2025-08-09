# Forky

Welcome to **Forky** — a fork-friendly development convention designed to make upstream code changes ✨ clean ✨, 😌 safe 😌, and 💥 merge-proof 💥.

When you work in a fork of a large codebase (like Telegram), it’s easy to fall into chaos: silent overwrites, messy merges, mystery bugs caused by untracked changes…

That’s where **Forky**, born inside Darlingram, comes in.

---

## ✨ What is Forky?

**Forky** is not just a tool. It’s a mindset.

It’s a simple but powerful convention:
> 🧠 “All changes to upstream code must be explicit, visible, and respectful.”

It means that all your edits, tweaks, and interventions into upstream files should be *intentionally marked* and *structurally predictable*. This enables:

- 💬 Safer merges from upstream
- 🔍 Automated detection of unmarked changes
- 🛠 Easier debugging (you always know what’s yours)
- 🤝 Cleaner collaboration on forks

Forky is built to grow — with tools, scripts, and possibly even plugins.

---

## 🪄 Origin Story

Forky was born when [Darlingram](https://github.com/Darlingram/Darlingram-Android) — already a fork of Telegram —
when we added a second copy of upstream Telegram as a Git submodule.

> We forked Telegram,
> then added Telegram as a submodule
> *inside the same repo.*

That metaphysical moment — a fork watching its own origin —
sparked the creation of Forky: a tiny guardian of merge sanity and diff cleanliness.

---

## 🧩 What does Forky include?

- 📎 **Structured comment conventions** — so your additions are always wrapped in safe, searchable markers.
- 🔍 **Checker Gradle Task** — validates that no upstream code was accidentally overwritten, and all inserted code is properly marked.

You can think of it like a seatbelt:
> It won’t stop you from driving into a tree,
> but it’ll make sure you’re not flung into production headfirst 🚗🌳

## 📜 Live Templates

Use the provided `LiveTemplates.txt` file to insert common fork patterns quickly and consistently.

💡 **How to import:**
1. Open [LiveTemplates](LiveTemplates.txt) and select all text (`Ctrl+A`)
2. In Android Studio, go to `File → Settings → Editor → Live Templates`
3. Click the `+` button → `Template Group` → name it **Forky**
4. With the new group selected, press `Ctrl+V` to paste the templates
5. Click `OK` — your Forky templates are ready!

---

## 🛠 How to use

1. **Don't touch upstream directly**.
2. Wrap all changes with Forky markers using Live Templates or manually.
3. Run the Forky checker script to validate changes.
4. Stay smug during every upstream merge 😌

---

## 📚 Coming Soon

- 📖 Full documentation of patterns
- 💡 JetBrains plugin for syntax support, navigation & highlighting
- 🧪 CI integration
- 💬 Community feedback (maybe?)

---

> Forky doesn’t stop you from changing upstream.
> Forky helps you avoid being eaten alive the next time upstream changes you.
