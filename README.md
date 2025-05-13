# 🚀 Datanaut

**Explore data like never before.**  
Datanaut is a full-stack Azure-powered analytics platform designed to replace Excel-based workflows with a scalable, interactive, and modern web application.

---

## 🌐 Tech Stack

### 🔧 Frontend
- **React** – UI framework
- **TanStack Query** – Data fetching & caching
- **Wouter** – Lightweight routing
- **Tailwind CSS** – Utility-first styling
- **shadcn/ui** – Accessible UI components
- **React Hook Form** – Form handling
- **Framer Motion** – UI animations

### 🧪 Backend
- **ASP.NET Core Web API** – RESTful API
- **Formula Engine** – Custom calculation logic in `calculator.ts`
- **Excel Import** – Using `EPPlus` or `ClosedXML`
- **Authentication** – Optional: Azure AD or ASP.NET Identity

### 🗄️ Database
- **Azure SQL Database** – Scalable relational backend
- **Azure Blob Storage** – File upload/export handling
- **Azure Functions** *(optional)* – Background processing

---

## 🧱 Architecture Overview

```txt
Frontend (React + Tailwind) --> API (ASP.NET Core) --> Azure SQL Database
                                |
                          Excel Parser + Formula Engine
```
## 🧩 Key Frontend Components

### 📊 Excel-like Grid
**File:** `client/src/components/ui/data-grid.tsx`

- Editable cells with formula support (`=SUM(C2:F2)`)
- Cell formatting, copy/paste, selection
- Reactive formula recalculation

### 🧭 Layout
- `Header.tsx` – Title, user info, global actions  
- `Sidebar.tsx` – Workbooks & database connections  
- `RightPanel.tsx` – Visualizations & DB insights  
- `StatusBar.tsx` – Sync info and status indicators  

### 📈 Data Insights
- `chart.tsx` – Bar charts  
- `progress-bar.tsx` – KPIs and progress indicators  
- `database-status.tsx` – Real-time connection monitoring  

### 💬 Dialogs & Modals
- `formula-modal.tsx` – Advanced formula editor  
- `loading-indicator.tsx` – Operation feedback  
- `tutorial-modal.tsx` – Guided onboarding experience  

---

## 📄 App Pages

- `home.tsx` – Landing page with app overview, tutorial, and feature showcase  
- `data-sheet.tsx` – Main Excel-like data interface with formula bar  
- `visualizations.tsx` – Chart/dashboard view with filters  
- `reports.tsx` – Custom reports with export & scheduling options  

---

## 🔄 Data Flow

- **TanStack Query** handles all API interactions and caching  
- **API logic** defined in: `client/src/lib/queryClient.ts`  
- **Azure integration** (`azure-service.ts`) manages:
  - Database connections  
  - Import/export actions  
  - Real-time sync indicators

- **Formula Engine** (`calculator.ts`):
  - Parses Excel-style formulas (e.g. `SUM`, `AVERAGE`)  
  - Supports cell references and ranges  
  - Automatically updates dependent cells  

---

## 📱 Responsive Design

- Mobile/tablet/desktop support  
- Collapsible sidebar for smaller screens  
- Grid + Flexbox-based layout  
- Touch-friendly UI interactions  

---

## ✨ User Experience Features

- ✅ 15-step tutorial for onboarding new users  
- 🎯 Excel-style keyboard shortcuts (`F2` to edit, `Ctrl+C/V`, etc.)  
- 🎨 Light/Dark mode with customizable theme accents  
- 📘 Feature showcase and "Get Started" guide on homepage  

---

## 📦 Future Enhancements

- 🧠 AI-assisted formula suggestions  
- 🤝 Shared workbooks and team collaboration  
- 📊 Custom chart builder UI  
- 📤 PDF and Excel export engine  

---

## 📛 Name Inspiration

**Datanaut** = *Data* + *Astronaut*  
*Explore, analyze, and launch insights 🚀*

---

## 🧠 Project Purpose

Datanaut is a portfolio-grade full stack application that demonstrates:

- Cloud integration (Azure SQL, Blob Storage)  
- Scalable spreadsheet-style data manipulation  
- Custom formula engine  
- Clean, modern frontend design with real-time UX  

It can serve as:
- A professional portfolio centerpiece  
- An internal analytics tool for teams  
- A prototype for a SaaS spreadsheet alternative  

---

## 📬 Contact

For collaboration, feedback, or questions:  
[github.com/jamreichen](https://github.com/jamreichen) • [linkedin.com/in/jamiereichenberger](https://www.linkedin.com/in/jamiereichenberger/)

