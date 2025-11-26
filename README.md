# Case 1. Academic Profile: A Scientist's Digital Footprint

## Background
The Sirius University is rapidly expanding, attracting talented students, scientists, tutors, and researchers with diverse competencies and scientific interests. The growing number of students and staff creates new organizational challenges: it is difficult to quickly assess the achievements of individual researchers, form teams, and encourage collaborative research. To effectively manage the team and foster the development of interdisciplinary research, we need a platform that unites all members of the university community and allows for objective tracking of each specialist's scientific productivity and impact.

**Goal:** To create an intelligent service for the automated collection, systematization, and visualization of publication activity for the university's staff, students, and postgraduate students.

## Core Functional Requirements

1. **Automated data collection** on publications by the university's staff, students, and postgraduate students from various abstract and bibliographic databases, digital archives (Google Scholar, Scopus, Web of Science, RSCI, MathSciNet, PubMed, arXiv.org, Crossref). This should utilize page parsing/open APIs.
2. **Analysis of individual key metrics** for publication authors (citation impact, h-index, affiliation, authorship contribution).
3. **The ability to manually edit author profiles** (.xls, .csv). When using Django, configure editing via Django Admin (using a local administrator).
4. **Construction of a knowledge graph** and search for communities within it by research areas, disciplines, and staff.
5. **Generating recommendations** for potential collaborative research within the university.

## Work Plan

### Checkpoint 1: Author Profile Generation
- **Goal:** To demonstrate the capability of forming an author profile.
- **Expected Outcome:** 
  - A REST API with Swagger documentation for core CRUD operations related to the author profile is implemented.
  - The description of methods and received/returned attributes is provided, including sample test data.
  - Preliminary interface mock-ups and main system screens are prepared.
  - The type of ML model is selected, and the data processing method using the chosen ML model is developed.

### Checkpoint 2: Graphical User Interface for Forming Author (Research Group) Profiles
- **Goal:** To develop an interface for collecting, analysing, and visualising key metrics of authors (a research group).
- **Expected Outcome:**
  - Periodic mechanisms (e.g., with a monthly interval) for data collection, processing, and storage are implemented.
  - An ML model is created. The model is trained on a limited set of collected data.
  - The API interface is configured and capable of providing processed data for further visualisation and analysis.
  - Initial datasets on publications of specific scientists (a research group) are obtained.

### Checkpoint 3: Development of the User Interface and Related Components
- **Goal:** Prototyping the user interface and its integration with the system's internal implementation.
- **Expected Outcome:**
  - A ready-made solution demonstrating the core functionality.
  - Visual interface elements are refined for user-friendly navigation and perception.
  - Detailed information about each scientist is displayed, including publication history, cited articles, and general indicators of scientific productivity.
  - A recommendation system for forming interdisciplinary research teams within the university is proposed.
  - Project documentation with a description of the launch process is prepared.
  - The project is launched using Docker.

---

### Rules:
- **At the time of the start of development, share the project's git repository with experts.**
- **Upload the code and presentation to your git before stop-coding.**
- **Provide the code with a brief description of how to deploy the proposed solution.**
