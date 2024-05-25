# PortalPeek

PortalPeek is a long unawaited project of mine that I have thought throughout my spring 2024 semester. However, due to time constraints, I was unable to implement it. Now that I have some time off college, I am starting out on implementing it. I will explain the motivations and requirements behind this project.

## Motivation

Most of the schools have their own intranet or a portal for announcements or news going on in the school. This can be anything like a research participation announcement, extracurricular activities, job postings, career opportunities, and many more. Most of the time, I do not (and I assume most of the students) open the portal. I certainly don't open it everyday which means I am going to miss most of the announcements and opportunities.

##### **What if all of those announcements come in my email itself everyday so that I can be up to date regarding all of the news and opportunities on campus.**

This is the aim of this Project **PortalPeek**. It allows students to receive all the news on the student portal to the email itself. This will not make my miss any announcements, opportunities, job postings or anything important to me.

## Implementation Details

### Overview

PortalPeek will be implemented as a web-based service that automatically scrapes the student portal for new content, processes the data, and sends it as an email digest to all subscribed users. The following sections detail the technical architecture, features, and tools used in the project.

### Technical Architecture

1. Web Scraping Module:

    - Technology: Python with BeautifulSoup and Requests.
    - Function: Logs into the student portal, scrapes new announcements, and extracts relevant information.

2. Database:

    - Technology: PostgreSQL.
    - Function: Stores user information, subscription preferences, and a cache of the portal's announcements.

3. Email Notification System:

    - Technology: Python with smtplib or an email service like SendGrid.
    - Function: Sends out daily email updates to all subscribed users.

4. User Interface:

    - Technology: Flask for the backend, HTML/CSS/JavaScript for the frontend.
    - Function: Allows new users to register, log in, and manage their subscription preferences.

## Detailed Implementation Plan

Below is a detailed Step by Step plan for the implementation of the project. The steps will be timestamped in the document itself to track my progress and be true to the progres of the project. Below is a step by step implementation.

### Step 1 : Requirements Gathering and Planning

1. Objective
    - Scrap the Student Portal of my college, and send daily updates via email.

2. Necessary Features
    - User Registration
        - User should be able validated (through the school email address), and they should be able to update their preferences ( being able to subscribe or unsubscribe to the email).
    - Database
        - Database should store user information as well as the scrapped data from the website.
    - Email delivery
        - Email should be delivered to the subscribed users. It should be clearly formatted and should include all of the announcements.
    - Scraping
        - A scraping module should be able to scrape the student portal. It should be able to authenticate itself, and scrape the portal.

    A place where additional technologies can be included is the use of LLM's to get context from the announcements to generate short summaries of the announcements. It can be used as the subject for the daily emails. It can also categorize announcements. For example : announcements could be general, regarding jobs, graduate schools, events on campus, or miscellaneous. This is where a LLM can come in.

3. Setting Project deadlines and goals.

    | Project Goal | Description | Deadline
    ----- | ----------- | --------
    Database Design | Define Data Models and integrate with your program using ORM tools | May 30th 2024.
    Backend Implementation | Setup Backend and API's if required to store scraped data and user information. Set up mail service in the backend to send regular emails. | June 15th 2024.
    Frontend Implementation | Implement frontend to validate user account and also manage user preferences for the service | June 30th 2024.
    Scraping Module | Implement scraping module for scraping the website. Most likely use beautifulsoup or selenium for performing the automation. | July 15th.
    Testing and Integration | Perform unit tests and integration tests on the project to ensure that it it working as expected and cover all the edge cases. | July 30th.
    Deployment | 


### Step 2 : Database Design




### Step 3 : Backend Implementation

Backend will be implemented using the Django Framework. 