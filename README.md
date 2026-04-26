# 🗳️ Personal Election & Voting Tracker

A structured repository to maintain a historical, organized record of election research, ballot proposition analysis, and voting strategy. 

This system cuts through the noise of election season by strictly separating objective ballot data from personal strategy. It scales to act as a definitive voting dashboard for my own ballots, while providing a cleanly isolated framework for analyzing and generating tailored recommendations for friends, family, and network requests across any jurisdiction.

---

## 🗂️ Structure

To prevent data overlap and streamline administration, the repository is grouped first by **Election Date**, and then strictly isolated by **Jurisdiction and Intent**. 

* `_Personal`: My actual, legal voting jurisdiction. This is the only place a `vote.md` file lives.
* `_Analysis`: Research conducted for external districts. Used to generate shareable guides.

By removing unnecessary subfolders, all relevant data and final outputs for a specific location are kept in a single, flat directory.

```text
election-tracker/
├── README.md                                     # This file (Overview & instructions)
└── 2026/
    ├── 06-02-2026_Primary/                       # Grouped by Election Date
    │   ├── CA-Irvine_Personal/                   # MY LEGAL BALLOT
    │   │   ├── election.md                       # Unbiased overview of my ballot
    │   │   ├── candidates.md                     # Research on candidates in my district
    │   │   ├── propositions.md                   # Pros/cons for state and local measures
    │   │   ├── reasoning.md                      # [OPTIONAL] Complex ideological balancing
    │   │   ├── vote.md                           # My final personal decisions (Source of Truth)
    │   │   └── vote_recommendation_jocelyn.md    # [OPTIONAL] Tailored summary for our household
    │   │
    │   ├── CA-LaMirada_Analysis/                 # EXTERNAL NETWORK REQUEST
    │   │   ├── election.md                       # Overview of the La Mirada/LA County ballot
    │   │   ├── candidates.md                     # Candidates strictly for this specific district
    │   │   └── vote_recommendation_brother.md    # Specific picks & rationale tailored to his ballot
    │   │
    │   └── CA-Bellflower_Analysis/               # EXTERNAL NETWORK REQUEST
    │       ├── election.md                       
    │       ├── candidates.md                     
    │       └── vote_recommendation_colleague.md  # Specific picks & rationale for a Bellflower voter
    │
    └── 11-03-2026_General/                       # Grouped by Election Date
        ├── CA-Irvine_Personal/                   # MY LEGAL BALLOT
        │   ├── election.md                       
        │   ├── candidates.md                     
        │   ├── propositions.md                   
        │   ├── vote.md                           
        │   └── vote_recommendation_jocelyn.md    
        │
        └── TX-Austin_Analysis/                   # OUT-OF-STATE NETWORK REQUEST
            ├── election.md                       
            ├── candidates.md                     
            └── vote_recommendation_friend.md     # Tailored picks for a Texas voter
```

---

## 📄 Core Files Explained

For every specific jurisdiction directory, the workflow utilizes distinct documents to establish a clean separation of concerns and ensure data portability.

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

### 6. `vote_recommendation_[target].md` (The Shareable Exports)
Clean, sanitized summaries designed to be shared, living directly in the jurisdiction folder.
* **Contains:** A markdown file tailored to a specific person or demographic. Features top-level picks, brief rationales, and coordination instructions.
* **Purpose:** Allows me to provide customized, isolated guidance based on a requester's exact jurisdiction and political alignment. For `_Analysis` directories, these files act as the ultimate output.

---

## ⚙️ Standard Workflow

1. **Setup:** Create the `YYYY/MM-DD-YYYY_ElectionType/` master folder, then build the `State-City_Intent/` subfolders as needed.
2. **Populate `election.md`:** Pull all offices and propositions from the exact sample ballot for that jurisdiction. 
3. **Research Phase:** Fill in `candidates.md` and `propositions.md` within that jurisdiction's folder.
4. **Draft Logic:** Use `reasoning.md` to map out difficult decisions if necessary.
5. **Lock In Decisions:** * If `_Personal`: Finalize my `vote.md`.
    * If `_Analysis`: Skip directly to step 6.
6. **Generate Exports:** Create targeted `vote_recommendation_[target].md` files to fulfill network requests or provide household guides.
7. **Execute:** Cast my personal vote, monitor the results, and archive the directory.
