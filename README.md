# 🗳️ Personal Election & Voting Tracker

A structured repository to maintain a historical, organized record of my election research, ballot proposition analysis, and final voting decisions. 

This system cuts through the noise of election season by separating objective ballot data from personal strategy. By Election Day, this ensures I have a fully researched, philosophically grounded voting plan ready to transfer directly to my official ballot.

---

## 🗂️ Repository Structure

The repository is organized chronologically by year, followed by the exact date and type of the election. 

```text
election-tracker/
├── README.md                           # This file (Repository overview & instructions)
└── 2026/
    ├── 06-02-2026_Primary/             # Folder for the June Primary
    │   ├── election.md                 # Unbiased overview of the ballot and key dates
    │   ├── candidates.md               # Detailed research on federal, state, and county candidates
    │   ├── propositions.md             # Pros, cons, and funding research for state/local measures
    │   ├── reasoning.md                # [OPTIONAL] Long-form logic or complex fiscal analysis 
    │   └── vote.md                     # My final decisions and concise ideological rationale
    │
    └── 11-03-2026_General/             # Folder for the November General Election
        ├── election.md
        ├── candidates.md
        ├── propositions.md
        ├── reasoning.md                # [OPTIONAL]
        └── vote.md
```

---

## 📄 Core Files Explained

For every election folder, the workflow utilizes distinct documents to establish a clean separation of concerns.

### 1. `election.md` (The Dashboard)
An objective, high-level overview of exactly what is on the ballot. 
* **Contains:** Key election deadlines, mail-in dates, a list of all offices up for election, and a summary of the state/local propositions. 
* **Purpose:** Acts as the landing page for that specific election cycle so I know exactly what needs to be researched.

### 2. `candidates.md` (The Data)
The research scratchpad for individuals running for office.
* **Contains:** Tables listing candidates from the sample ballot, party affiliations, professional backgrounds, and links to debates or policy platforms.
* **Purpose:** A place to compile objective data, track challengers vs. incumbents, and monitor endorsements.

### 3. `propositions.md` (The Policy Breakdown)
The research scratchpad for state and local measures.
* **Contains:** Title, summary, fiscal impact, major financial backers, and key endorsements.
* **Purpose:** To decode confusing ballot language and track the actual tax, regulatory, or zoning impacts of each measure.

### 4. `vote.md` (The Final Plan)
My final decisions and the strategic reasoning behind them.
* **Contains:** The specific candidate or measure I am voting for, alongside a concise rationale evaluated through my specific political/ideological lens. 
* **Purpose:** This is the exact document I open when I sit down to bubble in my official mail-in ballot. It serves as the definitive source of truth.

### 5. `reasoning.md` (Optional: The Deep Logic)
An overflow document for highly complex decisions.
* **Contains:** Long-form thoughts, complex ideological balancing (e.g., weighing Libertarian vs. Conservative priorities), or extensive financial modeling for complicated tax propositions.
* **Purpose:** To keep `vote.md` clean and scannable. If a decision requires a multi-paragraph explanation or deep philosophical breakdown, it is written here, and `vote.md` simply links to it.

---

## ⚙️ Standard Workflow

1. **Setup (1-2 Months Out):** When the sample ballot arrives, create the new `year/mm-dd-yyyy_ElectionType/` folder.
2. **Populate `election.md`:** Copy all offices and propositions from the sample ballot into the overview file. 
3. **Research Phase:** Over the following weeks, fill in `candidates.md` and `propositions.md` as information becomes available.
4. **Draft Logic (If Needed):** Use `reasoning.md` to map out difficult decisions, such as strategic vote-splitting in jungle primaries or evaluating multi-layered propositions.
5. **Lock In `vote.md`:** Finalize decisions and document the concise rationale for historical reference. 
6. **Cast Ballot:** Use `vote.md` to fill out the official ballot. Drop it in the mail or at a local drop box.
7. **Post-Election Audit:** Track the ballot online to ensure it was counted, note the final election results, and archive the folder.