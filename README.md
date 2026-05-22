# Fusion 360 Post-Processor Training — Exercise Files

Hands-on exercises for the **Fusion Post-Processor Training** course. Each exercise uses FANUC post-processor (`.cps`) files so you can practice editing posts in a code editor and verifying your work against reference solutions.

Repository: [Fusion-Post-Processor-Training](https://github.com/rohitmane5/Fusion-Post-Processor-Training)

---

## Getting the exercise files

You do **not** need Git installed. Download the repository as a ZIP and extract it on your computer.

### Option A — Download ZIP (recommended)

1. Open the repository in your browser:  
   **https://github.com/rohitmane5/Fusion-Post-Processor-Training**
2. Click the green **Code** button.
3. Choose **Download ZIP**.
4. Save the file (for example, `Fusion-Post-Processor-Training-main.zip`).
5. Extract the ZIP to a folder you can find easily, for example:
   - `Documents\Fusion-Post-Processor-Training`
6. Open the extracted folder. The exercise content is in:

   ```
   Fusion-Post-Processor-Training-main\
   └── Exercise_Files\
       ├── Day-01\
       ├── Day-02\
       ├── sample CNC files\
       └── README.md          ← this file
   ```

### Option B — Clone with Git (optional)

```bash
git clone https://github.com/rohitmane5/Fusion-Post-Processor-Training.git
cd Fusion-Post-Processor-Training/Exercise_Files
```

---

## Folder layout

| Folder | Contents |
|--------|----------|
| `Day-01\` | Day 1 exercises (`Ex_0` … `Ex_9`), each in its own subfolder |
| `Day-02\` | Reserved for Day 2 exercises (added as the course progresses) |
| `sample CNC files\` | Sample `.cnc` programs for post-processing and proving your changes in Fusion CAM |

Each exercise folder contains one or more FANUC post files (`.cps`).

---

## File naming convention

For every exercise, files follow the same pattern (names may use `Before` / `After` with capital letters in this repo):

| File | Purpose |
|------|---------|
| `fanuc_Before.cps` | **Starting point** — open this file and make the required changes |
| `fanuc_After.cps` | **Expected result** — compare your edited file to this when you are done |
| `fanuc_Advance.cps` | **Optional advanced solution** — provided for some exercises only |

### Exercise workflow

1. **Open** `fanuc_Before.cps` for the exercise you are working on.
2. **Implement** the changes described in the training slides or instructor notes.
3. **Compare** your modified file with `fanuc_After.cps` to confirm you match the expected solution.

> **Tip:** Work on a **copy** of `fanuc_Before.cps` if you want to keep the original unchanged, or edit `fanuc_Before.cps` directly and use `fanuc_After.cps` only for comparison.

---

## Day 1 exercises

| Exercise | Topic | Files included |
|----------|--------|----------------|
| `Ex_0__` | Introduction / baseline FANUC post | Before, After |
| `Ex_1__comments ON vs OFF` | Program comments on vs off | Before, After |
| `Ex_2__tool list ON vs OFF` | Tool list in header on vs off | Before, After |
| `Ex_3__ sequence numbers ON vs OFF` | Sequence numbers on vs off | Before, After |
| `Ex_4__ program name and program number` | Program name and program number | Before only |
| `Ex_5__remove comments and keep tool list` | Remove comments, keep tool list | Before, After |
| `Ex_6__header content requests` | Custom header content | Before, After, Advance |
| `Ex_7__ optional stop after every tool` | Optional stop (M01) after each tool | Before, After, Advance |
| `Ex_8__coolant output is wrong` | Correct coolant M-codes | Before, After |
| `Ex_9__tool change format not accepted` | Tool-change block format | Before, After |

Exercise folder names describe the scenario (for example, “comments ON vs OFF”). Follow the corresponding section in the course presentation **Fusion Post-Processor Training** for step-by-step tasks.

---

## Comparing files in Visual Studio Code

Use the built-in diff view to check your work against `fanuc_After.cps`:

1. Open **both** files in VS Code (your edited `fanuc_Before.cps` and `fanuc_After.cps`).
2. Activate the file you edited (click its tab).
3. Press **F1** to open the Command Palette.
4. Type: `Compare`
5. Select: **File: Compare Active File With...**
6. Choose `fanuc_After.cps` from the list.

VS Code shows the files **side by side** and highlights differences so you can see what still needs to change.

Other editors (Notepad++, WinMerge, etc.) can compare two files the same way if you prefer.

---

## Sample CNC files

The folder `sample CNC files` contains `.cnc` setups you can use in **Fusion 360 CAM** when testing a post:

- `2D.cnc`, `Drilling cycles.cnc`, `coolant codes.cnc`, `mist coolant.cnc`
- `Program Comment.cnc`, `manual NC stock.cnc`, `manual NC non stock - requires customization.cnc`
- `Setup for 4x.cnc`, `5x 3+2.cnc`, `5x simultaneous.cnc`
- `workpieceMaterial.cnc`


---

## Requirements

- [Autodesk Fusion](https://www.autodesk.com/products/fusion-360/overview) with CAM
- A text editor — [Visual Studio Code](https://code.visualstudio.com/) is recommended for JavaScript-based `.cps` posts
- Course slides: **Fusion Post-Processor Training** (provided with the class)

---

## Quick checklist

- [ ] Downloaded and extracted the repository ZIP
- [ ] Located `Exercise_Files\Day-01\` and opened `fanuc_Before.cps` for the current exercise
- [ ] Made the required edits in VS Code (or your editor)
- [ ] Compared your file with `fanuc_After.cps`

---

## Support and updates

- Report issues or request updates via the GitHub repository **Issues** tab.
- Pull the latest ZIP or run `git pull` before each class session so you have new `Day-02` exercises when they are published.

**Copyright** — Post files are based on the Autodesk FANUC post processor. Use in accordance with Autodesk licensing and your training agreement.
