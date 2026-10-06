# Activity 12 — Prompt Engineering & Refinement Log

**Course:** Portfolio Building (B25CS0311)  
**Student Name:** ABHISHEK MAURYA  
**SRN:** R25EJ004  
**Batch / Branch:** 3rd Semester B.Tech CSIT, REVA University  
**Live Site URL:** [https://kudokode.github.io](https://kudokode.github.io)  

---

## 1. Initial Generation Prompt (Step 2)

```text
Act as a senior frontend UI designer and engineer. Build a complete, responsive, modern single-page developer portfolio blog in a self-contained index.html file with embedded CSS.

Student Details:
- Name: Abhishek Maurya (SRN: R25EJ004)
- Degree: 3rd Semester B.Tech in Computer Science & Information Technology, REVA University
- Role/Focus: Systems Software, C/C++ Programming, and Algorithmic Problem Solving
- GitHub: https://github.com/KudoKode
- HackerRank: https://www.hackerrank.com/profile/KudoKode (3-Star Badge)

Design & Layout Requirements:
1. Theme: Modern dark-slate aesthetic (Deep navy #0b1120, slate cards #151f32, cyan accent #38bdf8, high-contrast typography).
2. Navigation: Sticky navigation with backdrop blur effect and anchor links.
3. Hero Section: Name, SRN badge, clear two-line elevator pitch, GitHub/HackerRank call-to-action buttons, and a quick statistics counter (Repositories, Line Editor score 100/100, HackerRank 3-Star).
4. Featured Projects:
   - "Simple Line Editor in C" linking to https://github.com/KudoKode/one_line_command_abhishek_maurya
   - "HackerRank Algorithmic Suite" linking to https://github.com/KudoKode/HackerRank-3rdSem-Portfolio
   - "2D Canvas Graphics System in C" linking to https://github.com/KudoKode/Graphics_using_2D_array
   - "LeetCode Practice Suite" linking to https://github.com/KudoKode/leetcode-solutions
5. Skills Section: Categorized badge pills (Languages, Toolchain, Core CS Concepts).
6. Footer: Clean copyright and university affiliation note.

Constraints:
- Single clean index.html file with zero external framework dependencies (pure CSS, no React/Bootstrap).
- Fully responsive on mobile, tablet, and desktop viewports.
```

---

## 2. Iterative Refinement Log (Step 4)

### Refinement 1: Project Card Interactivity & Direct GitHub Links
* **Prompt Submitted:**
  > *"The initial project cards do not emphasize that the projects are live on GitHub. Update the project cards to include clickable 'View Repository' callout links pointing directly to my specific repositories (one_line_command_abhishek_maurya, HackerRank-3rdSem-Portfolio, etc.) and add subtle hover lift transitions."*
* **Before:** Plain informational text cards with generic non-clickable labels.
* **After / Impact:** Each card now has a distinct accent-colored `View Repository →` link that opens the corresponding GitHub project in a new tab, with a smooth `transform: translateY(-4px)` hover elevation and subtle box-shadow.

---

### Refinement 2: Adding Metric Counters & Verified Badges
* **Prompt Submitted:**
  > *"Add a high-level metrics grid right below the hero biography highlighting 4 key quantitative achievements: '5+ Production Repositories', '100/100 Line Editor Project Score', '3-Star Problem Solving Badge', and 'O(1) / O(N) Target Asymptotic Efficiency'. Make the numbers large and highlighted in cyan."*
* **Before:** The hero section transitioned directly into project listings without quick measurable indicators of technical ability.
* **After / Impact:** Introduced a responsive `.stats-grid` element that presents recruiters and evaluators with immediate quantitative proof of coursework performance.

---

### Refinement 3: Mobile Breakpoint & Contrast Optimization
* **Prompt Submitted:**
  > *"Ensure the layout renders cleanly on mobile viewports under 600px without horizontal scroll. Switch the project grid to a single column on mobile, reduce hero title padding slightly, and adjust pill badge spacing."*
* **Before:** Grid columns caused horizontal overflow on smaller screens, and badges wrapped unevenly.
* **After / Impact:** Added `grid-template-columns: repeat(auto-fit, minmax(300px, 1fr))` and flexible padding units, achieving 100% responsive fluid scaling across all device resolutions.

---

## 3. Reflection Note (Step 6)
> The prompt that produced the single biggest improvement was **Refinement 1**, which transformed passive text blocks into an interactive technical portfolio with direct, verified repository links. The main element the AI initial output missed was omitting specific repository URLs and using placeholder `#` anchors; specifying exact GitHub paths in the refinement prompt ensured the portfolio accurately represents my actual engineering artifacts.
