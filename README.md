# 📚 Wren & Martin — Grammar Portal

A complete multi-page web application for Wren & Martin *High School English Grammar & Composition* with Student Login, Admin Dashboard, and all **3187 questions** from HW #63 to HW #329.

---

## 🗂️ Project Structure

```
wren-martin/
├── index.html                  ← Login Page (Student + Admin)
├── exercises/
│   └── student.html            ← Student Exercise Portal
├── admin/
│   └── dashboard.html          ← Admin Dashboard
├── js/
│   ├── shared.js               ← Common JS (auth, toggle, search)
│   ├── exercises_data.js       ← All 3187 Q&A data
│   └── index_data.js           ← Section index for admin
├── css/
│   └── shared.css              ← Common styles
└── README.md
```

---

## 🔐 Login Credentials

### Student Login

| Username | Password  |
|----------|-----------|
| student  | wren123   |
| rahul    | rahul2024 |
| priya    | priya2024 |
| amit     | amit2024  |
| sneha    | sneha2024 |
| rohit    | rohit2024 |

### Admin Login

| Username | Password   |
|----------|------------|
| admin    | admin2024  |
| teacher  | teach2024  |

---

## ✨ Features

### Student Portal
- 🔍 **Full-text search** — search by word, sentence, or HW number
- 📖 **Chapter filter pills** — filter by topic (Subject & Predicate, Nouns, Verbs, etc.)
- 📌 **Jump TOC** — click any HW# to jump instantly
- 👆 **Click to reveal** — show/hide answers per question
- ✅ **Show All / Hide All** per section
- 📈 **Progress bar** — reading progress shown at top
- ⬆️ **Back to top** button

### Admin Dashboard
- 📊 **Overview stats** — total sections, questions, students
- 📋 **All Sections table** — searchable list of all 267 HW sections
- 👥 **Student management** — view registered students
- 📖 **Chapter summary** — question distribution per chapter
- 🔗 **Quick view** — click to open any section in student view

---

## 📊 Content Stats

| Metric | Value |
|--------|-------|
| Total HW Sections | 267 |
| HW Range | #63 – #329 |
| Total Q&A | 3187 |
| Grammar Rules | 3187 |
| Chapters | 12 |

---

## 🚀 How to Run

### Option 1 — Open Locally
Just open `index.html` in any browser. No server needed.

### Option 2 — GitHub Pages
1. Push all files to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Your site will be live at `https://yourusername.github.io/wren-martin/`

### Option 3 — VS Code Live Server
Install the **Live Server** extension and click "Go Live".

---

## 📖 Chapters Covered

| # | Chapter | HW Range |
|---|---------|----------|
| 1 | Subject & Predicate | #63–69 |
| 2 | Parts of Speech | #70–89 |
| 3 | Nouns & Pronouns | #90–119 |
| 4 | Adjectives | #120–139 |
| 5 | Verbs & Tenses | #140–179 |
| 6 | Adverbs | #180–199 |
| 7 | Prepositions | #200–219 |
| 8 | Conjunctions | #220–239 |
| 9 | Sentences & Clauses | #240–269 |
| 10 | Direct & Indirect Speech | #270–289 |
| 11 | Active & Passive Voice | #290–309 |
| 12 | Composition & Essays | #310–329 |

---

## ⚙️ Customization

### Adding Students (in `index.html`)
```js
const USERS = {
  student: {
    'newstudent': 'password123',  // add here
    ...
  }
};
```
Also add the same student to the `STUDENTS` array in `admin/dashboard.html`.

### Adding Admin Users (in `index.html`)
```js
const USERS = {
  admin: {
    'newteacher': 'teachpass',  // add here
  }
};
```

---

*Built for Wren & Martin — High School English Grammar & Composition*
