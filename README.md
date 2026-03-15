 # 🚀 ApproveFlow: Enterprise Workflow Automation

A state-of-the-art, role-based hierarchical approval and workflow automation system. Built with modern web technologies, it streamlines corporate request routing with configurable Service Level Agreements (SLAs), auto-escalation matrices, and a premium Dark UI.

## ✨ Key Features

- **Dynamic Role-Based Access Control (RBAC):** Distinct dashboards and secure authentication for Employees, Team Leaders, Accountants, CFOs, and Managing Directors.
- **Auto-Escalation & SLA Timers:** Configurable countdown SLAs for every role. If an approver misses the deadline, the request automatically jumps to the next higher authority in the hierarchy.
- **Emergency Override Routing:** Critical requests bypass standard protocols and are routed directly to the top-level management (e.g., Managing Director) with neon-red highlighted priority.
- **Smart Form Filtering:** Conditional rendering logic that dynamically hides/shows budget fields based on the selected category (e.g., Leave Approvals vs. Financial Approvals).
- **Super Admin Portal:** A master admin access portal (SVHEC) to oversee user registrations, manage the pending queue, and monitor system-wide approvals.
- **Premium UI/UX:** 3D tilt interactive cards, responsive glassmorphism modals, embedded inline login states, and sleek dark-mode aesthetics.

## 🛠️ Tech Stack

- **Frontend:** React.js, TypeScript
- **Styling:** Tailwind CSS (Custom Glassmorphism & Neon Glow effects)
- **Icons:** Lucide React
- **State Management & Persistence:** React Hooks, Browser LocalStorage API (No backend required for preview)

## ⚙️ How It Works (Workflow Logic)

1. **User Registration:** New users register and are placed in a `Pending` state.
2. **Admin Approval:** The Super Admin (`svhec`) logs in and approves/rejects new user accounts.
3. **Request Creation:** Employees submit requests with specific categories and urgency levels.
4. **Smart Routing:** The system auto-assigns the request to the correct authority (e.g., requests > ₹50,000 go to the CFO).
5. **SLA Escalation:** If the assigned authority fails to act within the configured time frame (e.g., 24 hours), the request escalates up the chain.

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) installed on your machine.

### Installation & Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/approve-flow.git](https://github.com/yourusername/approve-flow.git)
Navigate into the project directory:

Bash
cd approve-flow
Install all dependencies:

Bash
npm install
Start the local development server:

Bash
npm run dev
Open your browser and visit: http://localhost:5173
