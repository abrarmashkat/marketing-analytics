# Marketing Analytics — Your Course Repository

This is your repository for the whole course. Each homework arrives as its own
folder — `hw00/`, `hw01/`, … `hw14/` — and everything you submit stays here.

**Start with [`hw00/`](hw00/).** It is ungraded. Its only job is to prove your
environment works before the first graded homework arrives.

---

## First-time setup — do this once, before the first graded homework

### 1. This repository is yours

You created it from the course template. It is private unless you chose
otherwise, and nobody on the course can see it yet. That is the point of step 2.

### 2. Install the course app on this repository

Go to **<https://github.com/apps/nu-mktg-grader/installations/new>**, choose **Only select repositories**, and select
this repository.

**Why this is needed, plainly:** this repository belongs to you, so the course
has no access to it by default. The app is how graded homework is delivered into
it and how your feedback is written back. It can read and write repository
contents and nothing else — it cannot see your other repositories, and you can
remove it whenever you like from **Settings → Applications → Installed GitHub
Apps**.

**Confirm it worked:** <https://github.com/settings/installations> should list
**NU-mktg-grader**, with this repository under it.

⚠️ **Do this before the first graded homework is released.** Assignments are
pushed to the repositories the app can reach. If it cannot reach yours, the
assignment never arrives — and nothing on your end will look broken.

### 3. Open your Codespace

Green **Code** button → **Codespaces** tab → **Create codespace on main**.

The first build takes a few minutes. It installs Python 3.11 and every library
this course uses, pinned to exact versions — that pinning is what keeps your
results consistent with what the grader expects, so please do not upgrade
packages.

**You only ever create one.** This single repository holds every homework, so one
Codespace serves the whole course. When you come back, you *reopen* it — see
below.

⚠️ **The editor opens before the install has finished.** The libraries are still
downloading in the background for the first few minutes, even though everything
looks ready. If you run `hw00` immediately and a library is "not found", that is
what is happening — **wait a couple of minutes and run it again.** Do not rebuild
and do not install anything yourself.

### 4. Run `hw00`

Open `hw00/homework_00_introduction.ipynb`.

**Pick the right Python first.** The first time you open a notebook, VS Code asks
which Python to run it with. Click **Select Kernel** at the top right and choose the
**Python 3.11.x** entry — **not** the Python 3.13 one. Only 3.11 has the course
libraries installed, so choosing the other one makes every `import` fail and looks
exactly like a broken Codespace. VS Code asks again for each new notebook file, so
you will do this once per homework.

**Then run it from a clean state:** click **Restart** in the notebook toolbar, then
click **Run All**. They are two separate buttons, sitting next to **Clear All
Outputs** — VS Code has no single "restart and run all" command.

If it finishes with no errors, you are set up. The first cell tells you which
libraries are missing if any are, and whether it is still installing.

---

## Git, in the four commands you actually need

**This whole repository is ONE git repository.** The `hwNN/` folders are just
folders inside it, not separate projects — so you run git from the repository
root, which is exactly where the Codespace terminal opens, and one commit can
cover whatever you changed.

| command | what it does |
|---|---|
| `git pull` | brings *down* anything new — this is how a new homework folder appears |
| `git add .` | stages your changes: marks them to be included in the next save |
| `git commit -m "completed hw01"` | saves a snapshot **locally**, inside your Codespace |
| `git push` | sends your commits *up* to GitHub — **nothing is submitted until you push** |

`add` → `commit` → `push` is one sequence, and you will run all three every time.
`git status` shows what you have changed; `git log --oneline` shows what you have
already committed.

**If `git push` is rejected,** it means new homework was added to your repository
since you last pulled. This is normal and is not something you did wrong:

```bash
git pull
git push
```

---

## Every homework

1. **`git pull`** — the assignment appears as a new `hwNN/` folder
2. Open `hwNN/homework_NN_*.ipynb` and replace every `None` with your answer
3. Pick the kernel: **Select Kernel** (top right) → **Python 3.11.x**, not Python 3.13. VS Code asks this for every new
   notebook file, so it is a per-homework step, not only a first-time one.
4. Run it clean: **Restart**, then **Run All** (two separate toolbar buttons). Your notebook must run top to bottom from a
   fresh kernel.
5. Submit:

```bash
git add .
git commit -m "completed hw01"
git push
```

6. Your feedback appears as **`hwNN/GRADE.md`** — run `git pull` to read it.

## How your work gets graded

After you push, the course's grading system picks up your latest commit, grades
it, and writes your feedback into this repository as **`hwNN/GRADE.md`**. It runs
every couple of hours, so allow some time — and push early rather than once at
the deadline, since every push is regraded.

`GRADE.md` names the commit it graded, so you can always tell whether the
feedback you are reading is for your latest work.

⚠️ **`hw00` is ungraded and produces no `GRADE.md`.** If none appears for hw00,
nothing is wrong — hw00's confirmation is the notebook running clean.

---

## Working across more than one sitting

You do not have to finish a homework in one go.

- **Closing the browser is safe.** Your Codespace stops by itself after about 30
  minutes of inactivity, and everything you saved is still there when you reopen
  it.
- **Reopen the same one.** Go to your repository's **Code → Codespaces** tab, or
  to <https://github.com/codespaces>, and click the Codespace you already have.
  Do not create a second one.
- ⚠️ **Push before a long break.** GitHub deletes a stopped Codespace after **30
  days without use, and it does that even if it holds work you never pushed.**
  Once your work is pushed, the Codespace is disposable: if it ever disappears,
  create a new one and everything is still on GitHub.
- **Mind your free hours.** A free GitHub account includes 120 core-hours per
  month, which is **60 hours** on the default 2-core machine. Stop your Codespace
  when you finish for the day — <https://github.com/codespaces> → `…` →
  **Stop codespace** — rather than leaving it idling.

---

## Your numbers are your own

Part A of each homework uses constants generated for you specifically, so your
classmates' numbers are different and a copied answer is wrong by construction.
Part A is individual work. Parts B and C permit collaboration; each of you
submits your own work.

---

## Using AI agents

This course expects you to work with an agent — the agent can interpret, propose
and flag, and you verify, catch its errors and own the result. GitHub Copilot is
already installed in your Codespace. See the course site's *AI agent usage guide*
for what is expected and what counts as your own work.

---

*Questions? Post to the Canvas discussion or come to office hours.*
