# Project-management-standard

## Introduction to Project Management
Project management is defined as the process of keeping track of the many inputs and outputs of a project from experimental design through publication.

### The main components of project management include but may not be limited to:
1. Folders and Files
2. Notebook record of commands, thought process and related code
3. Communication and Discussion
4. ToDo list
5. Record of your time spent

#### 1. Folders and Files
Most people use folders to organize their files regardless of operating system (Windows, IOS, Linux). A small change to how folders are labeled can significantly improve the ability for others to follow what you did, the order you did it in and where you did it.

**Number folders in order of their creation**

Prepend the descriptive folder name that you usually create with a number starting with 00*, followed by 01*, 02*, 03* and so forth like so:

- Project folder
  - 00_RawData
  - 01_AnalysisStepOne
  - 02_AnalysisStepTwo
  - 03_AnalysisStepThree

The extra 0 from 00 - 09 keeps the folders in numerical order when executing the list `ls` command. The you in 6 months or the next person on the project will thank you as it is easy to numerically follow the steps based on the folder number and the date the folder was generated `ls -lha`.

The name of your project folder should be descriptive of the project, for example, WhiteAbaloneRNA-Seq or SeriolaGWAS.

#### 2. Notebook

Science isn’t reproducible if it isn’t recorded. Traditionally, paper notebooks have been used in the wet lab to record the science performed that day and the outcome. In bioinformatics, science is recorded digitally in a digital notebook. We recommend using GitHub as your digital notebook.

This last step is important as it is a discrete block of notes that is the smallest unit of replicable notes in your notebook. The Why, How and Result can be replicated multiple times if it is the same day in the same folder.
**GitHub**

GitHub is often thought of as a tool for programmers to version control code but it can also be used to version control text documents as an online notebook. If you don’t have a GitHub account, you can set one up based on this [GitHub Tutorial](https://bioinformaticsworkbook.org/Appendix/github/introgithub.html) and the free version of GitHub now allows for unlimited free repositories. In addition, as a researcher or educator you can request a free upgrade to get access to [unlimited users in private repos.](https://help.github.com/articles/about-github-education-for-educators-and-researchers/).

One of the great aspects of GitHub is that you can use [markdown](https://bioinformaticsworkbook.org/Appendix/Markdown.html) syntax to very quickly format your notebook. For example, This tutorial is written in markdown and you can make headers`# ## ###`, bullet points `*`, code blocks and insert images very easily. Markdown can also be easily converted to PDF for sharing.

Assuming you now have a GitHub account, create a GitHub repository with the same name you labeled your project folder (ie: WhiteAbaloneRNA-Seq or SeriolaGWAS).

Here is the first integration between project components.

**For every subfolder create a markdown file**

For every subfolder you make in your project folder on your remote machine or computer, create a markdown file in your GitHub repository.

- Notebook_LastName
  - 00_RawData.md
  - 01_AnalysisStepOne.md
  - 02_AnalysisStepTwo.md
  - 03_AnalysisStepThree.md

After you git clone your repo you can create a folder named Notebook_LastName and then add markdown files corresponding to each new subfolder you add during the analysis pipeline.

If you work on multiple machines and your laptop then create a folder for each machine.

- Notebook_LastName
  - remote machine
    - 00_RawData.md
    - 01_AnalysisStepOne.md
    - 02_AnalysisStepTwo.md
    - 03_AnalysisStepThree.md
  - laptop
    - 01_AnalysisStepOne.md
    - 02_AnalysisStepTwo.md

#### What, When, Where, Why, How and the Result

For every step you perform bioinformatically, record it in your markdown file along with

- Title
- Date
- Computername and path of working directory
- Description of what you are trying to do and why
- Code block of the commands you used
- Description of the result

#### 3. Communication and Discussion

In a group with multiple active projects, it is helpful to have a running dialogue of progress and discussion for each project that can be easily referred to and searched. Many times this comes in the form of email exchanges.

**Slack**

However, a communication platform based around group chats can also be extremely effective when you have a medium sized group (3+) of knowledgeable individuals. We use

[Slack](https://bioinformaticsworkbook.org/Appendix/slack.html) and create a channel for each active project. This group chat (text messaging style) communication generates a transcript of conversations about projects that you can go back and reread. It also permits, text, images and files to be attached during conversation. I strongly encourage you to use it primarily for text communication and discussion and not for file storage.

You can create your own team using [this link: Team signup](https://slack.com/r/0mklqxar-0tnh0jhj) and get a $100 credit if you decide to purchase it beyond the free version. The upgraded version will let you search beyond the 10,000 most recent messages in your group and there is a steep academic discount.

**OneNote**

Microsoft Onenote has the ability to create notebooks, tabs and pages. This can be done on your laptop or tablet using a pen. Both will result in a significant reduction in your paper usage. In addition you will have a well organized record of every in person meeting you have with a student or colleague on a particular project.

- Meetings Notebook
  - ProjectName Tab
    - Meeting date1 page
    - Meeting date2 page
    - Meeting date3 page
  - ProjectName2 Tab
    - Meeting date1 page
    - Meeting date2 page
    - Meeting date3 page

Since the Genome Informatics Facility works on multiple projects with multiple PIs, we use the PI name for the project name tab. Within a lab group you may have a folder for every person in your group.

#### 4. To-Do Lists

Use a Kanban board. Kanban boards can be thought of as a 2D To-Do list. Take a whiteboard and section it into 6 columns. (There is a digital equivalent that I will provide you below so don’t actually do this with a real whiteboard)

- New tasks
- IceBox
- Backlog
- In progress
- In review
- Completed

Take a post-it note and write down the task you need to do and everything you need to know about how to do it. Repeat for every task you have. Place all post-it notes into the `New tasks` column on your whiteboard.

Now that all the tasks are on the whiteboard, separate out those tasks that are higher priority from those that are lower priority and place them into `In Progress` and `Backlog`, respectively.

The `Icebox` column is for those ideas that are rumbling around in your head that are really cool and you don’t want to forget but don’t have time for right now. Write down that idea/task and put it in the `Icebox` column for when you do have time and get it out of your head.

Now prioritize the tasks in `In Progress` and `Backlog` columns by placing the most important tasks at the top of the column.

When you complete a task move it to `In review` or `Completed` columns.

Cool idea right? But a real-life whiteboard and post-it notes would be very time consuming so we use a digital whiteboard.

[Zenhub](https://www.zenhub.com/pricing) is free for public, personal, and academic repositories and the chrome or firefox plugin can be downloaded [from here](https://www.zenhub.com/extension). It uses the issues in a github repository. So now you can for every project have a Kanban board for all tasks related to that project. If you have more than one project it may be helpful to create a separate private repository just for your todo lists on several projects.

#### 5. Record of time spent

Bioinformatics projects can be time consuming and frustrating with a lot of trial and error. It often happens that at the end of a week, it doesn’t feel like anything was accomplished. Keeping track of your time spent on a daily basis can bring peace of mind. This can be easily accomplished using a Google spreadsheet with days of the month at the top as columns and project names as rows on the left. For each project there should be two rows; hours spent and description of what you did. The column widths can be relatively short since hours spent in a day is not more than 2 digits and the description can just flow into adjacent cells. It is also helpful to see where your time is being spent and better manage your work/life balance and provide a tool for those in your group to manage their work/life balance.

> [Project Management](https://bioinformaticsworkbook.org/projectManagement/Intro_projectManagement)
