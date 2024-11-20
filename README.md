[Dog Adoption Website]{.mark}

[Software Requirements Specification]{.mark}

[0.1]{.mark}

[10/07/24]{.mark}

[Team members:]{.mark}

[Simon Rosenberg]{.mark}

[Benjamin Schulz]{.mark}

[Caeden Francis]{.mark}

# [Revision History]{.mark}

  ------------------- -------------------------- --------------------- -----------------------
  **[Date]{.mark}**   **[Description]{.mark}**   **[Author]{.mark}**   **[Comments]{.mark}**

  [10/7/24]{.mark}    [0.1]{.mark}               [Simon                [\<First Revision,
                                                 Rosenberg]{.mark}     beginning
                                                                       project\>]{.mark}

                                                                       

                                                                       

                                                                       
  ------------------- -------------------------- --------------------- -----------------------

# Document Approval

The following Software Requirements Specification has been accepted and
approved by the following:

  ----------------- ----------------- ----------------- -----------------
  **Signature**     **Printed Name**  **Title**         **Date**

                    \<Your Name\>     Lead Software     
                                      Eng.              

                    A. David McKinnon Instructor, CptS  
                                      322               

                                                        
  ----------------- ----------------- ----------------- -----------------

**Table of Contents**

Revision History [ii](#revision-history)

Document Approval [ii](#document-approval)

1\. Introduction [1](#introduction)

1.1 Purpose [1](#purpose)

1.2 Scope [1](#scope)

1.3 Definitions, Acronyms, and Abbreviations
[1](#definitions-acronyms-and-abbreviations)

1.4 References [1](#references)

1.5 Overview [1](#overview)

2\. General Description [2](#general-description)

2.1 Product Perspective [2](#product-perspective)

2.2 Product Functions [2](#product-functions)

2.3 User Characteristics [2](#_Toc506458780)

2.4 General Constraints [2](#general-constraints)

2.5 Assumptions and Dependencies [2](#assumptions-and-dependencies)

3\. Specific Requirements [2](#specific-requirements)

3.1 External Interface Requirements
[3](#external-interface-requirements)

3.1.1 User Interfaces [3](#user-interfaces)

[3](#_Toc506459154)

3.2 Functional Requirements [3](#section)

[3](#_Toc506459157)

3.3 Use Cases [3](#use-cases)

3.3.1 Use Case #1 [3](#_Toc506459159)

[3](#_Toc506459160)

3.4 Classes / Objects [3](#classes-objects)

[3](#_Toc506459163)

3.5 Non-Functional Requirements [4](#non-functional-requirements)

3.5.1 Performance [4](#_Toc506459165)

3.5.2 Reliability [4](#_Toc506459166)

3.5.3 Availability [4](#_Toc506459167)

3.5.4 Security [4](#_Toc506459168)

3.5.5 Maintainability [4](#performance)

3.5.6 Portability [4](#portability)

3.6 Inverse Requirements [4](#inverse-requirements)

3.7 Design Constraints [4](#design-constraints)

3.8 Logical Database Requirements [4](#logical-database-requirements)

3.9 Other Requirements [4](#other-requirements)

4\. Analysis Models [4](#analysis-models)

4.1 Sequence Diagrams [5](#sequence-diagrams)

4.3 Data Flow Diagrams (DFD)
[5](#data-flow-diagrams-dfd-or-activity-diagrams)

4.2 State-Transition Diagrams (STD) [5](#state-transition-diagrams-std)

5\. Change Management Process [5](#change-management-process)

A. Appendices [5](#a.-appendices)

A.1 Appendix 1 [5](#a.1-appendix-1)

A.2 Appendix 2 [5](#a.2-appendix-2)

# 1. Introduction

The introduction to the Software Requirement Specification (SRS)
document should provide an overview of the complete SRS document. While
writing this document please remember that this document should contain
all of the information needed by a software engineer to adequately
design and implement the software product described by the requirements
listed in this document. (Note: the following subsection annotates are
largely taken from the IEEE Guide to SRS).

## 1.1 Purpose

*What is the purpose of this SRS and the (intended) audience for which
it is written?*

*This document outlines the software requirements for our adoption. It
allows us to make a clear path of our goals, constraints and
specifications/*

## 1.2 Scope

*This subsection should:*

*(1) Identify the software product(s) to be produced by name; for
example, Host DBMS, Report Generator, etc*

*(2) Explain what the software product(s) will, and, if necessary, will
not do*

*(3) Describe the application of the software being specified. As a
portion of this, it should:*

> *(a) Describe all relevant benefits, objectives, and goals as
> precisely as possible. For example, to say that one goal is to provide
> effective reporting capabilities is not as good as saying
> parameter-driven, user-definable reports with a 2 h turnaround and
> on-line entry of user parameters.*
>
> *(b) Be consistent with similar statements in higher-level
> specifications (for example, the System Requirement Specification) ,
> if they exist.What is the scope of this software product.*
>
> *The software product is a web-based dog adoption service that
> simplifies the adoption process. The platform will allow users to
> browse animals, submit adoption applications, and communicate with the
> shelter*

## 1.3 Definitions, Acronyms, and Abbreviations

*This subsection should provide the definitions of all terms, acronyms,
and abbreviations required to properly interpret the SRS. This
information may be provided by reference to one or more appendixes in
the SRS or by reference to other documents.*

*SRS: Software Requirements Specification*

*UI: User Interface*

*DBMS: Database Management System*

## 1.4 References

*This subsection should:*

*(1) Provide a complete list of all documents referenced elsewhere in
the SRS, or in a separate, specified document.*

*(2) Identify each document by title, report number - if applicable -
date, and publishing organization.*

*(3) Specify the sources from which the references can be obtained.*

*This information may be provided by reference to an appendix or to
another document.*

*IEEE Guide to SRS*

*ASP.NET Core Blazor Documentaiton*

## 1.5 Overview

*This subsection should:*

*(1) Describe what the rest of the SRS contains*

*(2) Explain how the SRS is organized.*

*This document covers the project scope, requirements, and analysis of
models needed for the dog adoption website.*

# 2. General Description

*This section of the SRS should describe the general factors that affect
\'the product and its requirements. It should be made clear that this
section does not state specific requirements; it only makes those
requirements easier to understand.*

## 2.1 Product Perspective

## *This subsection of the SRS puts the product into perspective with other related products or*

*projects. (See the IEEE Guide to SRS for more details).*

*This platform will integrate with an animal shelter and provide a
user-friendly interface for adopters.*

## 2.2 Product Functions

This subsection of the SRS should provide a summary of the functions
that the software will perform. []{#_Toc506458780 .anchor}

The system will allow users to:

Register and manage accounts

Browse adoptable dogs with filters (age, breed, etc.)

Submit adoption applications

2.3 User Characteristics

This subsection of the SRS should describe those general characteristics
of the eventual users of the product that will affect the specific
requirements. (See the IEEE Guide to SRS for more details).

The typical users will include:

-   Potential dog adopters

-   Animal shelter staff managing the listings

## 2.4 General Constraints

*This subsection of the SRS should provide a general description of any
other items that will*

*limit the developer's options for designing the system. (See the IEEE
Guide to SRS for a partial list of possible general constraints).*

* The system must be web-based*

* The system must adhere to GDPR regulations for data protection*

## 2.5 Assumptions and Dependencies

This subsection of the SRS should list each of the factors that affect
the requirements stated in the SRS. These factors are not design
constraints on the software but are, rather, any changes to them that
can affect the requirements in the SRS. For example, an assumption might
be that a specific operating system will be available on the hardware
designated for the software product. If, in fact, the operating system
is not available, the SRS would then have to change accordingly.

 The system must be web-based

 The system must adhere to GDPR regulations for data protection

# 3. Specific Requirements

This will be the largest and most important section of the SRS. The
customer requirements will be embodied within Section 2, but this
section will give the D-requirements that are used to guide the
project's software design, implementation, and testing.

Each requirement in this section should be:

-   Correct

-   Traceable (both forward and backward to prior/future artifacts)

-   Unambiguous

-   Verifiable (i.e., testable)

-   Prioritized (with respect to importance and/or stability)

-   Complete

-   Consistent

-   Uniquely identifiable (usually via numbering like 3.4.5.6)

Attention should be paid to the carefuly organize the requirements
presented in this section so that they may easily accessed and
understood. Furthermore, this SRS is not the software design document,
therefore one should avoid the tendency to over-constrain (and therefore
design) the software project within this SRS.

**[ADD TABLE]{.mark}**

**[For Example:]{.mark}**

![](./image1.png)

## 3.1 External Interface Requirements

### 3.1.1 User Interfaces

## 

## 

## 3.2 Functional Requirements

**[ADD TABLE - For every requirement, identify Input, Output,
Limitations, and Error messages.]{.mark}**

+-------+--------------------------------------------------------+-----+
| Ident | Requirement                                            | Use |
| ifier |                                                        | C   |
|       |                                                        | ase |
+=======+========================================================+=====+
| REQ1  | Register a new User                                    | U   |
|       |                                                        | C-1 |
|       | Any person can create a registered customer account    |     |
|       | ....                                                   |     |
|       |                                                        |     |
|       | ...................................                    |     |
+-------+--------------------------------------------------------+-----+
| REQ2  | Login                                                  | U   |
|       |                                                        | C - |
|       | The system must allow registered customers to log in   | 2   |
|       | to their accounts by entering their username and       |     |
|       | password.                                              |     |
|       |                                                        |     |
|       | The system must allow customers to reset their         |     |
|       | password by clicking \"I forgot my password\" and      |     |
|       | receiving a link to their verified email address.      |     |
|       |                                                        |     |
|       | Username should include:                               |     |
|       |                                                        |     |
|       | -   The username must be at least ten characters long. |     |
|       |                                                        |     |
|       | -   Use letters (a-z), letters (A-Z), numbers (0-9),   |     |
|       |     and underscore( \_ ) or ( @) characters.           |     |
|       |                                                        |     |
|       | The password should include:                           |     |
|       |                                                        |     |
|       | -   The password must be at least ten characters long. |     |
|       |                                                        |     |
|       | -   Use the mix of letters (a-z), letters (A-Z),       |     |
|       |     numbers (0-9), and special characters.             |     |
|       |                                                        |     |
|       | If the registered customers cannot provide a valid     |     |
|       | name and password, display the error message: "        |     |
|       | Invalid user name or password."                        |     |
+-------+--------------------------------------------------------+-----+
| REQ3  | Filter dogs by breed, size, and location               | U   |
|       |                                                        | C-3 |
+-------+--------------------------------------------------------+-----+
|       |                                                        |     |
+-------+--------------------------------------------------------+-----+
|       |                                                        |     |
+-------+--------------------------------------------------------+-----+

## 3.3 Use Cases

**[Add System Use Case]{.mark}.** For Example - see page 39, SRS Parking
Garage Automation Example.

**[Add the 3 Use Case Descriptions: Login, Registration, and Adopt a
Dog.]{.mark}**

**3.3.1 Use Case #1: Login**

-   **Use Case Name: Login**

-   **Primary Actor: Registered User**

-   **Stakeholders and Interests:**

    -   **Registered User: Wants to log in to access the system and view
        or update their profile, submit adoption applications, or manage
        adopted pets.**

    -   **System: Must authenticate the user's credentials to provide
        access to the system's functionality.**

-   **Preconditions:**

    -   **The user must have an existing registered account.**

    -   **The system must be online and functional.**

-   **Trigger:**

    -   **The user navigates to the login page and inputs their
        credentials (username and password).**

-   **Main Success Scenario:**

    1.  **The user navigates to the login page.**

    2.  **The user enters their username and password.**

    3.  **The system validates the credentials.**

    4.  **The system grants access to the user's account and redirects
        to the user's dashboard.**

-   **Extensions:\
    3a. Invalid credentials:**

    -   **The system displays an error message: \"Invalid username or
        password.\"**

    -   **The user is prompted to try again or click \"Forgot Password\"
        to reset credentials.**

-   **Postconditions:**

    -   **The user is logged in and can now access their account and
        features available to logged-in users.**

**3.3.2 Use Case #2: Registration**

-   **Use Case Name: Registration**

-   **Primary Actor: New User**

-   **Stakeholders and Interests:**

    -   **New User: Wants to create a new account in order to adopt pets
        or manage personal details.**

    -   **System: Must capture the required information and create a
        unique user profile for new users.**

-   **Preconditions:**

    -   **The user must have access to the registration page.**

    -   **The system must be online and ready to accept new user
        registrations.**

-   **Trigger:**

    -   **The user navigates to the registration page to create a new
        account.**

-   **Main Success Scenario:**

    1.  **The user navigates to the registration page.**

    2.  **The user fills in required details, including username,
        password, email, and personal information.**

    3.  **The system verifies that all required fields are filled and
        the information is valid.**

    4.  **The system creates a new user profile and sends a confirmation
        email to the user.**

    5.  **The user receives confirmation and is logged in automatically
        or prompted to log in.**

-   **Extensions:\
    3a. Invalid or incomplete information:**

    -   **The system displays an error message indicating which fields
        need to be corrected or filled.**

    -   **The user corrects the information and resubmits.**

-   **Postconditions:**

    -   **The system creates a new user account, and the user can now
        log in to the system.**

**3.3.3 Use Case #3: Adopt a Dog**

-   **Use Case Name: Adopt a Dog**

-   **Primary Actor: Registered User**

-   **Stakeholders and Interests:**

    -   **Registered User: Wants to adopt a dog by submitting an
        adoption application for a selected pet.**

    -   **Shelter Staff: Needs to manage and approve adoption
        applications, ensuring that each pet is adopted by a responsible
        and eligible user.**

-   **Preconditions:**

    -   **The user must be logged into the system.**

    -   **The user must have already completed the registration
        process.**

-   **Trigger:**

    -   **The user selects a dog from the available listings and begins
        the adoption process by clicking \"Adopt.\"**

-   **Main Success Scenario:**

    1.  **The user searches and selects a dog from the listings.**

    2.  **The user clicks on the \"Adopt\" button on the dog's profile
        page.**

    3.  **The system displays the adoption application form.**

    4.  **The user fills out and submits the application form with
        personal details and adoption preferences.**

    5.  **The system validates the application and sends it to shelter
        staff for review.**

    6.  **The shelter staff reviews the application and either approves
        or denies it.**

    7.  **If approved, the system notifies the user and provides further
        instructions for completing the adoption.**

-   **Extensions:\
    5a. Incomplete application:**

    -   **The system prompts the user to complete the missing fields.**

    -   **The user resubmits the application.**

**6a. Application denial:**

-   **The shelter staff denies the application.**

-   **The system notifies the user with the reason for denial and
    provides the option to apply for another dog.**

```{=html}
<!-- -->
```
-   **Postconditions:**

    -   **If approved, the user receives instructions to finalize the
        adoption process.**

    -   **If denied, the user is notified with details and may reapply
        for another pet.**

## 3.4 Classes / Objects

[Add Domain class diagram. **For every class**, provide the class **Name
and Attributes**]{.mark}**. Do not add functions.**

**Class Name: User**

**Attributes: username, password, email**

![](./image2.png)

## 3.5 Non-Functional Requirements

Non-functional requirements may exist for the following attributes.
Often these requirements must be achieved at a system-wide level rather
than at a unit level. State the requirements in the following sections
in measurable terms (e.g., 95% of transaction shall be processed in less
than a second, system downtime may not exceed 1 minute per day, \> 30
day MTBF value, etc).

### 3.5.1 Performance 

### 95% of actions should complete in under 2 seconds.

### 3.5.2 Reliability 

### The system must have an uptime of 99.5%.

### 3.5.3 Availability 

### The system must be available 24/7.

### 3.5.4 Security 

### User data must be encrypted during transmission.

### 3.5.5 Maintainability

### 3.5.6 Portability

## 3.6 Inverse Requirements

State any \*useful\* inverse requirements.

The system should not store any sensitive financial information.

## 3.7 Design Constraints

Specify design constrains imposed by other standards, company policies,
hardware limitation, etc. that will impact this software project.

The system must follow HTML5, CSS3 standards.

## 3.8 Logical Database Requirements

Will a database be used? If so, what logical requirements exist for data
formats, storage capabilities, data retention, data integrity, etc.

The database must store user data, dog listings, and adoption
applications.

## 3.9 Other Requirements

Catchall section for any additional requirements.

# 4. Analysis Models

List all analysis models used in developing specific requirements
previously given in this SRS. Each model should include an introduction
and a narrative description. Furthermore, each model should be traceable
the SRS's requirements.

## 4.1 Sequence Diagrams

## 4.3 Data Flow Diagrams (DFD) or Activity diagrams 

**[Submit two Activity Diagrams for the "Login" and "Adopt a Dog"
functions.]{.mark}**

![](./image3.png)

## 4.2 State-Transition Diagrams (STD)

# 5. Change Management Process

Identify and describe the process that will be used to update the SRS,
as needed, when project scope or requirements change. Who can submit
changes and by what means, and how will these changes be approved.

# A. Appendices

Appendices may be used to provide additional (and hopefully helpful)
information. If present, the SRS should explicitly state whether the
information contained within an appendix is to be considered as a part
of the SRS's overall set of requirements.

*Example Appendices could include (initial) conceptual documents for the
software project, marketing materials, minutes of meetings with the
customer(s), etc.*

## A.1 Appendix 1

## A.2 Appendix 2
