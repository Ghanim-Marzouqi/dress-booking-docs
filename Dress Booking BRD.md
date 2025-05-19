
# Business Requirements Document: LUXURIOUS BRIDE Web Application

**Document Version:** 1.3
**Revision Date:** 19-May-2025
**Author:** Ghanim Al Marzouqi
**Project Owner:** Tasneem Al Shaybia
**Project Sponsor:** LUXURIOUS BRIDE Ownership/Management

---

## Table of Contents
1.  Introduction
    1.1. Purpose
    1.2. Project Background
    1.3. Document Scope
    1.4. Intended Audience
2.  Business Problem / Opportunity
    2.1. Problem Statement
    2.2. Opportunity Statement
3.  Proposed Solution
    3.1. Solution Overview
    3.2. Key Features (High-Level)
4.  Business Objectives & Goals
    4.1. Primary Objectives
    4.2. Secondary Objectives
    4.3. Success Metrics / KPIs
5.  Project Scope
    5.1. In Scope
    5.2. Out of Scope
    5.3. Deliverables
6.  Stakeholders
7.  Business Requirements
    7.1. Functional Requirements
        7.1.1. User Roles & Personas
        7.1.2. User Stories / Use Cases
    7.2. Non-Functional Requirements
        7.2.1. Performance
        7.2.2. Scalability
        7.2.3. Usability / User Experience (UX)
        7.2.4. Security
        7.2.5. Reliability & Availability
        7.2.6. Maintainability
        7.2.7. Compatibility (Platforms, Devices, Browsers)
    7.3. Data Requirements
    7.4. Reporting Requirements
    7.5. Regulatory/Compliance Requirements
8.  Assumptions & Constraints
    8.1. Assumptions
    8.2. Constraints
9.  Risks & Mitigation Strategies
    9.1. Identified Risks
    9.2. Mitigation Plans
10. Glossary
11. Appendices

---

## 1. Introduction

### 1.1. Purpose
This document outlines the business requirements for the LUXURIOUS BRIDE Web Application. It serves as a guide for project stakeholders and the development team to understand the business needs, objectives, scope, and desired outcomes of the project.

### 1.2. Project Background
LUXURIOUS BRIDE currently manages client inquiries for photo taking sessions and bookings for dress rentals primarily through manual, direct messaging channels, including **WhatsApp and Instagram Direct Messages (DMs)**. This distributed and manual process leads to challenges in efficiently tracking requests, coordinating availability, managing customer information, and scaling operations. This often results in mismanagement, difficulty in tracking requests/orders, and potential for errors. To address these issues, a web application, also titled "LUXURIOUS BRIDE," will be developed. This application will feature a public-facing landing page for clients to request photo sessions directly, and an administrator dashboard for staff to manage these web-submitted requests, confirm bookings, manage dress rentals (booked in-shop), and oversee overall operations, thereby providing a centralized alternative to the current chat-based methods.

### 1.3. Document Scope
This BRD covers the business requirements for the initial release (MVP) of the LUXURIOUS BRIDE Web Application. It defines what the app will do from a business perspective, not how it will be technically implemented (though key technology constraints are noted).

### 1.4. Intended Audience
This document is intended for: LUXURIOUS BRIDE Ownership/Management (Project Sponsor), Tasneem Al Shaybia (Project Owner), Ghanim Al Marzouqi (Project Manager & Developer), LUXURIOUS BRIDE Staff (Administrators), Prospective Clients (using the photo session request portal), and QA Team (if separate).

---

## 2. Business Problem / Opportunity

### 2.1. Problem Statement
LUXURIOUS BRIDE currently manages client inquiries and bookings for its core services—photo taking sessions and dress rentals—primarily through disparate manual chat-based systems, including **WhatsApp and Instagram DMs**. This reliance on fragmented, manual communication presents several operational challenges, including inefficiencies in tracking photo session requests across multiple platforms, coordinating availability for photographers, managing dress rental inventory and bookings (which are confirmed in-person), and consolidating customer information effectively. As the business grows, these methods become increasingly difficult to scale, leading to potential delays, missed opportunities, and a higher risk of errors in service fulfillment and resource allocation. Furthermore, the lack of a dedicated digital platform for initial inquiries can result in a less streamlined experience for customers and limits the business's ability to gather actionable data, optimize resource allocation for all services, and project a consistently high-end, organized brand image expected by its clientele.

### 2.2. Opportunity Statement
The development of a dedicated web application for LUXURIOUS BRIDE presents a significant opportunity to transform its operational efficiency and elevate the client experience, particularly for photo session inquiries. By introducing a structured web-based request system for photo sessions and a centralized backend for managing all services (including in-shop dress bookings and requests manually entered from **WhatsApp/Instagram DMs**), the business can significantly reduce administrative overhead and the potential for human error associated with manual, multi-channel coordination. This will enable clear visibility of photo session availability for clients via the web portal, streamlined request submission, and an efficient internal process for admin confirmation and client registration. For dress rentals, while booking remains in-shop, the system will centralize inventory and booking management. The application will provide a more professional and seamless initial contact point for photo session clients, consistent with the "LUXURIOUS BRIDE" brand, potentially attracting a wider clientele and reducing reliance on less formal DM-based interactions. The structured data captured for all services will unlock valuable insights into service popularity, booking trends, and resource utilization, empowering data-driven decision-making for future growth and service optimization.

---

## 3. Proposed Solution

### 3.1. Solution Overview
The proposed solution is a dedicated web application for LUXURIOUS BRIDE, designed to streamline the client inquiry process for photo taking sessions and centralize the management of all services, including in-shop dress rentals and requests received via other channels like **WhatsApp or Instagram DMs**. This web-based platform will feature a public-facing portal where clients can directly view photo session availability via an interactive calendar and submit a request by filling out a simple form. Dress rentals will continue to be booked in-person at the shop. For LUXURIOUS BRIDE administrators, the system will include an integrated backend interface to manage photo session services, process incoming web-submitted requests, manually input and manage requests received from **Instagram DMs or WhatsApp**, register clients, confirm photo session bookings, manage dress inventory and in-shop dress bookings, oversee booking calendars for all services, and handle client communications. The primary goal is to provide a sophisticated and convenient initial request experience for photo session clients through the web portal, and a robust, efficient internal management system for all LUXURIOUS BRIDE services, reflecting the premium nature of the brand while significantly improving operational efficiency and data management. The entire application (client-facing and admin) will support Arabic and English, with Arabic as the default. All financial references (e.g., rental fees) will be managed in OMR.

### 3.2. Key Features (High-Level)
*(No direct change here, as the app itself doesn't integrate with Instagram. The admin portal's ability to manually create bookings covers this. The problem it solves is now broader.)*
*   **1. Client-Facing Photo Session Request Portal:**
    *   Publicly accessible landing page showcasing photo session services.
    *   Interactive calendar displaying real-time availability for photo sessions.
    *   Simple request form for clients to select a time slot and submit their contact details (name, email, phone) and notes, without needing to register.
    *   Informational display of photo session package details.
    *   (Optional: View-only catalog of dresses, without online booking capability for dresses).

*   **2. Administrator Dashboard & Operations Management:**
    *   **Photo Session Service Management:** Admins can define, update, and manage details of photo session packages.
    *   **Dress Inventory & In-Shop Booking Management:** Admins can manage a catalog of rentable dresses (details, images, sizes) and record dress bookings made in-person at the shop, including advance payment status.
    *   **Photo Session Request Processing:** Admins can view and manage incoming photo session requests from the web portal **and manually input requests received from other channels (e.g., Instagram DM, WhatsApp).**
    *   **Admin-Led Client Registration & Booking Confirmation:** Admins can register clients based on request details (web or manual entry) and confirm photo session bookings within the system.
    *   **Centralized Booking Calendar:** A comprehensive calendar view for admins to see all confirmed photo sessions and dress rental periods.
    *   **Basic Client Information Management:** Admins can view and manage basic details of clients registered by them, along with their booking history.

*   **3. Automated Notifications (Multi-Channel):**
    *   System sends automated email and (with client consent) WhatsApp notifications to clients upon admin confirmation of their photo session booking, and for important reminders.
    *   Admins receive system notifications for new photo session requests submitted via the web portal.

*   **4. Multi-Language Support:**
    *   The entire web application (both client-facing portal and administrator dashboard) will support **Arabic and English**, with Arabic set as the default language.

*   **5. SEO-Friendly Public Pages:**
    *   The client-facing landing page and photo session request pages will be built with technical SEO best practices to enhance search engine visibility.

---

## 4. Business Objectives & Goals

### 4.1. Primary Objectives
*   **Objective 1: Enhance Operational Efficiency:** To reduce the administrative time spent managing client inquiries and scheduling for photo sessions (received via web portal, **WhatsApp, or Instagram DMs**) by at least 35%, and improve the efficiency of tracking dress rental inventory and bookings, within 6 months of the web application launch.
*   **Objective 2: Improve Client Photo Session Request Experience & Conversion (Web Portal):** To provide a seamless, professional, and user-friendly online request process via the web portal for photo sessions that results in a 20% increase in the conversion rate of photo session page visitors to submitted requests within 6 months post-launch, and gradually shift inquiries from DMs/WhatsApp to the portal.
*   **Objective 3: Facilitate Accurate Booking Management & Support Business Growth:** To support an increase in accurately managed and fulfilled service bookings (photo sessions and dress rentals combined) by 15% within 12 months post-launch, by making photo session requests more accessible via the web portal and overall service management (including manually entered requests) more robust.

### 4.2. Secondary Objectives
*(No direct change needed here, but the impact is amplified by consolidating more diverse manual channels.)*
*   **Objective 1: Strengthen Brand Image:** To elevate the LUXURIOUS BRIDE brand perception by offering a sophisticated, modern, and reliable online request platform for photo sessions and a well-organized backend for all services, consistent with its premium market positioning.
*   **Objective 2: Improve Data Accuracy and Insights:** To establish a centralized system for accurate capture and management of booking data (for photo sessions and dress rentals, regardless of original inquiry source), client information, and service performance, enabling better-informed business decisions and identification of trends.
*   **Objective 3: Reduce Booking Errors & Miscommunications:** To minimize errors (e.g., double bookings for photo sessions) and miscommunications associated with the current manual processes across multiple channels, leading to improved resource allocation and client satisfaction.

### 4.3. Success Metrics / KPIs
*(Minor adjustments to reflect the multiple manual channels)*
*   **KPI 1: Reduction in Administrative Time for Photo Session Processing:**
    *   Average time (e.g., in minutes) spent by staff processing a photo session request (from initial contact on any channel to system confirmation) (pre-app vs. post-app).
    *   Number of manual follow-ups or corrections required per photo session booking.
*   **KPI 2: Photo Session Request Channel Shift & Web Portal Conversion Rate:**
    *   Percentage of photo session inquiries originating from the web portal vs. manual channels (WhatsApp/Instagram DMs) over time.
    *   Percentage of visitors to the photo session landing page who submit a request form via the web portal.
    *   Ratio of submitted web portal photo session requests to admin-confirmed bookings.
*   **KPI 3: Booking Volume & Management:**
    *   Total number of confirmed photo sessions booked per month/quarter (consolidated in system).
    *   Total number of dress rentals recorded and managed in the system per month/quarter.
*   **KPI 4: Client Satisfaction (Photo Session Request Process):**
    *   Client feedback scores (e.g., on a 1-5 scale via short surveys post-confirmation) on the ease and clarity of the photo session request process (primarily for web portal users).
    *   Reduction in client complaints or issues related to photo session scheduling.
*   **KPI 5: System Usage & Data Integrity:**
    *   Number of photo session requests submitted via the web application daily/weekly.
    *   Number of client accounts created by admins (including those from manually entered requests).
    *   Percentage of dress inventory accurately reflected in the system.
*   **KPI 6: Error Rate Reduction:**
    *   Number of scheduling errors (e.g., double bookings for photo sessions, incorrect information for dress rentals) per month compared to baseline across all booking sources.

---

## 5. Project Scope

### 5.1. In Scope
*(Added a note in Admin-Facing section for manual entry)*
*   **Web Application Development (Client-Facing - Primarily for Photo Session Requests):**
    *   Development of a responsive web application accessible via standard web browsers (desktop and mobile).
    *   User interface (UI) and user experience (UX) design for client-facing pages.
    *   **Public Landing Page:** Featuring an interactive calendar for photo session availability.
    *   **Photo Session Availability Calendar:** Clients can view available dates/time slots for photo sessions.
    *   **Photo Session Request Form:** Upon selecting an available slot, clients can submit a request by providing their full name, email, phone number, and optional notes. (No client registration required to submit a request).
    *   **Multi-Language Support:** The client-facing interface will support **English and Arabic, with Arabic as the default language.**
    *   (Optional, if pursued: View-only catalog of dresses with images and descriptions, clearly indicating booking is in-shop only).

*   **Web Application Development (Administrator-Facing):**
    *   Development of a secure admin dashboard/portal using Firebase Authentication.
    *   User interface (UI) and user experience (UX) design for admin-facing pages.
    *   **Multi-Language Support:** The admin portal will support **English and Arabic, with Arabic as the default language.**
    *   **Service Management (Photo Sessions):** CRUD (Create, Read, Update, Delete) functionality for photo session packages/types (e.g., defining duration, what's included, internal notes), including image uploads via Firebase Storage.
    *   **Dress Inventory Management:** CRUD functionality for dress listings (images via Firebase Storage, descriptions, sizes, unique ID, rental fee reference in OMR). Admins can manage availability status (e.g., available, booked, maintenance, cleaning).
    *   **Booking Request Management (Photo Sessions):** Admins can view incoming photo session requests from the web portal **and have functionality to easily manually input and track requests received via other channels (e.g., Instagram DM, WhatsApp).**
    *   **Client Registration (Admin-initiated):** Admins can register a client account based on request details (web or manual entry) or in-shop visit.
    *   **Order Creation (Admin-initiated):** Admins can create a confirmed booking for a photo session for a registered client, linking it to their request and updating calendar.
    *   **Dress Booking Management (Admin-initiated):** Admins can manually create and manage dress bookings for clients who visit the shop (including client details, dress ID, rental start/end dates, and advance payment status tracking).
    *   **Calendar Management:** Centralized view for admins of all scheduled photo sessions and dress rental periods, with filtering options.
    *   **Client Management (Basic):** Admins can view and manage client accounts created by them (contact info, notes), and view their booking history (photo sessions and dress rentals).
    *   **Automated Notifications (Client - Post-Admin Confirmation):** Email and (with consent) WhatsApp notifications sent to clients once an admin confirms their photo session booking and for booking reminders.
    *   **Automated Notifications (Admin):** Notifications (e.g., on-screen, email) for new photo session requests submitted via the web portal.

*   **General:**
    *   Database design and setup (PostgreSQL) to store all application data.
    *   Integration of Firebase Authentication for secure administrator portal access.
    *   Integration of Firebase Storage for efficient management (upload, storage, retrieval) of images related to services and dresses.
    *   Basic security measures (e.g., HTTPS, input validation, protection against common web vulnerabilities like XSS, SQLi).
    *   **Search Engine Optimization (SEO):** Implementation of technical SEO best practices for the client-facing public landing page to improve search engine visibility (e.g., semantic HTML, meta tags, sitemap.xml, robots.txt, schema markup for services, site performance optimization).
    *   Testing (Unit, Integration, User Acceptance Testing support).
    *   Deployment of the web application to a hosting environment.
    *   Basic training for administrators.

### 5.2. Out of Scope
*(No direct change needed here, but the app's non-integration with Instagram/WhatsApp is reinforced)*
*   **Direct automated integration with Instagram DMs or WhatsApp for request intake.** (Requests from these channels will be manually entered by admins).
*   **Client Self-Registration/Client Accounts (for initial photo session request):** Clients do not create accounts to request a photo session. Account creation is admin-initiated post-request.
*   **Online Payments / Payment Gateway Integration:** All payments are handled offline. The system will not process online transactions.
*   **Client-Facing Online Dress Booking:** Clients cannot book dresses directly via the web application.
*   **Native Mobile Applications (iOS/Android):** The solution is a web application.
*   **Display of prices in any currency other than OMR (e.g., USD exchange rate display).**
*   **Advanced Analytics & Complex Custom Reporting:** Dashboards beyond basic operational views for admins.
*   **Photographer-Specific Portals/Logins.**
*   **Client-to-Client Interaction:** Features like client reviews, ratings, or forums.
*   **Marketing Automation Integrations (beyond transactional email/WhatsApp notifications).**
*   **On-site/Physical Point of Sale (POS) System Integration.**
*   **Complex Customization Requests from Individual Clients for Photo Sessions via the Web Form.**
*   **Content Creation for Services/Dresses:** The business (LUXURIOUS BRIDE) will be responsible for providing all textual descriptions, images, and pricing details for services and dresses in both Arabic and English.
*   **Ongoing content-based SEO campaigns (e.g., blog writing, link building) beyond technical optimization of the web application itself.**
*   **Integration with any other third-party systems not explicitly mentioned in "In Scope" (e.g., accounting software).**
*   **Advanced user role management beyond a single 'Administrator' type.**

### 5.3. Deliverables
*(No change needed)*

---

## 6. Stakeholders
*(No change needed)*

---

## 7. Business Requirements

### 7.1. Functional Requirements

#### 7.1.1. User Roles & Personas
*(Minor update to Admin goals)*
*   **User Role 1: Prospective Client (Guest User)**
    *   Description: An individual visiting the LUXURIOUS BRIDE website to inquire about photo taking sessions. Does not have an account.
    *   Goals: To easily view available dates/times for photo sessions, understand service offerings (with fees in OMR), and submit a request for a photo session without needing to create an account. To receive clear feedback that their request has been submitted.
*   **User Role 2: Registered Client (Managed by Admin)**
    *   Description: A client whose details have been entered into the system by an administrator after a photo session request is processed (from web or manual entry from DM/WhatsApp) or an in-shop dress booking is made. They primarily interact with the business via notifications.
    *   Goals: To receive clear confirmation and reminders about their bookings via email and/or WhatsApp.
*   **User Role 3: Administrator (LUXURIOUS BRIDE Staff)**
    *   Description: Staff member responsible for managing service offerings, photo session requests (from web and manual channels), client registration, booking confirmations, dress inventory, in-shop dress bookings, and overall system operation using the defined technology stack.
    *   Goals: To efficiently manage all incoming photo session requests from the web portal and easily input requests received via **Instagram DMs/WhatsApp**, maintain an accurate booking calendar for all services, manage dress inventory effectively (including uploading images to Firebase Storage), register clients with necessary details, confirm bookings, communicate with clients, and ensure a smooth operational workflow with minimal errors. To switch interface language between Arabic and English.

#### 7.1.2. User Stories / Use Cases
*(Added a User Story for admin manual entry)*
*   **Client-Facing (Photo Session Request Portal):**
    *   **FR-001:** As a Prospective Client, I want to view a calendar showing available time slots for photo sessions, so that I can choose a convenient time for my request.
    *   **FR-002:** As a Prospective Client, I want to easily switch the website language between Arabic and English, so that I can view information in my preferred language.
    *   **FR-003:** As a Prospective Client, I want to submit a photo session request by providing my full name, email, phone number, and preferred date/time, so that LUXURIOUS BRIDE can contact me to confirm.
    *   **FR-004:** As a Prospective Client, I want to receive an on-screen confirmation message after submitting my request, so I know it has been successfully sent.
    *   **FR-005:** (Optional) As a Prospective Client, I want to browse a view-only catalog of dresses with images and descriptions (rental fees in OMR), so I can get an idea of styles before visiting the shop.
*   **Administrator Portal:**
    *   **FR-006:** As an Administrator, I want to log in securely to the admin portal using my Firebase Authentication credentials, so that I can access management functions.
    *   **FR-007:** As an Administrator, I want to easily switch the admin portal language between Arabic and English, so that I can work in my preferred language.
    *   **FR-008:** As an Administrator, I want to receive a notification (e.g., dashboard alert, email) for a new photo session request submitted via the web portal, so that I can promptly review and process it.
    *   **FR-009:** As an Administrator, I want a clear and efficient way to manually enter a new photo session request received via Instagram DM or WhatsApp, capturing client details (name, contact, requested date/time, notes), so it can be processed within the system.
    *   **FR-010:** As an Administrator, I want to view a list of all photo session requests (both web-submitted and manually entered) with their details and status (e.g., New, In Progress, Confirmed, Cancelled), so I can manage the workflow.
    *   **FR-011:** As an Administrator, I want to be able to register a new client in the system using their name, email, and phone number from a request or in-shop visit, so that I can create a formal booking for them.
    *   **FR-012:** As an Administrator, I want to confirm a photo session booking in the system for a registered client, select the service package, and have the calendar updated automatically, so that the slot is marked as unavailable and the client receives a confirmation.
    *   **FR-013:** As an Administrator, I want to add, edit, and manage photo session package details (name, description, duration, internal notes, images uploaded to Firebase Storage), so that information is accurate.
    *   **FR-014:** As an Administrator, I want to add, edit, and manage dress details in an inventory (name, description, size, images uploaded to Firebase Storage, rental fee in OMR, unique ID), so that we have an accurate catalog.
    *   **FR-015:** As an Administrator, I want to update the availability status of a dress (e.g., Available, Booked, Maintenance, Cleaning), so that inventory is current.
    *   **FR-016:** As an Administrator, I want to create a new dress booking for a registered client, selecting the dress, rental dates, and noting the advance payment status, so that the booking is recorded and the dress availability is updated.
    *   **FR-017:** As an Administrator, I want to view a master calendar showing all confirmed photo sessions and dress rental periods, so I can have an overview of all scheduled activities.
    *   **FR-018:** As an Administrator, I want to view and edit basic client information (contact details, notes, booking history), so client records are up-to-date.
    *   **FR-019:** As an Administrator, I want the system to automatically send a confirmation email and WhatsApp message (with consent) to a client when their photo session is confirmed, so they are informed.
    *   **FR-020:** As an Administrator, I want to be able to manually trigger a reminder notification to a client for an upcoming booking.
    *   **FR-021:** As an Administrator, I want to mark a photo session or dress booking as completed or cancelled, so the records are accurate.

### 7.2. Non-Functional Requirements
*(No changes needed here for this update)*

### 7.3. Data Requirements
*(Minor clarification for client data source)*
*   **Prospective Client Request Data:** Full name, email address, phone number, preferred date/time for photo session, notes, source of request (Web Portal, Instagram DM, WhatsApp).
*   **Registered Client Data:** Unique Client ID, full name, email address, phone number, registration date, communication preferences (e.g., consent for WhatsApp), internal notes.
*   **Photo Session Service Data:** Service ID, name (Arabic/English), description (Arabic/English), duration, included items, internal notes.
*   **Photo Session Booking Data:** Booking ID, Client ID, Service ID, confirmed date/time, status (e.g., Confirmed, Completed, Cancelled), creation date, admin notes.
*   **Dress Data:** Dress ID (unique), name/description (Arabic/English), size, color, high-quality images (multiple angles), rental fee (in OMR for reference), current status (Available, Booked, Maintenance, Cleaning), acquisition date, internal notes.
*   **Dress Booking Data:** Dress Booking ID, Client ID, Dress ID, rental start date, rental end date, advance payment status (e.g., Paid/Unpaid/Amount), actual return date, booking status (e.g., Confirmed, Active, Completed, Cancelled), admin notes.
*   **Admin User Data:** User ID, username, hashed password, role (Administrator), language preference.
*   All textual data requiring localization (e.g., service names, descriptions) must support storage for both Arabic and English.
*   Data to be stored in a relational database (PostgreSQL).

### 7.4. Reporting Requirements
*(No changes needed here for this update)*

### 7.5. Regulatory/Compliance Requirements
*(No changes needed here for this update)*

---

## 8. Assumptions & Constraints

### 8.1. Assumptions
*   LUXURIOUS BRIDE staff will continue to monitor **Instagram DMs and WhatsApp** for photo session requests and will be responsible for manually entering these requests into the new web application's admin portal if clients do not use the web portal directly.
*   LUXURIOUS BRIDE staff have access to reliable internet and compatible devices (computers/tablets) to use the admin portal effectively.
*   Prospective clients generally have access to modern web browsers on desktops or mobile devices capable of rendering responsive websites.
*   The business (LUXURIOUS BRIDE) will provide all necessary content (textual descriptions, high-quality images, service details) for the photo session packages and dress catalog in both Arabic and English, in a timely manner.
*   Access to and cooperation for integrating with a WhatsApp Business API provider will be available and feasible if direct API integration for notifications is pursued. If not, admins will handle WhatsApp communication manually guided by system information.
*   The business has clear, existing internal processes for handling payments offline and managing physical dress handovers/returns.
*   Staff are willing and able to be trained on the new system.

### 8.2. Constraints
*(The technology stack information has been moved here for clarity and consistency)*
*   **Budget:** [To be specified by LUXURIOUS BRIDE Ownership/Management, e.g., The project has an allocated budget of X OMR for MVP development.]
*   **Timeline:** [To be specified by LUXURIOUS BRIDE Ownership/Management, e.g., The MVP is targeted for launch within Y months from project commencement.]
*   **Resources (Development):** Development primarily relies on Ghanim Al Marzouqi. Additional specialized resources (e.g., for complex UX/UI design for Arabic) may need to be considered or outsourced if required.
*   **Technology Stack (Initial):**
    *   **Frontend:** React (likely with React Router v7) + TypeScript
    *   **UI Framework:** Tailwind CSS
    *   **Database:** PostgreSQL
    *   **Backend:** NestJS + Prisma ORM
    *   **Authentication:** Firebase Authentication (integrated with NestJS for admin portal)
    *   **File Upload/Download:** Firebase Storage (integrated with NestJS for images)
*   **No Online Payments (MVP):** The system will not integrate any payment gateways for V1. All financial transactions are handled offline. Default currency for display/reference is OMR.
*   **Dress Booking Process (MVP):** Dress bookings are finalized in-person at the shop; the web app only supports admin management of these bookings and related inventory.
*   **No direct integration for automated intake from Instagram DMs or WhatsApp.**

---

## 9. Risks & Mitigation Strategies
*(No changes needed here for this update, though the manual entry reinforces Risk 5 if not done efficiently)*

### 9.1. Identified Risks
*   **Risk 1: Scope Creep:** Requests for features outside the defined MVP (e.g., online payments, client self-service for dress bookings, advanced reporting, direct Instagram/WhatsApp integration) during development.
    *   *Likelihood: High, Impact: Medium*
*   **Risk 2: Content Delays:** Delays in receiving necessary business content (text, images for services and dresses in Arabic & English) from LUXURIOUS BRIDE, impacting development timelines.
    *   *Likelihood: Medium, Impact: Medium*
*   **Risk 3: WhatsApp Business API Complexity/Cost:** Challenges with WhatsApp Business API integration (technical, policy approval) or unexpected costs associated with its use for outgoing notifications.
    *   *Likelihood: Medium, Impact: Medium*
*   **Risk 4: Bilingual Implementation Challenges:** Underestimation of complexity for robust bilingual (Arabic/English) implementation, especially regarding UI/UX for right-to-left (RTL) layout, date/time formats, and testing.
    *   *Likelihood: Medium, Impact: Medium*
*   **Risk 5: Staff Adoption & Training:** LUXURIOUS BRIDE staff resistance to change or insufficient training leading to low adoption or incorrect/inefficient use of the admin portal, especially for manual entry of DM/WhatsApp requests.
    *   *Likelihood: Medium, Impact: Medium* (Increased likelihood slightly due to manual entry aspect)
*   **Risk 6: Key Person Dependency:** Heavy reliance on Ghanim Al Marzouqi for both project management and development could create a bottleneck or risk if availability is impacted.
    *   *Likelihood: Medium, Impact: High*

### 9.2. Mitigation Plans
*   **For Risk 1:** Strict adherence to the defined scope in this BRD. Implement a formal change request process for any deviations. Prioritize MVP features. Regular stakeholder meetings with Tasneem Al Shaybia to manage expectations.
*   **For Risk 2:** Establish clear content delivery schedules and formats with LUXURIOUS BRIDE early in the project. Provide templates or guidelines for content. Use placeholder content during development if necessary but highlight impact.
*   **For Risk 3:** Thoroughly research WhatsApp Business API provider options, policies, and costs early. Design the system to allow for manual WhatsApp notifications based on system alerts as a fallback if API integration is delayed or unfeasible for MVP.
*   **For Risk 4:** Allocate sufficient time for design, development, and thorough testing of bilingual features. Utilize established libraries/frameworks that support internationalization (i18n) and RTL. Consider engaging a UX consultant with Arabic language expertise if needed.
*   **For Risk 5:** Involve staff representatives in UAT. Provide clear, concise training documentation (in Arabic/English) and hands-on training sessions. Emphasize the efficiency gains and error reduction benefits of centralizing all requests, even those manually entered, into the new system.
*   **For Risk 6:** Document all critical project information and technical designs. Ghanim Al Marzouqi to prioritize tasks effectively. For critical phases, identify potential backup support or knowledge transfer opportunities if feasible within budget/resource constraints. Open communication with Tasneem Al Shaybia about workload and potential risks.

---

## 10. Glossary
*(No changes needed here for this update)*

---

## 11. Appendices
*(No changes needed here for this update)*

---
**Document Approval Signatures (if applicable for formal process):**

*   **Project Sponsor (LUXURIOUS BRIDE Owner/Manager):** _________________________ Date: _________
*   **Project Owner (Tasneem Al Shaybia):** _________________________ Date: _________
*   **Project Manager (Ghanim Al Marzouqi):** _________________________ Date: _________
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2MzI3ODM1MjBdfQ==
-->