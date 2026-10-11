# WD-401 Term Project Guide

**Student Instructions**

**Course Term Project**  
October 13 – December 18, 2026

## 1. Project Overview

This term project is a simulation of a real production build. Over ten weeks, your team will plan, design, build, and present a full-scale web platform. This is not a sample assignment — it is treated as professional work from day one.

You have two paths to choose from.

### Path A – Your Own Project

Your team may propose and build a project of your own. This is the path we encourage if your team has an idea you genuinely want to build and ship.

If you choose this path, your project must be **at least as feature-rich as ManageSmartr** (described in Path B). The scope bar in Section 2 defines what "as feature-rich" means in practice.

Path A teams will spend the first two weeks of the term producing their own Project Scope Document and Figma design (see Section 4), equivalent to the ones provided for ManageSmartr. Development begins once the instructor approves them.

### Path B – ManageSmartr (Default)

If your team does not have an idea you want to pursue, you will build **ManageSmartr**, a web platform for BuildSmartr Inc. that modernizes the process of ordering, managing, and tracking steel wall deliveries.

You are expected to deliver all major platform features, including:

- Admin System (Clients, Projects, PDFs, Orders, Status Control)
- Client Portal (Kanban Board, Modification Requests, Orders, Tracking)
- Employee Views (Driver, Manufacturer, Sales – Status Updates)
- Invoicing, Logs, Notifications, Dashboard UI

Whichever path you take, the expectations, timeline, and standards are the same.

## 2. Scope Bar for Own Projects (Path A)

To be approved, a Path A project must include **all** of the following:

- At least three distinct user roles with authentication and role-based access
- A relational database schema with roughly eight or more related entities
- A multi-stage status workflow with defined business rules (for example, an order lifecycle or an approval pipeline)
- File upload and cloud storage (documents, images, or PDFs)
- Notifications (in-app, email, or both)
- A dashboard with summaries or reporting
- Activity logs or an audit trail
- A deployed, publicly accessible build by the final presentation

Simple CRUD apps, single-role tools, and tutorial clones will not be approved.

## 3. Reference Materials

**Path B teams** will work from two core documents provided by the instructor:

- ManageSmartr Project Scope Document (Functional & Feature Requirements) - https://docs.google.com/document/d/1tgPmZvT5URFDjGnw9VqST5o3aCgWkb9Jp3Y5PDXNAmg/edit?usp=sharing
- Figma Design Link (Visual direction and interface layout) - https://www.figma.com/design/0cwQuhdZMnKYgnot8RuAUk/ManageSmart?node-id=64-772&t=WyHSDqmJPzyNtYzk-1

These documents define your requirements. Do not invent features outside of these references.

**Path A teams** do not receive these documents. You will create the equivalent for your own project during the documentation and approval phase (see Section 4). Use the ManageSmartr documents as the reference for the level of detail expected.

## 4. Documentation & Approval Phase (Path A)

The first two weeks of the term (**October 13 – October 23**) are the documentation and approval phase for Path A teams. Before any development begins, your team must prepare the following and have it approved by the instructor.

**1. Project Scope Document** — modeled on the ManageSmartr Scope Document. At minimum it must include:

- Problem statement and project goals
- User roles and their permissions
- Complete feature list, mapped to the scope bar in Section 2
- User flows for each role
- Status workflows and business rules
- Database schema (ERD with entities, fields, and relationships)
- Technology stack and third-party services

**2. Figma Design** — covering all major screens and user flows for every role.

Submit both to the instructor by **Friday, October 23**. The instructor will review and either approve the project or request revisions. Once approved, these documents become your team's requirements for the rest of the term and are held to the same standard as the ManageSmartr references.

## 5. Team Structure & Roles

- Teams will be determined by the instructor.
- Teams may self-organize roles internally, but each team ***must declare one Product Manager***.
- The Product Manager is responsible for communication with the instructor, understanding the product requirements, and tracking team deliverables.
- Every member must contribute to development; no one may remain in a non-coding role.

## 6. Technology Expectations

Both paths must be built on the same core stack:

- Next.js / React
- Relational Database (PostgreSQL or MySQL)
- Authentication (NextAuth, Clerk, or Supabase)
- Cloud Storage for files (S3, Cloudflare R2, Supabase Storage, etc.)

You may include supporting libraries or tools, but you cannot replace the core platform stack.

## 7. Development Expectations

- **Full Build Required:** All core functionalities must be attempted.
- **Design Compliance:** UI must follow the provided Figma (Path B) or your approved design (Path A).
- **Feature Flow Accuracy:** Follow the exact status stages and business logic defined in your scope document.
- **Architecture Planning:** Teams are expected to produce a basic system structure before coding.

## 8. Progress & Accountability

Follow the 10-week timeline below. The instructor may visit any team during any class and request:

- Progress update
- Code walkthrough
- Feature demonstration

There are two formal checkpoints in addition to the final presentation:

- **Mid-Term Demo – Friday, November 20:** Each team demonstrates working features to the instructor.
- **Feature Freeze – Friday, December 4:** No new features after this date. Remaining time is for testing, integration, and polish.

Lack of progress will not be excused by planning delays.

## 9. Scope Updates

Minor adjustments or clarifications to features may be provided by the instructor during the term. These changes will be clearly communicated and reflected in shared documentation. Teams must adapt professionally.

## 10. Final Deliverables

You will present a working platform on **Friday, December 18**. Your final presentation must include:

- Live walkthrough of features (not slides only)
- Real end-to-end workflows across every user role
- Team explanation of architecture and challenges
- A deployed, publicly accessible build

This project is a simulation of a real production team. Treat it with professional standards.

## 10-Week Timeline (Oct 13 – Dec 18)

| Week    | Dates            | Primary Focus                                                                                                                                                  |
|---------|------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Week 1  | Oct 13 – Oct 16  | Project Orientation<br>Teams announced by the instructor, choose your path<br>Path A: begin Project Scope Document & Figma design<br>Path B: read Scope Doc & study Figma, understand all user flows |
| Week 2  | Oct 19 – Oct 23  | Planning & Architecture<br>Declare Product Manager<br>Define tasks, assign responsibilities<br>Path A: finalize Scope Document & Figma, submit for approval (due Oct 23)<br>Path B: draft system architecture & database model (ERDs) |
| Week 3  | Oct 26 – Oct 30  | Development Sprint 1<br>Project setup, authentication & roles, database schema, app skeleton                                                                  |
| Week 4  | Nov 2 – Nov 6    | Development Sprint 2<br>Core admin modules and primary CRUD flows                                                                                              |
| Week 5  | Nov 9 – Nov 13   | Development Sprint 3<br>Secondary user roles and their views                                                                                                   |
| Week 6  | Nov 16 – Nov 20  | Development Sprint 4<br>Status workflows and business logic<br>**Mid-Term Demo – Fri Nov 20**                                                                   |
| Week 7  | Nov 23 – Nov 27  | Development Sprint 5<br>File storage, notifications, logs                                                                                                      |
| Week 8  | Nov 30 – Dec 4   | Development Sprint 6<br>Dashboard, invoicing/reporting, remaining modules<br>**Feature Freeze – Fri Dec 4**                                                    |
| Week 9  | Dec 7 – Dec 11   | Testing & Integration<br>Bug fixing, flow validation<br>Data consistency & UX cleanup<br>Deployment                                                            |
| Week 10 | Dec 14 – Dec 18  | Finalization & Mock Presentations<br>Polish & refine<br>Prepare live demo & team presentation<br>**Final Presentation – Fri Dec 18**                            |

The project timeline is not adjusted around college holidays. For holidays and closures, refer to the CICCC Academic Calendar: https://ciccc.ca/en/academic-calendar

## Reminder to Teams

> Your success depends on clarity, collaboration, and steady progress. Treat this as production work — design carefully, build responsibly, and communicate consistently.
