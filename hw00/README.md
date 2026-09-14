# Homework 0: Setup Verification
### Marketing Analytics — **ungraded**

---

## What this is for

This homework has no math and carries no marks. It exists to prove three things
work before the first graded homework arrives:

1. Your Codespace builds and every course library imports
2. You can run a notebook and render LaTeX
3. You can commit and push from the Codespace terminal

## What to do

**Step 1 — open `homework_00_introduction.ipynb`.**

**Pick the right Python first.** The first time you open a notebook, VS Code asks
which Python to run it with. Click **Select Kernel** at the top right and choose the
**Python 3.11.x** entry — **not** the Python 3.13 one. Only 3.11 has the course
libraries installed, so choosing the other one makes every `import` fail and looks
exactly like a broken Codespace. VS Code asks again for each new notebook file, so
you will do this once per homework.

**Then run it from a clean state:** click **Restart** in the notebook toolbar, then
click **Run All**. They are two separate buttons, sitting next to **Clear All
Outputs** — VS Code has no single "restart and run all" command.

⚠️ In a brand-new Codespace the libraries are still installing for the first few
minutes even though the editor looks ready. If something is "not found", wait a
couple of minutes and run it again rather than rebuilding.

**Step 2 — replace each `None` with your answer,** then **Restart** and **Run All**
again.

**Step 3 — push it:**

```bash
git add .
git commit -m "completed hw00"
git push
```

## How you know it worked

**The notebook itself is the confirmation.** The first cell imports every library
this course uses and prints its version; the final cell reports how many of your
answers are still `None`. If both run without errors, your environment is
correct.

That first cell also writes a small file, **`setup_report.json`**, recording your
Python version, each library's version, which ones failed, and whether you ran in
a Codespace. It contains nothing personal. **Commit it with your work** — it is
how the course confirms your environment is right, and how we can spot a broken
library and help you before it costs you a homework.

⚠️ **This homework is ungraded, so no `GRADE.md` will appear for it.** That is
expected — do not wait for feedback here. Graded homework (hw01 onward) does
produce a `hwNN/GRADE.md`.

Separately, confirm the course app is installed at
<https://github.com/settings/installations> — **NU-mktg-grader** should be listed
with this repository. Without it, hw01 will never be delivered to you.

---

*Questions? Post to the Canvas discussion or come to office hours.*
