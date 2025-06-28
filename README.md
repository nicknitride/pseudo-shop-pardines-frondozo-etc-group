# Project Retrospective

**Date:** June 28, 2025
**Team:** Ivan Frondozo, Jaime Manalo, Nicholo Pardines, Paolo Flores, Johnvee Mandal
**Project:** FECP5 Final Exercise - Pseudo Shop

This document summarizes the team's experience, challenges, and learnings during the development of the Pseudo Shop project.

### 1. How did your team divide the work?

We adopted a **feature-branch workflow**. Each of the four developers was responsible for a specific feature, and **Johnvee Mandal** acted as our **Project Manager**. His role was crucial in acting as a communication bridge, helping to coordinate the integration of different features, and guiding the resolution process when conflicts emerged.

The work was divided as follows:

* **Feature 1 (Filtering):** Ivan (`ivanp-frondozo`)
    * `store_view.pseudo`
    * `product_model.pseudo`
* **Feature 2 (User Auth):** Jaime Manalo (`mnljm`)
    * `user_controller.pseudo` (This feature was developed in isolation, which successfully prevented merge conflicts with the product-related features).
* **Feature 3 (Product Creation):** Nicholo Pardines
    * `product_model.pseudo`
    * `store_view.pseudo`
* **Feature 4 (Storefront & Display):** Paolo Flores (`paolofloress44`)
    * `store_view.pseudo`
    * `product_model.pseudo`

### 2. What Git commands or workflows were most useful to you?

* **Workflow:** The **feature branching strategy** was fundamental to our process. It allowed for parallel development while keeping the `main` branch stable. We used a consolidation branch (`feat/filter-products`) to integrate related features before the final merge to `main`.

* **Commands:** The following Git commands were essential to our daily workflow:
    * `git commit`: For saving incremental progress with clear, descriptive messages.
    * `git merge`: For integrating completed feature branches.
    * `git log --graph --oneline`: For visualizing branch history and understanding the sequence of commits.
    * `git diff`: For reviewing changes and analyzing merge conflicts.

### 3. Describe the merge conflict your team encountered. What caused it and how did you resolve it?

We encountered a merge conflict when merging `feat/storefront_layout_and_display_logic` into our integration branch, `feat/filter-products`.

* **Conflicted Files:**
    * `product_model.pseudo`
    * `store_view.pseudo`
* **Cause of the Conflict:**
    The conflict was caused by developers on both branches making changes to the same lines of code in shared files. One branch added new sample product data while the other implemented a database upload function in the same location.
* **Resolution:**
    We resolved the conflict manually using VS Code's tools. The team discussed the necessary changes, decided to **accept both changes**, and integrated them to ensure the code was functional before committing the merge resolution.

### 4. What were the biggest challenges during this activity?

Our main challenge was **asynchronous communication**. Working at different times led to minor inconsistencies in variable naming and assumptions about function outputs, which required extra time to resolve during integration.

### 5. What did you learn about using Git in a team setting?

This project reinforced the importance of a **disciplined Git workflow** and **proactive conflict management**. A deep understanding of which files are affected by each feature is crucial for anticipating and minimizing merge conflicts.

### 6. How would you improve your workflow in future projects?

Based on the challenges we faced, we would implement the following improvements:

* **Establish a Strict Coding Standard:** Agree on and document guidelines for naming, style, and structure before coding begins.
* **Define API Contracts Early:** For interacting features, define function signatures and data structures in advance.
* **Enhance Communication Protocols:** Schedule brief, regular check-ins to increase awareness of potential work overlap.
* **Mandatory Pull Request (PR) Reviews:** Enforce code reviews to catch inconsistencies and share knowledge before merging.