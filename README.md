# 🗳️ Personal Election & Voting Tracker

A structured repository to maintain a historical, organized record of election research, ballot proposition analysis, and voting strategy. 

This system cuts through the noise of election season by strictly separating objective ballot data from personal strategy. It scales to act as a definitive voting dashboard for my own ballots, while providing a cleanly isolated framework for analyzing and generating tailored recommendations for friends, family, and network requests across any jurisdiction.

---

## 🗂️ Structure

To prevent data overlap (e.g., mixing up candidates from different congressional districts or county lines), the repository is strictly isolated by **Date, Election Type, State-City, and Intent**. 

* `_Personal`: My actual, legal voting jurisdiction. This is the only place a `vote.md` file lives.
* `_Analysis`: Research conducted for external districts. Used to generate shareable guides.

```text
election-tracker/
├── README.md                                         # This file (Repository overview & instructions)
└── 2026/
    ├── 06-02-2026_Primary_CA-Irvine_Personal/        # MY LEGAL BALLOT
    │   ├── election.md                               # Unbiased overview of my ballot
    │   ├── candidates.md                             # Research on candidates in my district
    │   ├── propositions.md                           # Pros/cons for state and Irvine measures
    │   ├── reasoning.md                              # [OPTIONAL] Complex ideological balancing
    │   ├── vote.md                                   # My final personal decisions (Source of Truth)
    │   └── recommendations/                          # [OPTIONAL] Export for my household
    │       └── vote_recommendation_jocelyn.md        # Tailored summary of our household's plan
    │
    ├── 06-02-2026_Primary_CA-LaMirada_Analysis/      # EXTERNAL NETWORK REQUEST
    │   ├── election.md                               # Overview of the La Mirada/LA County ballot
    │   ├── candidates.md                             # Candidates strictly for this specific district
    │   └── recommendations/                          
    │       └── vote_recommendation_brother.md        # Specific picks & rationale tailored to his ballot
    │
    ├── 06-02-2026_Primary_CA-Bellflower_Analysis/    # EXTERNAL NETWORK REQUEST
    │   ├── election.md                               
    │   ├── candidates.md                             
    │   └── recommendations/                          
    │       └── vote_recommendation_colleague.md      # Specific picks & rationale for a Bellflower voter
    │
    ├── 11-03-2026_General_CA-Irvine_Personal/        # MY LEGAL BALLOT
    │   ├── election.md                               
    │   ├── candidates.md                             
    │   ├── propositions.md                           
    │   ├── vote.md                                   
    │   └── recommendations/                          
    │       └── vote_recommendation_jocelyn.md        
    │
    └── 11-03-2026_General_TX-Austin_Analysis/        # OUT-OF-STATE NETWORK REQUEST
        ├── election.md                               
        ├── candidates.md                             
        └── recommendations/                          
            └── vote_recommendation_friend.md         
```

---

## 📄 Core Files Explained

For every election directory, the workflow utilizes distinct documents to establish a clean separation of concerns and ensure data portability.

### 1. `election.md` (The Dashboard)
An objective, high-level overview of exactly what is on that specific ballot. 
* **Contains:** Key election deadlines, a list of all offices up for election, and a summary of propositions. 
* **Purpose:** Acts as the landing page for that exact geographic cycle.

### 2. `candidates.md` (The Data)
The research scratchpad for individuals running for office.
* **Contains:** Tables listing candidates, party affiliations, professional backgrounds, and links to platforms.
* **Purpose:** To compile objective data without cluttering final decisions. 

### 3. `propositions.md` (The Policy Breakdown)
The research scratchpad for state and local measures.
* **Contains:** Title, summary, fiscal impact, major financial backers, and key endorsements.
* **Purpose:** To decode ballot language and track actual tax or regulatory impacts.

### 4. `vote.md` (The Final Personal Plan)
My personal, final decisions and the strategic reasoning behind them. 
* **Crucial Note:** This file is strictly for `_Personal` directories. It is NEVER included in `_Analysis` folders.
* **Contains:** The specific candidate or measure I am voting for, alongside a concise ideological rationale. 
* **Purpose:** This is the document I use to fill out my official mail-in or in-person ballot.

### 5. `reasoning.md` (Optional: The Deep Logic)
An overflow document for highly complex decisions.
* **Contains:** Long-form thoughts, multi-step strategic logic (e.g., jungle primary vote-splitting), or extensive financial modeling.
* **Purpose:** To keep `vote.md` clean and scannable. 

### 6. `recommendations/vote_recommendation_*.md` (The Shareable Exports)
A dedicated directory holding clean, sanitized summaries designed to be shared.
* **Contains:** Individual markdown files tailored to a specific person or demographic. Features top-level picks, brief rationales, and coordination instructions.
* **Purpose:** Allows me to provide customized, isolated guidance based on a requester's exact jurisdiction and political alignment. For `_Analysis` directories, these files act as the ultimate output.

---

## ⚙️ Standard Workflow

1. **Setup:** Create the new `YYYY/MM-DD-YYYY_ElectionType_State-City_Intent/` folder. 
2. **Populate `election.md`:** Pull all offices and propositions from the exact sample ballot for that jurisdiction. 
3. **Research Phase:** Fill in `candidates.md` and `propositions.md`.
4. **Draft Logic:** Use `reasoning.md` to map out difficult decisions.
5. **Lock In Decisions:** * If `_Personal`: Finalize my `vote.md`.
    * If `_Analysis`: Skip directly to step 6.
6. **Generate Exports:** Create targeted `vote_recommendation_[target].md` files inside the `recommendations/` folder to fulfill requests.
7. **Execute:** Cast my personal vote, monitor the results, and archive the directory.
