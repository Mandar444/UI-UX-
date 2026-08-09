# Viva Voce Defense Preparation Guide
## UI/UX Mid-Term Examination Case Study Defense Sheet
**Project Title**: Booking a Classroom Shouldn’t Require Guesswork  
*Note: This guide is prepared for oral examination / viva voce defense. Excluded from `submission.zip`.*

---

## Section 1: Research Methodology & Data Integrity

### Q1: Why did you separate your survey respondents into 12 experienced users and 5 inexperienced users?
> **Answer**:  
> In our 17-person survey, 5 respondents had never attempted to book a campus classroom. When asked about process satisfaction, some gave high ratings (4 or 5 out of 5) simply because they had never experienced administrative delays, paperwork, or room conflicts. 
> If we had averaged all 17 responses together, the pain statistics would have been distorted. Therefore, to ensure empirical accuracy, we isolated the **12 respondents with direct booking experience** to analyze pain points (75% hidden availability, 67% slow approval, 58% cancelled events) and calculate true satisfaction (2.42 out of 5).

### Q2: Why did your research methodology use a structured survey rather than 3 observational interviews?
> **Answer**:  
> The available Phase 1 research comprised a structured participant survey with 17 respondents (16 students, 1 club coordinator). To maintain strict academic integrity, we accurately labeled the methodology as a **Structured Participant Survey**. Fabricating interview records, participant names, or fake quotes would violate research ethics. We utilized all authentic qualitative feedback and structured data from the 17 respondents.

---

## Section 2: Information Architecture & Tree-Test Diagnostics

### Q3: Why did IA V1 fail on Task 1 during tree testing, and what was your structural pivot?
> **Answer**:  
> In IA V1, we separated *Find a Classroom* and *Book a Classroom* into distinct top-level branches based on card-sorting categories. However, during tree testing, **Task 1 (Check availability) achieved only 40% direct success** (60% of users started under *Book a Classroom* or *My Bookings*).  
> **Structural Pivot**: Participants mentally treat room discovery and reservation as one continuous activity. In **IA V2**, we merged these branches into **"Find and Book a Classroom"**, while preserving sub-groupings for room details and starting a booking.

### Q4: Explain the "Satisfaction vs. Path Accuracy Gap" discovered during tree testing.
> **Answer**:  
> On Task 1, **80% of participants reported high satisfaction** with their choice, even though **60% actually selected the wrong menu path**. This proves a critical UX principle: *subjective user confidence is often misleading*. Requesters assume they are on the right path even when navigating incorrectly, demonstrating why objective path tracking (tree testing) is mandatory before finalizing Information Architecture.

---

## Section 3: Prioritization & Trade-Off Analysis

### Q5: Why did you relegate Escalate Delayed Request to "Won't Have in this MVP" despite 67% complaining of slow approval?
> **Answer**:  
> Escalating a delayed request requires defined Service Level Agreements (SLAs), administrative escalation roles, and policy enforcement rules. Technology cannot enforce escalation before institutional policy exists. The MVP first provides status transparency and logs request timestamps to establish empirical baseline data on approval delays before introducing policy escalation logic.

### Q6: Why did Check Approval Status beat Notification for the final Must-Have spot in DFV analysis?
> **Answer**:  
> In our DFV matrix:
> - **Check Approval Status** scored **14 / 15**: Desirable (5/5), Feasible (4/5, exposes existing database state), Viable (5/5, zero messaging delivery cost).
> - **Approval or Rejection Notification** scored **10 / 15**: Desirable (4/5), Feasible (3/5, requires mail servers, trigger logic, retry queues), Viable (3/5, ongoing maintenance).
>  
> Check Approval Status directly solves the primary pain (approval uncertainty) with zero infrastructure overhead, whereas Notification adds delivery complexity that manual status checking easily bypasses for an MVP.

---

## Section 4: Project Scope & Editorial Constraints

### Q7: Why are there no app screens, wireframes, or mobile mockups on this website?
> **Answer**:  
> This project is strictly an **editorial UX research case study and information architecture blueprint**. Designing visual screens before validating taxonomy leads to superficial UI fixes that mask underlying structural confusion. By focusing exclusively on research sensemaking, card sorting, tree testing, and MoSCoW/DFV prioritization, we established a validated structural foundation (IA V2) before any UI design begins.
