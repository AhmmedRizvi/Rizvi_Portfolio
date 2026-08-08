# Rizvi Ahmmed — Portfolio Source & Configuration Reference

This file serves as the **Single Source of Truth** for all content, configurations, and deployment steps used in your developer portfolio. If you ever need to restore, recreate, or update your site, all the necessary information is compiled here.

---

## 1. Personal & Contact Details
* **Name**: Rizvi Ahmmed
* **Primary Title**: Full-Stack Developer & AI/ML Enthusiast
* **Status**: Computer Science & Engineering (CSE) Student (Expected Graduation: 2027)
* **Core Bio (Hero)**:
  > *Full-stack developer with real e-commerce experience, now exploring AI/ML and intelligent systems.*
* **SEO Metadata Description**:
  > *Rizvi Ahmmed — Full-Stack Developer & AI/ML Enthusiast. CSE student building full-stack and AI-powered applications while exploring Machine Learning.*
* **GitHub Profile**: [https://github.com/AhmmedRizvi](https://github.com/AhmmedRizvi)
* **LinkedIn Profile**: [https://www.linkedin.com/in/ahmmedrizvi/](https://www.linkedin.com/in/ahmmedrizvi/)
* **Contact Email**: [ahmmed.rizvi30@gmail.com](mailto:ahmmed.rizvi30@gmail.com)
* **Canonical URL**: `https://ahmmedrizvi.github.io/`

---

## 2. Technical Stack (Toolbox)
These are the technologies loaded dynamically under the **Toolbox** section on the website:

* **Frontend**:
  * HTML5 (Intermediate)
  * CSS3 (Intermediate)
  * JavaScript ES6+ (Working Knowledge)
  * Tailwind CSS (Working Knowledge)
  * React.js (Familiar)
  * Vite (Familiar)
* **Backend**:
  * C# (Working Knowledge)
  * ASP.NET Core (Working Knowledge)
  * Python (Intermediate)
  * PHP (Intermediate)
* **Database**:
  * MySQL (Intermediate)
* **Programming**:
  * C (Working Knowledge)
  * C++ (Working Knowledge)
* **Tools**:
  * Git (Intermediate)
  * GitHub (Intermediate)
  * VS Code (Intermediate)
  * Docker (Working Knowledge)
  * Linux (Working Knowledge)
  * XAMPP (Intermediate)
  * phpMyAdmin (Intermediate)
* **AI / Cloud**:
  * Ollama (Working Knowledge)
  * Google AI Studio (Learning)
  * Azure AI Vision (Learning)
  * Azure AI Search (Learning)
  * Azure OpenAI (Learning)

---

## 3. Experience Details
* **Role**: Full-Stack Developer
* **Organization**: Freelance & Independent Projects
* **Period**: 2021 — Present
* **Core Responsibilities**:
  * Designed and developed customized e-commerce platforms and web applications.
  * Built robust backend systems using Django, PHP, and ASP.NET Core, and relational databases (MySQL/SQLite).
  * Created AI-powered assistant tools integrating locally-hosted LLMs using Python and Ollama.
  * Deployed and maintained secure web applications ensuring uptime, clean API structure, and responsive design.
  * Configured database architectures with proper normalization and optimized query performance.

---

## 4. Development Journey Timeline
* **2021**: Began building web applications
* **2025**: Focus shifted toward software engineering
* **2025+**: Full-stack development & AI-powered applications
* **2026+**: AI / ML exploration & Research preparation
* **2027**: Expected CSE graduation

---

## 5. Featured Projects Data
These are the configurations mapped to the interactive case study cards on your home page:

### Project 1: Solid AI Assistant
* **Slug**: `solid-ai-assistant`
* **Title**: Solid AI Assistant
* **Category**: AI / Full-Stack
* **Short Description**: A personal Jarvis-style AI assistant built using Django and Ollama, designed to explore local and offline AI capabilities.
* **Tech Stack**: Python, Django, Ollama, LLM, SQLite
* **Highlight Quote**: *Exploring intelligent assistants that can operate locally while remaining useful and extensible.*
* **Overview**: Solid AI Assistant is a locally-run, Jarvis-style assistant that pairs a Django backend with Ollama for on-device model inference.
* **Problem**: Most consumer AI assistants require sending data to third-party cloud APIs, which limits privacy, offline use, and control over model behavior.
* **Solution**: A Django application orchestrates requests to a locally hosted Ollama model, storing conversation state in SQLite so the assistant works fully offline.
* **Architecture**: User → Frontend (Django templates) → Django application layer → Ollama (local LLM) → SQLite
* **Challenges**:
  * Keeping response latency reasonable on consumer hardware with a local model.
  * Designing a conversation memory model that stays useful without unbounded growth.
  * Structuring the app so it can later swap in other model backends.
* **Lessons Learned**:
  * How local LLM tooling like Ollama differs from cloud inference in practice.
  * Trade-offs between response quality and local hardware constraints.
  * Designing extensible service layers around a fast-moving AI ecosystem.

### Project 2: Smart Hotel Reservation System
* **Slug**: `smart-hotel-reservation-system`
* **Title**: Smart Hotel Reservation System
* **Category**: Full-Stack Web Application
* **Short Description**: A hotel reservation platform featuring authentication, room management, reservations, and an administrative dashboard.
* **Tech Stack**: Django, SQLite, Tailwind CSS, HTML, JavaScript
* **Overview**: A complete reservation workflow covering guest authentication, room availability, booking, and an admin dashboard for managing rooms and reservations.
* **Problem**: Small hotels often rely on manual booking processes that make it hard to track room availability and reservations accurately.
* **Solution**: A Django application models rooms, guests, and reservations, exposing an admin dashboard to manage inventory and bookings in one place.
* **Architecture**: User → Frontend (Tailwind + JS) → Django application layer → SQLite
* **Challenges**:
  * Preventing double-booking through correct availability queries.
  * Designing an admin dashboard that stays simple for non-technical staff.
  * Structuring authentication cleanly across guest and admin roles.
* **Lessons Learned**:
  * Modeling date-range availability correctly in a relational schema.
  * Building admin-facing tooling that is usable, not just functional.

### Project 3: Sheba Clinic — Pharmacy Management System
* **Slug**: `sheba-clinic-pharmacy-management-system`
* **Title**: Sheba Clinic — Pharmacy Management System
* **Category**: Full-Stack / Database
* **Short Description**: A pharmacy management system designed to manage customers, medicines, prescriptions, administrators, orders, and order details.
* **Tech Stack**: PHP, MySQL, HTML, CSS, JavaScript
* **Overview**: A relational system for managing pharmacy operations: customers, medicine inventory, prescriptions, orders, and administration.
* **Problem**: Pharmacies handling prescriptions and inventory by hand risk stock errors and lost records.
* **Solution**: A PHP and MySQL application normalizes customers, medicines, prescriptions, and orders into a relational schema with a clear admin workflow.
* **Architecture**: User → Frontend (HTML/CSS/JS) → PHP application layer → MySQL
* **Challenges**:
  * Designing a normalized schema that ties prescriptions to orders correctly.
  * Handling order/order-detail relationships without data duplication.
* **Lessons Learned**:
  * Practical relational database design under real-world constraints.
  * Structuring PHP applications around clear data boundaries.

### Project 4: Festivo
* **Slug**: `festivo`
* **Title**: Festivo
* **Category**: Database Management System
* **Short Description**: An event management system designed around structured database operations and web-based management.
* **Tech Stack**: PHP, MySQL, HTML, CSS, JavaScript
* **Overview**: Festivo organizes event creation, scheduling, and management through a structured relational database and a web interface.
* **Problem**: Coordinating events across organizers and attendees needs a reliable, centralized system rather than scattered spreadsheets.
* **Solution**: A PHP and MySQL application models events, organizers, and attendees, exposing web-based tools to manage them.
* **Architecture**: User → Frontend (HTML/CSS/JS) → PHP application layer → MySQL
* **Challenges**:
  * Structuring the schema to support recurring and one-off events cleanly.
  * Keeping the web interface simple for non-technical organizers.
* **Lessons Learned**:
  * Translating real-world event workflows into database schema.
  * Building CRUD-heavy interfaces that stay readable as they grow.

### Project 5: Campus Evacuation & Connectivity Analysis
* **Slug**: `campus-evacuation-connectivity-analysis`
* **Title**: Campus Evacuation & Connectivity Analysis
* **Category**: Algorithms / Graph Theory
* **Short Description**: A graph-based system for analyzing campus connectivity and evacuation routes using BFS and Dijkstra's algorithm.
* **Tech Stack**: Python, BFS, Dijkstra, Graph Algorithms
* **Overview**: Models a campus as a graph of buildings and paths, then analyzes connectivity and shortest evacuation routes.
* **Problem**: Understanding which paths are shortest or most critical during an evacuation isn't obvious from a map alone.
* **Solution**: Campus locations and paths are modeled as a weighted graph in Python; BFS finds reachability and Dijkstra's algorithm finds shortest evacuation routes.
* **Architecture**: Campus map data → Graph model (Python) → BFS / Dijkstra analysis → Output routes & connectivity report
* **Challenges**:
  * Translating a real physical campus layout into an accurate graph model.
  * Comparing BFS and Dijkstra results to validate correctness.
* **Lessons Learned**:
  * Applied graph theory to a real, spatial problem.
  * Trade-offs between unweighted (BFS) and weighted (Dijkstra) shortest paths.

### Project 6: IUBAT Library Management System
* **Slug**: `iubat-library-management-system`
* **Title**: IUBAT Library Management System
* **Category**: Software / Database
* **Short Description**: A library management system designed to organize books, users, borrowing records, and library operations.
* **Tech Stack**: PHP, MySQL, HTML, CSS
* **Overview**: A system for tracking a library's catalog, members, and borrowing activity.
* **Problem**: Manual tracking of borrowed books and due dates leads to lost books and inconsistent records.
* **Solution**: A relational database tracks books, members, and borrow/return records, with a web interface for library staff.
* **Architecture**: User → Frontend (HTML/CSS) → PHP application layer → MySQL
* **Challenges**:
  * Modeling borrowing history without losing referential integrity.
  * Designing clear staff-facing views for day-to-day operations.
* **Lessons Learned**:
  * End-to-end CRUD system design for a real institutional workflow.
  * Practical database normalization.

---

## 6. How to Edit Website Content
All visible content is loaded from a single file: `js/data.js`.
1. **To Update Projects**: Edit the `PROJECTS` array in `js/data.js`.
2. **To Update Skills**: Edit the `SKILLS` object, adding/removing items or changing their `level` (`learning`, `familiar`, `working`, `intermediate`).
3. **To Update Experience**: Edit the `EXPERIENCE` array.
4. **To Update Journey**: Edit the `JOURNEY` array.
5. **To Change Profiles**: Modify the values inside `SOCIAL_LINKS`.

---

## 7. How to Run & Deploy the Portfolio
Because this is a static webpage (fully client-side rendered), you can host it for free on any static provider without compiling anything.

### Running Locally
Run either of these commands in the project directory to serve it locally:
```bash
# Option A: Python server
python -m http.server 8000

# Option B: Node.js static server
npx serve .
```
Access the website at: `http://localhost:8000` (or the port shown by `serve`).

### Deploying to GitHub Pages
1. Create a repository named `AhmmedRizvi.github.io` on GitHub.
2. Initialize git and commit your files:
   ```bash
   git init
   git add .
   git commit -m "Initialize portfolio website"
   ```
3. Push to your repository:
   ```bash
   git remote add origin https://github.com/AhmmedRizvi/AhmmedRizvi.github.io.git
   git branch -M main
   git push -u origin main
   ```
4. Within a minute, your portfolio will be live at `https://ahmmedrizvi.github.io/`!
