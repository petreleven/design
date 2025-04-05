
## 🧩 Server Dashboard UI — SPA with Snabbdom

### 🎯 Objective

Create a **Single Page Application (SPA)** using **Snabbdom** and **Tailwind CSS** that lets users manage multiple mock servers. Navigation between **Dashboard** and **Settings** panels should be smooth, dynamic, and handled entirely on the frontend without page reloads.

---

### 📷 Design Breakdown (Based on Your Sketch)

| PAGE      | Design Template                                               | Inspiration Ideas                         |
|-----------|----------------------------------------------------------------|--------------------------------------------|
| **DASHBOARD** | ![Server Cards] When clicked, each card routes to the config panel/settings page . | A grid layout with dark theme cards for inspiration |
| **SETTINGS** | Includes server status, action buttons, and a dynamic form with different input types (text, number, toggle, dropdown). | Mimics clean control panels seen in modern UIs |

---

### ⚙️ Tech Stack

- **Frontend:** [Snabbdom](https://github.com/snabbdom/snabbdom) (Virtual DOM)
- **Styling:** [Tailwind CSS](https://tailwindcss.com/)
- **Routing/State:** Manual handling via Snabbdom + JS (no backend or router library)

---

### 🔄 SPA Behavior

- The **server cards** on the **Dashboard** are clickable.
- Clicking a card **replaces the current view** with the corresponding **Settings page** using Snabbdom patching (no page reload).
- Users can return to the dashboard via a Back or Logout button (SPA logic).

---

### 📐 Component Guidelines

#### 🧭 Dashboard View

- **Clickable Cards:**  
  - Represent servers (e.g., `Mock Server 1`, `Mock Server 2`)
  - Styled as card elements using Tailwind  
  - Highlight on hover, add cursor effect
- **Logout Button:**  
  - Positioned top-right
  - Simulates a logout or navigation back to login (no real auth)

#### 🛠 Settings View

- **Status Indicator:**  
  - Shows `online`, `offline`, etc. using color-coded labels
- **Action Buttons:**
  - Start / Stop / Restart / Backup
  - Simulate mock actions (you can show loading state temporarily)
- **Configuration Panel:**
  - **Text Input** – Server name  
  - **Number Input** – Difficulty  
  - **Dropdown** – Mods  
  - **Toggle Switch** – Public/Private  

