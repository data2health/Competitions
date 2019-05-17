# Budget
Don't edit this - the RPPR generater populates this section

# Research Design
A platform to support robust peer review within and across CTSA hubs does not currently exist. Competitions is a software tool for investigators, reviewers and administrators to solicit and review various types of competitions; this include pilot projects, research awards and their peer review. Here, we will upgrade Competitions platform (1) to support CTSA consortium-wide peer-review activities through a cloud-deployment that supports single sign-on and (2) to work on the competitions code base to enhance the ease and robustness of its adoption by interested institutions.

# Methodology
The Competitions team is part of the larger ARIG Group at Northwestern University. The team runs a version of the Agile methodology to plan work incrementally, paired with continuous feedback, integration, and testing to drive forward progress of this project. We run bi-weekly sprints, with daily stand-ups where team members can call out blockers and dependencies. 

**Software upgrades:** The Competitions code itself has been in production for around 5 year with only incremental bug fixes and peacemeal feature requests. THis project is an opportunity to upgrade the underlying Ruby on Rails (RoR) framework to a contemporaneous version. We will also redesign some of the public and participant facing using interfaces as well as the authentication workflow to support the broader use case (beyond NU). We will also integrate a RoR Gem for utilizating SAML-based SSO authentication.

**Cloud Work:** The architeture of the application is predicated on a classic stack: web server, database server, file system. We will utilize this project opportunity to package this software in a manner that can rely on cloud-based application provisioning. For example, documents and other digital assets can be stored as Amazon S3 objects within an abstraction layer that is invisible to the rest of the application. The work done to identify the best practices for doing so can be reused by subsequent applications that would utilize CDH2/NCATS cloud infrastructure or components.

**Testing:** The ethos of our agile development methodology is to present a minimally viable instance as early as we can and then to engage the users in iterative refinement. We plan to solicit direct feedback via demos and provisioning for users so they can inform the subsequent tightly coupled development sprints throughout the rest of the project timeline. 

# Expected Outcomes
A functioning prototype of a CTSA Program-level competition review tool for projects and events that can be used in the cloud or implemented locally, if desired. This entails the availability of the following:  

- Public GitHub repo where software can be downloaded, features requested, etc.
- A publicly available cloud-hosted instance that supports SSO user authentication, user-created competitions, user-submitted proposals, and user review.
- Engagement/support materials and activities, including documentation for interested adopters.
- Roadmap for next phase of work, including incorporation of expertise work such as CEREC.

# Timeline 
Broadly, the goal of this project is to provide a minimally viable cloud-based product by September 30, 2019 for initial presentation to and review by the CTSA community. We envision a 6-month tail after that dedicated to UAT and feedback; hands-on demonstration; on-boarding (including institutional on-boarding to the NCATS SSO platform); and development of multi-modality educational artifacts. 

Milestone: A functioning prototype of a CTSA Program-level competition review tool for projects and events that can be used in the cloud or implemented locally, if desired. 

This translates to the following timeline:

- Public GitHub repo where software can be downloaded, features requested, etc. 
    - Available at end of Q1 (June); expand through Q4
- A publicly available cloud-hosted instance that supports SSO user authentication, user-created competitions, user-submitted proposals, and user review. 
    - Available at end of Q2 (Sept)- CTSA Fall Meeting; expand through onboarding, enhancements through Q4 (March)
- Publicly shared requirements-gathering and testing results of cloud deployment
    - Available at end of Q2 (Sept); expand through Q4 (March)
- Engagement/support materials and activities, including documentation for interested adopters.
    - Available at end of Q2 (Sept); expand through Q4 (March)
- Roadmap for next phase of work, including incorporation of expertise work such as CEREC.


# Potential Pitfalls and Alternative Strategies

Since this is a mature application, we anticipate most of our pitfalls to be contained to the following components: (1) cloud deployment including SSO authentication; (2) unforeseen user needs that arise from the broader context of the CTSA-wide scope. We plan to mitigate the former by engaging the NCATS cloud team as early as possible and to mitigate the latter via the long tail of user acceptance testing coupled with frequent short development / deployment cycles in the second half of our timeline.
