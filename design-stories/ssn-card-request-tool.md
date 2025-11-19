---
layout: page
title: SSN Card Request Tool
permalink: /design-stories/ssn-card-request-tool/
classes: large-text
---

[← Back to Design Stories]({{ site.baseurl }}/design-stories/)

# SSN Card Request Tool  
### Workflow Design • Eligibility Logic • UX Writing • Mobile-First UI • End-to-End HCD

---

## Design Story Overview

Requesting or replacing a Social Security card sounds simple — but in practice, it’s one of SSA’s **most complex eligibility workflows**.

Users fall into dozens of categories:

- Newly married / name change  
- U.S. citizens or non-citizens  
- Newborns applying for their first SSN  
- People living abroad  
- People experiencing homelessness  
- Users without access to original documents
- Those that can file online, must appear in person, or are able to do both

Before this work, SSA’s guidance was difficult to navigate:

- **Scattered across many pages**  
- Written in **technical program language**  
- Lacked a clear starting point  
- Hard to use on mobile  
- Confusing for users with limited documentation knowledge  

The SSN Card Request Tool (affectionately called "the enumeration screener" by internal staff) was designed to **simplify the user's journey**, reduce confusion, and guide users step-by-step to the correct instructions for *their* situation.

I served as a **UX strategist, content designer, and flow architect**, shaping the logic, UI structure, and plain-language experience behind the tool.

---

# 1. The Call to Solve a Problem - Clarifying User Needs, Pain Points, and the Core Challenge

The original experience had several challenges, users often dealt with:

### a. Highly complex policy
Eligibility rules vary depending on:

- citizenship  
- age  
- name-change status  
- immigration category  
- presence of original or certified documents  
- location (inside the U.S. vs abroad)  

### b. Fragmented guidance creating confusion and stallled applications
SSA's documentation rules were scattered across inconsistent sources, including: 

- help pages created at different times with uneven updates, leaving users unsure which instructions to trust  
- outdated FAQs with contradicting rules  
- field-office exceptions that never surfaced online
- “sanitized” internal policy manuals (POMS) not designed for public use, but shared on the public site in ways that often confused users

  This “before” experience (see Figure 1) tried to answer everyone’s question of **“What documents do I need?”**—but failed to answer what **I**, the individual user, needed based on **my** situation. With generic, conflicting instructions and no clear call to action, users were left uncertain and overwhelmed, a major driver of application errors and repeat office visits.

### c. Broken user journeys that created avoidable strain on staff

Users frequently arrived at field offices:

- without the right documents  
- unsure which form they needed  
- confused about eligibility  
- misdirected for tasks they *could* do online  

### d. High-pressure moments that triggered a stress cycle for users and staff

Most users approached this task with real urgency. They needed a Social Security card so they could:

- start a new job  
- enroll a child in school  
- complete a housing application  
- receive benefits from a third party

That urgency elevated stress, and that stress made an already confusing experience feel even harder to navigate, increasing errors, repeat visits, and frustration. In turn, stressed and confused users put additional pressure on already overworked staff, creating a vicious cycle where unclear guidance amplified stress on both sides of the counter. 

We needed an experience that was:

- clear  
- mobile-first  
- personalized  
- low-literacy-friendly  
- policy-accurate  
- accessible  


![Stitched set of three mobile screenshots showing the previous Social Security Administration 'required documents' page as it appears on mobile, with dense text and minimal visual hierarchy.](/assets/images/ss5/what-docs-instructions.png){: .diagram } 

*Figure 1.: Before, users lacked a single, authoritative way to verify the documents they specifically needed.*

---

# 2. Gathering the Right Team - My Role, Collaboration Approach, and Cross-Functional Partnerships

### **Role: UX Strategist / Content Designer**

I led or co-led:

- Mapping the **full decision logic**  
- Translating policy into **user-friendly questions**  
- Designing wireframes and multi-step flows (See Figure 2)  
- Creating mobile-first UI patterns  
- Writing eligibility and result content  
- Ensuring design system and accessibility alignment  
- Collaborating closely with policy SMEs and operations teams

### Core collaborators:

- Policy experts (SSN/Enumeration)  
- UX researchers  
- Front-end developers  
- Spanish-language reviewers  
- Field office SMEs  
- Accessibility and design system contributors  

![Flowchart showing a high-level internal process for Social Security Card applications, indicating that all children must visit an office, and only U.S. citizens who can be verified electronically can file online.](/assets/images/ss5/multi-step-flow.png){: .diagram }

*Figure 2: High-level visualization of the user's Social Security card application flow.*

---

# 3. Navigating the Design Journey - End-to-End UX Process: Discovery, IA, Content Strategy, Prototyping, and Testing

## 3a. Discovery & Research

  We identified:

  - the *top reasons* people request an SSN card  
  - the *biggest user misunderstandings*  
  - the *most common failure points* in eligibility flows  

  Research methods:

  - Analytics review (search queries, task funnels)  
  - Interviews with field office staff  
  - Review of call-center logs  
  - Assessment of common user error cases  
  - Spanish-language comprehension feedback  
  - Comparative analysis of decision tools (DMV, USCIS, GOV.UK)  

  Key insights:

  - Users misunderstood what “original documents” meant  
  - Name-change workflows were deeply confusing  
  - Non-citizen pathways were unclear  
  - Living-abroad rules were hidden or inconsistent  
  - Users felt overwhelmed by dense information
  - Child-focused workflows needed to balance clear guidance for minors with strict compliance to federal (COPPA/CIPA) regulations. 



## 3b. Defining Logic & Requirements

  The tool required mapping **every possible user scenario**, including:

  - reason for request  
  - citizenship status  
  - location  
  - documentation availability  
  - special exceptions
  - state laws concerning electronic disclosure   

  We converted complex program logic into **user-centered logic**:

  I. Who are you?  
  II. Why do you need a card?  
  III. Where are you located?  
  IV. Do you have these documents?  
  V. What applies to your situation?  

This produced a streamlined decision-tree architecture.



## 3c. Design & Prototyping (Figma)

  Deliverables I created:

  - Wireframes for each decision step  
  - Mobile-first UI patterns  
  - Question and answer structures  
  - Document explainer components  
  - Results-page layout and content   
  - Reusable components integrated with the design system  

  UX principles used:

  - **One question per screen**  
  - **Plain language**  
  - **Contextual help** for documents  
  - **Progressive disclosure**  
  - **Error prevention through clarity**  
  - **WCAG AA+ accessibility**  



## 3d. Testing & Iteration

  We used:

  - Moderated usability sessions  
  - Comprehension testing  
  - Spanish-language QA  
  - Accessibility reviews  
  - Policy accuracy checks  
  - Error-case walkthroughs  

  Improvements made:

  - Simplified question wording  
  - Reordered steps based on user mental models  
  - Added clearer document descriptions  
  - Strengthened final next steps “Pause Point” instructions  
  - Improved readability and scannability  
  - Ensured parity across English and Spanish  

Testing confirmed major increases in clarity and task confidence.



## 3e. Delivery & Collaboration

I collaborated with:

- Developers (to convert logic to code)  
- Spanish reviewers (for linguistic parity)  
- Policy teams (for accuracy)  
- Operations teams (to confirm office readiness)  

We aligned on:

- Valid eligibility pathing  
- Content logic  
- Error-handling rules  
- UI patterns  
- Launch timing and review cycles  


---

# 4. Reaching the Breakthrough Moments - Key Insights, Usability Findings, Decisions, and Iterations

### Clarity & comprehension

I crafted the copy to match the terminology field offices use every day, ensuring users and staff were finally speaking the same language. (See Figure 4)

- Significant reduction in comprehension errors  
- Spanish-language comprehension improved due to rewritten structures   
- Name-change confusion dropped from **~60% → ~15%** in testing  

### Operational impact

- Fewer misdirected field office visits  
- Better-prepared users (correct documents on first attempt)  
- Reduced documentation confusion  
- Decreased “What do I need to bring?” call volume  

### User empowerment

Users reported:

- “finally knowing what I actually need”  
- “feeling less stressed”  
- “understanding what applies to me”

![Image showing five Pause Point examples for Social Security Card applications: one for users experiencing homelessness, two for users who must visit an office but should start online, one for users who can apply entirely online, and one for citizens living outside the U.S.](/assets/images/ss5/User_centric_instructions.png){: .diagram }

*Figure4: Examples of "Pause Points": strategically placed, user-specific prompts that increase the likelihood of resolving tasks during the initial interaction.*

---

# 5. Ripples Across the Organization - Outcomes, Impact Metrics, and Alignment to Agency Priorities

This project strengthened my ability to design:

- **multi-step, rules-based workflows**  
- **eligibility logic tools**  
- **guided decision experiences**  
- **back-office-optimized processes**  
- **compliance-aligned UI patterns**  

### Direct relevance to Institutional Services:

- Appian-style rule-driven workflows  
- Internal operational process mapping  
- High-clarity experiences for complex tasks  
- Cross-functional design alignment  
- System logic translated into user flows  

This project is a perfect example of designing experiences that work for users *and* meet strict regulatory and operational requirements.

---

# 6. Reflections and Future Direction - Summary, Lessons Learned, and Opportunities for Continued Improvement

The SSN Card Request Tool demonstrates how user-centered design can:

- simplify a highly complex task  
- reduce operational burden  
- improve accuracy  
- support multilingual access  
- increase clarity and user confidence  

Across research, design, logic mapping, testing, and delivery, I helped create an eligibility experience that is clearer, more accessible, and more efficient.

This is the type of workflow-heavy, mission-critical design work I’m passionate about.

---

[← Back to Design Stories]({{ site.baseurl }}/design-stories/)
