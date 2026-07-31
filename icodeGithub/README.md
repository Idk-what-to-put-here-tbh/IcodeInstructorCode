# Camp Code Library

A shared reference library of example programs for camp instructors, organized by class.

## Structure

```
camp-code-library/ (this repo)
├── TEMPLATE-Class-Name/       <- copy this to start a new class
│   ├── example-01-name/
│   │   └── main.py
│   └── example-02-name/
│       └── main.py
├── Drone-Coding/               <- sample class, filled in as a model
│   ├── example-01-hello-world/
│   │   └── hello_world.py
│   ├── example-02-basic-movement/
│   │   └── basic_movement.py
│   └── example-03-square-flight/
│       └── square_flight.py
└── (add more class folders here)
```

## Conventions

- One top-level folder per class (e.g. `Drone-Coding`, `Robotics`, `Game-Dev`).
- Inside each class folder, one subfolder per example program, numbered in teaching order: `example-01-...`, `example-02-...`.
- Each example folder holds just the code file(s) needed to run that example — no extra scaffolding required.

## Access levels

Two tiers, set in the repo's Settings → Collaborators:

- **Write access** — for instructors who'll contribute regularly. They can upload and commit straight to `main`, no review needed.
- **Read access** — for everyone else. They can't push directly, so their only path in is forking the repo and opening a pull request. You (or another Write-access person) review and merge it. This is the built-in "oops did this wrong" safety net — nothing lands in the main library without a look first.

## How to add an example

**If you have Write access** (no git experience needed, all through the GitHub website):

1. Open the class folder on GitHub (or create a new class folder by clicking "Add file" → "Create new file" and typing something like `Robotics/example-01-line-follower/placeholder.txt` as the filename — GitHub creates both folders automatically when you commit).
2. Click "Add file" → "Upload files" inside the example folder and drag in the code file(s).
3. Commit straight to `main`.

**If you have Read access:**

1. Click "Fork" on the repo to make your own copy.
2. Add or edit files in your fork the same way as above.
3. Click "Contribute" → "Open pull request" to submit it for review. Once approved, it gets merged into the main library.

## First-time setup (whoever owns the repo)

1. Create an empty repo on GitHub, e.g. `camp-code-library`.
2. From inside this folder, run:

```
git init
git add .
git commit -m "Initial camp code library"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```

3. In Settings → Collaborators, add regular contributors with Write access and everyone else with Read access.
