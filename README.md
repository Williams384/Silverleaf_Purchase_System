# SilverLeaf Academy - Purchase Pipeline System

A professional, role-based web application designed to streamline the procurement process for SilverLeaf Academy. This system manages the lifecycle of a purchase request from initial creation to final execution, ensuring financial accountability and operational clarity.

##  Live Demo
**URL:** [INSERT YOUR VERCEL LINK HERE]

---

## 🛠 Features

### 1. Secure Role-Based Access Control (RBAC)
The system identifies users by unique IDs and tailors the interface to their specific organizational responsibilities:
* **Requesters (Alice - U1, Bob - U2):** Create new purchase requests with titles, descriptions, and amounts. Track live status of submissions.
* **Approver (Carol - U3):** A management view focused on "Inbox Zero." Carol sees only pending requests and has the authority to **Approve** or **Reject** them.
* **Executor (Dave - U4):** An operations view that displays only **Approved** items ready for procurement. Dave marks items as **Completed** once fulfilled.

### 2. Intelligent Financial Logic
* **Dynamic Total Spend:** Calculates expenditure in real-time. It intelligently ignores **Pending** and **Rejected** requests, ensuring the "Total Spend" card reflects only authorized school expenses.
* **Tanzanian Shilling (Tshs) Integration:** All financial data is automatically formatted with the `Tshs` prefix and standard comma grouping.

### 3. Optimized User Experience (UX)
* **Contextual Headers:** Dashboard titles change dynamically (e.g., "Approve Requests" for Carol vs. "Execute Requests" for Dave).
* **Clean Interface:** Full-width table layout for maximum readability after removing unnecessary sidebars.
* **Persistent Storage:** Utilizes `localStorage` to maintain data consistency across sessions without a complex backend.

---

## Test Credentials

To test the full pipeline, please use the following User IDs:

| Name  | Role      | User ID | Responsibility                   |
| :---  | :---      | :---    | :---                             |
| Alice | Requester | `U1`    | Create and track requests        |
| Bob   | Requester | `U2`    | Create and track requests        |
| Carol | Approver  | `U3`    | Authorize or Deny pending items  |
| Dave  | Executor  | `U4`    | Finalize approved purchases      |

---

##  Technology Stack
* **HTML5 & CSS3:** Semantic structure and custom styling.
* **Tailwind CSS:** For a modern, responsive, and professional UI.
* **Vanilla JavaScript (ES6+):** For state management and role-based filtering.
* **Vercel:** Cloud hosting and deployment.

---

##  How to Run Locally
1. Download the project folder.
2. Ensure the main file is named `index.html`.
3. Open `index.html` in any modern web browser.
4. Use the credentials above to navigate the different roles.

---

##  Project History
This system was developed as a solution for the SilverLeaf Academy technical assessment. It focuses on solving real-world procurement bottlenecks through a clean, automated digital pipeline.
