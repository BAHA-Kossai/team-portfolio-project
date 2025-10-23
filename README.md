# SE_Project_Team_portfolio

## Team Members:


- (Team Leader) Kossai BAHA **(BAHA-Kossai)**  [https://github.com/BAHA-Kossai]
- Abderahim KHEFIF **(Abderahim-14)** [https://github.com/Abderahim-14]
- Ahlem TOUBRINET **(Ahlem Toubrinet)** [https://github.com/AhlemToubrinet]
- Abdelaali HABBECHE **(ali-hbch)** [https://github.com/HabbecheAbdeaali]
- Malak Yasmine MEZIGHECHE **(malakneedshelp)** [https://github.com/malakneedshelp]
- Youssef TOUAHRIA MILIANI **(ystm256)**  [https://github.com/yousseftouahria]

## deployment source
https://baha-kossai.github.io/team-portfolio-project/


## Team Retrospective Analysis

The biggest technical problem our team faced during the project was dealing with **merge conflicts** and keeping our code up to date while using **Git** for version control. We worked with different branches such as **main**, **develop**, and several **feature/...** branches. This helped us work in parallel, but it also created issues when more than one team member edited the same files, especially **README.md** and **index.html**. These files were often changed to improve documentation and design, so conflicts happened frequently.  

---

### Example: Merge Issue

For example, one major issue occurred when we tried to merge the branch **feature/implement-Youssef-touahria-miliani** or **feature/implement-kossai-baha-profile** into **develop**.  
The problem started because the local version of the feature branch was not updated with the latest remote changes. When we tried to merge, Git showed an error saying the branch was behind.  

To fix this, we first used the command:  
`git fetch origin`  
to get the newest updates from the remote repository, then we ran:  
`git pull origin feature/implement-...`  
to make the local branch up to date. After that, we used:  
`git merge develop`  
to start the merge, but this caused conflicts in both **README.md** and **index.html**. These conflicts happened because some team members had edited the project description, while others had made changes to the web page layout.  

---

### Conflict Resolution

We solved the issue by carefully checking the differences, keeping the necessary parts from each version, and saving the corrected files.  
Then, we used:  
`git add README.md index.html`  
`git commit -m "Resolved merge conflicts in README and index.html"`  
`git push`  
to stage, commit, and send the updated version to the remote repository.  

Also, some other problems appeared when **Git considered two branches to have different histories**. This can happen when the branches were created separately or when their commit histories did not share a common ancestor.  

---

### Pull Request & Review Process

The **pull request and review process** also helped us a lot. Every pull request allowed the team to check the code and documentation before adding them to the main project. This teamwork helped find mistakes early, keep the project consistent, and improve communication. Even though this process sometimes slowed us down, it made our final web application **more stable, clearer, and of higher quality**.  
