# Focus-cue

**An AI-powered behavioral cue to help people navigate web based task with focus**

## Project Overview
**Focus-cue** is a smarter, browser-based application designed to help people notice when their study or work session is breaking down from distraction of unrelated sites. 

Instead of treating all tab switching as bad, focus-cue distinguishes between productive switching, getting stuck, and drifting away. It understands the pattern of a user’s digital activity and detects whether they are focused, distracted, drifting away from their goal, or stuck in a loop.

## What We Are Building

### 1. Chrome Extension
The browser extension acts as the active monitoring and intervention layer. Users start a session by entering a specific study goal (e.g., *"Finish my machine learning homework on gradient descent"*). During the session, the extension tracks:
* Active tab and page title
* Domain/URL
* Dwell time on each tab
* Tab switching frequency
* Return rates to specific pages
* Goal relevance of the current page
* Transitions to social or recreational pages

### 2. Web Dashboard
The dashboard provides a post-session summary and analytics to help students understand their study habits. Key features include:
* Overall focus score for the session
* Breakdown of productive vs. distracting tabs
* Timestamps of when drifting started
* Frequency of "stuck loops"
* Time taken to return to work after an interruption
* Common distraction patterns and future session suggestions

## Data & Privacy
For the initial version, the system tracks simple, privacy-friendly data without permanently storing sensitive browsing content:
* Timestamp
* Tab title and domain
* Active duration
* Tab category and transition from the previous tab
* Goal relevance score
* Detected focus state
* Intervention shown and user compliance

## Example User Flow
1. User opens the extension.
2. User enters a specific goal: *"Finish CS homework problem 3."*
3. User begins studying.
4. The extension silently tracks browser activity.
5. The system classifies tabs and checks goal relevance in real-time.
6. A pattern is detected: `assignment -> ChatGPT -> Google -> YouTube -> assignment -> ChatGPT`.
7. AI predicts the user is entering a focus breakdown (Stuck Loop / Goal Drift).
8. A tailored reminder or recovery suggestion is displayed.
9. Upon completion, the dashboard provides a session summary.

## Expected Deliverables
* Fully functional Chrome extension
* Interactive web dashboard
* Trained AI models for tab classification and focus-state prediction
* Algorithmic system for detecting goal drift, stuck loops, and recovery failures
* Engine for context-aware reminders
* Small proprietary dataset of student study sessions
* Academic research paper based on system design and evaluation

## Relevant Literature & Supporting Research

| Paper Topic & Focus | Use Case for focus-cue | Link |
| :--- | :--- | :--- |
| **Task Interruption in Software Dev** | Proves task switching/self-interruption hurts complex work. | [arXiv: 1805.05508](https://arxiv.org/abs/1805.05508) |
| **Perceptions of Task Switching** | Shows task switching breaks flow and creates a cognitive cost. | [arXiv: 1805.05504](https://arxiv.org/abs/1805.05504) |
| **The Hidden Cost of Window Management** | Provides metrics on the measurable time cost of switching tasks. | [arXiv: 1810.04673](https://arxiv.org/abs/1810.04673) |
| **Multitasking Across Industry Projects** | Highlights how context switching affects real-world productivity. | [arXiv: 2006.12636](https://arxiv.org/abs/2006.12636) |
| **Attention Management Systems** | Background on attention fragmentation and sensing/ML systems. | [arXiv: 1806.06771](https://arxiv.org/abs/1806.06771) |
| **Productivity Social Robot Design** | SMART Lab alignment, app-switching behavior, student support. | [arXiv: 2512.01111](https://arxiv.org/abs/2512.01111) |
| **Social Robot Coaching for Productivity** | AI productivity coaching, dashboards, and personalized support. | [arXiv: 2512.01105](https://arxiv.org/abs/2512.01105) |
| **Robot Schoolwork Companion (ADHD)** | Attention monitoring and study companion systems for students. | [arXiv: 2401.06289](https://arxiv.org/abs/2401.06289) |
| **Student Programming Behavior** | Distraction and interruption behaviors during study sessions. | [arXiv: 2605.22657](https://arxiv.org/pdf/2605.22657) |
| **Attention Residue** (Leroy) | Vital research on the challenge of switching between work tasks. | [Princeton Open Pub](https://openpublishing.princeton.edu/read/work/section/ceb4b36c-63de-443c-bf03-dd3200065945) |
| **Cyberslacking & Procrastination** | Insight into digital procrastination habits. | [SAGE Journals](https://journals.sagepub.com/doi/full/10.1177/2050157921993896) |
| **Task Selection & Multitasking** | Detecting multitasking work and negative routines from logs. | [AJET / Scholar Archive](https://scholar.archive.org/search?q=Detecting+Multitasking+Work+and+Negative+Routines+from+Computer+Logs) |
| **Digital Distractions in Education** | Review of causes, consequences, and prevention strategies. | [Journal Article](https://ejournal-nawalaedu.com/index.php/JOP/article/view/2642) |