---
student: awais
date: 2026-10-18
title: Lesson 0 - Trial 🚀 Setup, First Program & Python's 6 Big Topics
subtitle: From zero setup to "Hello, ML world!" in one session
course: python-to-machine-learning
topics:
  - Learning roadmap
  - VS Code + Python setup
  - GitHub sign-up + first repo
  - .py vs .ipynb
  - Python's 6 main topics (quick recap)
platform: preply
lesson: 0 (trial)
---

Salam Awais! 👋 Welcome to **Lesson 0**, your launchpad. Today we don't just talk about machine learning. We **set up the rocket** 🚀 so every lesson after this is pure building.

:::aside title="🎯 MAIN learning goal (set when you joined)" color="indigo"
**Learn machine learning from the basics**, and level up your Python from *intermediate* to *advanced*, with NumPy, Pandas, GitHub and real projects along the way.
:::

:::aside title="🧩 SUB goal for today (Lesson 0)" color="green"
Have a **working setup** (VS Code + Python + GitHub), run your **first program** in both a `.py` file and a notebook, and do a **quick recap** of Python's 6 big topics.
:::

## 🗺️ Your roadmap: Python → Machine Learning

Here's the plan we'll follow. The phases are short, sharp and project-heavy. 💪

:::journey
- Lesson 0 🛠️ | Setup + Recap | VS Code, GitHub, first program | now
- Lessons 1–2 🔢 | NumPy | Arrays, maths at lightning speed
- Lessons 3–7 🐼 | Pandas | Clean, filter, group, merge real data
- Lessons 8–9 📈 | Matplotlib + Seaborn | Make data tell a story
- Lessons 10–16 🤖 | Machine Learning | Supervised + Unsupervised
- Lessons 17+ 🏆 | 3 Mini Projects | Recommender, predictor & more
:::

:::mermaid caption="The ML family tree we'll climb 🌳"
flowchart TD
    ML[🤖 Machine Learning] --> S[🎓 Supervised<br/>has answers / labels]
    ML --> U[🔍 Unsupervised<br/>no labels]
    S --> R[📈 Regression<br/>predict a number]
    S --> C[🏷️ Classification<br/>predict a category]
    U --> K[🫧 Clustering<br/>find groups]
    U --> D[🗜️ Dimensionality Reduction<br/>shrink data smartly]
:::

:::task id=q1 type=choice
❓ Predicting **tomorrow's temperature** (a number) is which kind of ML?

OPTIONS
- Clustering — Clustering finds groups. It doesn't predict numbers.
- Classification — That predicts categories like "hot / cold".
- [x] Regression — Yes! 📈 A number output means regression.
- Dimensionality reduction — That shrinks data. It doesn't predict anything.
:::

## 🛠️ Step 1: Install Python + VS Code

:::task id=t1 type=step
Install Python 3 🐍

NOTE
1. Go to **python.org → Downloads** and get the latest Python 3.
2. ⚠️ On Windows, **tick "Add python.exe to PATH"** before clicking Install!
3. Open a terminal (Command Prompt) and type:

```bash
python --version
```

DONE WHEN
You see something like `Python 3.12.x` (any 3.x is fine ✅).

SOLUTION
If you get "not recognized", re-run the installer, choose **Modify**, and make sure **Add to PATH** is ticked. Then close and reopen the terminal.
:::

:::task id=t2 type=step
Install VS Code + 2 extensions 💻

NOTE
1. Download **Visual Studio Code** from code.visualstudio.com.
2. Open it, click the **Extensions** icon (4 squares 🧩) on the left.
3. Install **Python** (by Microsoft) and **Jupyter** (by Microsoft).

DONE WHEN
Both extensions show **Installed** ✅.

SOLUTION
Search exactly "Python" and pick the one by **Microsoft** with millions of downloads, then do the same for "Jupyter".
:::

## 🐙 Step 2: GitHub, your coding portfolio

GitHub is like **Google Drive for code**, plus a **time machine** ⏳ that remembers every version. Recruiters look at it too! 👀

:::mermaid caption="How Git moves your code 🚚"
flowchart LR
    A[📝 Your files] -->|git add| B[📦 Staging box]
    B -->|git commit| C[💾 Local history]
    C -->|git push| D[☁️ GitHub online]
:::

:::task id=t3 type=step
Create your GitHub account + first repo 🎉

NOTE
1. Sign up at **github.com** (pick a professional username, e.g. `awais-ml`).
2. Click **New repository** → name it `python-to-ml`.
3. Tick **Add a README file** → **Create repository**.

DONE WHEN
You see your new repo page with a `README.md` in it.

SOLUTION
If the green **New** button is hidden, click your profile picture (top right) → **Your repositories** → **New**.
:::

:::card title="🧰 Git commands cheat sheet (we'll practise these over the course)"
| command | what it does |
|---|---|
| `git clone <url>` | download a repo to your computer |
| `git status` | "what changed?" 🔍 |
| `git add .` | put all changes in the staging box 📦 |
| `git commit -m "msg"` | save a snapshot with a note 💾 |
| `git push` | upload to GitHub ☁️ |
:::

:::task id=q2 type=choice
❓ Which command **uploads** your saved commits to GitHub?

OPTIONS
- `git add .` — That only stages changes locally.
- `git commit` — That saves locally. It's not online yet.
- `git status` — That only shows what changed.
- [x] `git push` — Correct! ☁️ Push = send to GitHub.
:::

## 📄 Step 3: `.py` file vs `.ipynb` notebook

:::grid
📄 .py FILE
▶️ Runs top to bottom, all at once
🏗️ Best for real apps & scripts
🐙 Clean on GitHub
---
📓 .ipynb NOTEBOOK
🧱 Runs in small cells, one by one
📊 Shows tables & charts inline
🤖 Best for data science & ML experiments
:::

:::task id=t4 type=code
Your first program in a `.py` file 🐍

NOTE
Create a folder `python-to-ml`, open it in VS Code (**File → Open Folder**), make a new file `hello.py` and type:

```python
name = "Awais"
goal = "Machine Learning"
print(f"Hello, {name}! 🚀 Welcome to {goal}.")
```

Click ▶️ **Run** (top right).

DONE WHEN
The terminal prints: `Hello, Awais! 🚀 Welcome to Machine Learning.`

SOLUTION
If ▶️ is missing, press **Ctrl+Shift+P** → "Python: Select Interpreter" → pick your Python 3.
:::

:::task id=t5 type=code
Same thing in a notebook 📓

NOTE
Create `hello.ipynb`. In cell 1 type the first two lines below, then run it with **Shift+Enter**. In cell 2 type the last line and run it.

```python
name = "Awais"
goal = "Machine Learning"
```

```python
print(f"{name} is starting {goal} today! 🎯")
```

DONE WHEN
Cell 2 prints: `Awais is starting Machine Learning today! 🎯`

SOLUTION
If VS Code asks for a **kernel**, choose your Python 3. If it asks to install `ipykernel`, click **Install**.
:::

:::task id=q3 type=choice
❓ In a notebook you run **cell 2 before cell 1**. What happens?

OPTIONS
- [x] NameError — Yes! `name` doesn't exist until cell 1 runs. 🧠 Notebook order matters!
- It works fine — No. Cell 1 hasn't created the variables yet.
- It prints blank — Python errors instead of printing nothing.
- VS Code crashes — No crash, just an error message.
:::

:::task id=q4 type=choice
❓ You're **exploring a dataset and drawing charts**. Best choice?

OPTIONS
- `.txt` file — That's not runnable Python.
- `.py` file — Possible, but charts won't show inline.
- [x] `.ipynb` notebook — Yes! 📊 Cells + inline charts = data heaven.
- `.md` file — That's for notes, not code.
:::

## 🎯 Python's 6 big topics: the quick recap

:::mermaid caption="The 6 building blocks of every Python program 🧱"
flowchart LR
    A[1️⃣ Data Types] --> B[2️⃣ Data Structures]
    B --> C[3️⃣ if / else]
    C --> D[4️⃣ Loops]
    D --> E[5️⃣ Functions]
    E --> F[6️⃣ Classes]
:::

### 1️⃣ Data types: what *kind* of value?

:::example
```python
age = 24            # int   🔢
height = 5.9        # float 📏
city = "Gujrat"     # str   🔤
is_student = True   # bool  ✅

print(type(age), type(height), type(city), type(is_student))
```
:::

:::task id=q5 type=choice
❓ Run it. What does `type(height)` print?

OPTIONS
- `<class 'int'>` — 5.9 has a decimal, so not int.
- `<class 'str'>` — No quotes, so not a string.
- [x] `<class 'float'>` — Yes! 📏 Decimal = float.
- `<class 'bool'>` — Bools are only True/False.
:::

### 2️⃣ Data structures: boxes that hold many values

:::example
```python
scores = [88, 92, 75]                  # list  📋 changeable
point = (3, 4)                         # tuple 🔒 fixed
student = {"name": "Awais", "lvl": 2}  # dict  📖 key → value
tags = {"ml", "python", "ml"}          # set   🎯 no duplicates

scores.append(99)
print(scores)
print(student["name"])
print(len(tags))
```
:::

:::task id=q6 type=choice
❓ Run it. What does `len(tags)` print?

OPTIONS
- 3 — The duplicate "ml" was removed, so not 3.
- 1 — There are two different words in the set.
- 0 — The set isn't empty.
- [x] 2 — Yes! 🎯 Sets drop the duplicate "ml".
:::

:::task id=q7 type=choice
❓ In ML, a **row of data** like `{"age": 24, "city": "Gujrat"}` is best stored as a…

OPTIONS
- tuple — Tuples have no names for each value.
- [x] dict — Yes! 📖 Column name → value, just like a Pandas row.
- set — Sets have no keys and no order.
- int — An int holds only one number.
:::

### 3️⃣ if / else: making decisions 🚦

:::example
```python
accuracy = 0.87

if accuracy >= 0.9:
    print("🏆 Excellent model!")
elif accuracy >= 0.8:
    print("👍 Good model")
else:
    print("🔧 Needs tuning")
```
:::

:::task id=q8 type=choice
❓ Run it. What prints?

OPTIONS
- 🏆 Excellent model! — 0.87 is less than 0.9.
- 🔧 Needs tuning — The `elif` catches it first.
- [x] 👍 Good model — Yes! 0.87 ≥ 0.8 ✅
- Nothing — One branch always runs here.
:::

### 4️⃣ Loops: repeat without copy-pasting 🔁

:::example
```python
# for loop: go through every item
losses = [0.9, 0.6, 0.4, 0.2]
for epoch, loss in enumerate(losses, start=1):
    print(f"Epoch {epoch}: loss = {loss}")

# while loop: repeat until a condition is false
battery = 3
while battery > 0:
    print("🔋" * battery)
    battery -= 1
```
:::

:::task id=q9 type=choice
❓ Run it. What is the **last** line printed?

OPTIONS
- `Epoch 4: loss = 0.2` — The while loop runs after the for loop.
- `🔋🔋🔋` — That's the first battery line.
- [x] `🔋` — Yes! battery goes 3 → 2 → 1, then stops at 0.
- An empty line — When battery hits 0, the loop just stops.
:::

:::task id=q10 type=choice
❓ Spot the bug 🐛 Which line makes this loop run **forever**?

```python
n = 5
while n > 0:
    print(n)
n -= 1
```

OPTIONS
- `n = 5` — Starting value is fine.
- `print(n)` — Printing doesn't cause a loop.
- `while n > 0:` — The condition is fine.
- [x] `n -= 1` — Yes! It's not indented, so it's outside the loop. 😱
:::

### 5️⃣ Functions: reusable mini-machines ⚙️

:::example
```python
def mean(numbers):
    return sum(numbers) / len(numbers)

marks = [80, 90, 70]
avg = mean(marks)
print(f"Average = {avg}")
```
:::

:::tip
💡 Prefer **`return`** over `print` inside functions. `return` hands the value back so you can **use** it later. `print` just shows it and it's gone. ML code is all about passing values around!
:::

:::task id=q11 type=choice
❓ Run it. What prints?

OPTIONS
- `Average = 80` — Close! But `/` always gives a float.
- [x] `Average = 80.0` — Yes! ⚙️ `/` returns a float.
- `Average = 240` — That's the sum, not the mean.
- `Average = None` — It would only be None without `return`.
:::

### 6️⃣ Classes: blueprints for your own objects 🏗️

:::example
```python
class Model:
    def __init__(self, name):
        self.name = name
        self.trained = False

    def train(self):
        self.trained = True
        return f"{self.name} trained ✅"

m = Model("HousePricePredictor")
print(m.train())
print(m.trained)
```
:::

:::aside title="🧠 Why classes matter for ML" color="teal"
scikit-learn models **are** classes! Soon you'll write `model = LinearRegression()` then `model.fit(X, y)`. That's exactly the pattern above: create an object, then call its method. 🤯
:::

:::task id=q12 type=choice
❓ Run it. What does the **second** print show?

OPTIONS
- `False` — `train()` changed it before this print.
- `None` — `trained` was set to a bool.
- [x] `True` — Yes! `train()` flipped it. ✅
- An error — The attribute exists, so no error.
:::

## 💪 Mini challenge: put all 6 together

:::practice id=p1
Write a program in `challenge.py` that:
1. Stores 4 student scores in a **list**
2. Has a **function** `grade(score)` that **returns** "A" (≥90), "B" (≥75) or "C"
3. **Loops** through the scores and prints each score with its grade

Use the scores `[95, 80, 60, 77]`.

EXPECTED
95 → A
80 → B
60 → C
77 → B

SOLUTION
```python
def grade(score):
    if score >= 90:
        return "A"
    elif score >= 75:
        return "B"
    else:
        return "C"

scores = [95, 80, 60, 77]
for s in scores:
    print(f"{s} → {grade(s)}")
```
:::

:::task id=t6 type=step
Push your work to GitHub 🐙☁️

NOTE
In the VS Code terminal, inside your project folder:

```bash
git init
git add .
git commit -m "Lesson 0: setup + first programs 🚀"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/python-to-ml.git
git pull origin main --allow-unrelated-histories
git push -u origin main
```

DONE WHEN
Refresh your GitHub repo page and see `hello.py`, `hello.ipynb` and `challenge.py`. 🎉

SOLUTION
If Git asks "who are you?", run `git config --global user.name "Awais"` and `git config --global user.email "you@email.com"`, then commit again. If the pull opens an editor, just save and close it.
:::

## ✅ What we covered today

:::steps
1. Made our **roadmap** from Python to Machine Learning 🗺️
2. Installed **Python + VS Code** + extensions 🛠️
3. Created a **GitHub** account and first repo 🐙
4. Ran code in a **`.py` file** and a **`.ipynb` notebook** 📄📓
5. Recapped Python's **6 big topics** 🧱
6. Pushed everything to GitHub ☁️
:::

:::checklist
- Python installed and `python --version` works
- VS Code has the Python + Jupyter extensions
- GitHub repo `python-to-ml` created
- hello.py and hello.ipynb run
- Mini challenge solved
:::

## 🎁 Did you know?

:::push title="Did you know you can build a mini AI in just 6 lines? 🤯"
With **scikit-learn** you can train a model that predicts a house price from its size. Try it after `pip install scikit-learn`:

```python
from sklearn.linear_model import LinearRegression

sizes = [[500], [1000], [1500], [2000]]   # square feet
prices = [50, 100, 150, 200]               # in thousands
model = LinearRegression().fit(sizes, prices)
print(model.predict([[1200]]))             # → [120.]
```

That's **supervised regression**, and it's exactly where we're heading! 🚀 Next stop: **NumPy** 🔢
:::
