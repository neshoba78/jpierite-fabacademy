# Project Management

#### Have you:

* [x] made a website and described how you did it

* [x] introduced yourself

* [x] documented steps for uploading files to archive

* [x] pushed to the class archive

In a previous life, I was an Internet Marketing Specialist for Mohegan Sun in Uncasville, CT. I helped manage six of their company websites using proprietary content managements systems and flat HTML. I got comfortable with working first with a local copy and pushing content to a server that was scheduled to cache every four hours.

These are some of the websites that I worked on:

[Mohegan Sun](https://mohegansun.com/)

[Mohegan Sun Pocono Downs](https://mohegansunpocono.com/)

[Mohegan Tribal Gaming Authority](http://newsroom.mtga.com/)

[The Fab Foundation](http://www.fabfoundation.org/)

[FAB11](http://fab11.fabevent.org/)

I started class work for [Fab Academy in 2015](http://fabacademy.org/archives/2015/na/students/pierite.jean-luc/old-site/index.html). Back then, we used Mercurial for version control. Repositories were divided by region. Continuing my work after FAB12 with Fab Lab Wgtn, I started to work in the git repository under a network folder with a very binary student ID.

![](/assets/Screen Shot 2016-09-12 at 7.02.15 PM.png)

Originally, I built my website with a local copy of Wordpress. I triple booted my work computer, “Mama Rosie”, and installed the CMS on an Ubuntu partition. As I made updates to my website, I mirrored it with httrack to make flat HTML files. This was a workflow that I used through Fab Academy 2015 and 2016.

As part of my job deploying fab lab inventory to new fab lab installations, I work out standard procedures for dual or triple booting computers and installing all the necessary freeware. Recently, we started to get requests for computers with Windows 10. Dual booting these machines wasn't working out too well. There was an issue with Ubuntu corrupting wireless networking drivers on the Windows side. We resolved with those fab labs like Fab Lab NOLA to run Ubuntu in VirtualBox.

![](/assets/mama-rosie.jpg)

I decided to try the same setup with Mama Rosie. I had to migrate the local Wordpress installation from the Ubuntu partition to the Vbox installation. I then mirrored and flattened the site. Even under VirtualBox, the workflow was pretty slow. To scan and flatten the site took up to 30 minutes, each time. I also had to go to The Fab Foundation office to work on my documentation.

It was after the first lecture for this cycle of Fab Academy that I worked out a procedure that would allow me to work from multiple devices. I cloned the repository to Mama Rosie's desktop. Eclipse is an editor that I was comfortable with using from my previous web work. I could work on the code locally and push to the server. To solve the need for a local copy, I turned on a localhost server on Mama Rosie. I then copied my student folder to a subfolder of the local WebServer. In order to keep the code up to date, I tried some solutions for file synchronization. Unison was one option that we covered in the lecture. This solution needed a couple dependencies and some edits to config files. After a couple attempts, the build still failed on OS X El Capitan. It was then that I resolved, when we cover topics we aren't exactly mandated to use the options covered. Unison and rsync are recommendations, but I needed a currently supported app that would synchronize the contents of two local folders. I found Sync Folders on the App Store. This not only works with Mama Rosie running El Capitan, but also with my home laptop which runs Lion. I can sync folders and push to the repository much faster.

![](/assets/git-commit.gif)

Overall, I would still compose a website originally in CMS, mirror and flatten to HTML. Instead of regular updates, it's better to set a template and then edit the HTML from Eclipse. There is some housekeeping to do, but I'm happy with the current workflow.

On to spending some mental cycles sketching my final project...

#### 2018 Class Notes

At the lowest level, the work for this assignment is synchronization. rsync is a tool that enables peer-to-peer synchronization. This reconciles what changes were made and what needs to be copied. This will only copy changes and can be used to synchronize TB of data.

Version control does multiple things: synchronize work between computers, manage the history of the work, collaborate with other people on projects, remotely manage content on a server. The most popular tool for version control is called, git. Github is a web platform that uses git, but has interface tools for collaboration. The Fab Cloud is a gitlab installation for the fab lab network. We will use git to compose the website, but publish through Fab Cloud.

Dropbox is a cloud version of content management. Under the hood, DropBox runs version control. ownCloud is a similar tool to DropBox.

Once git is learned, we will be able to share work with the class through the server.

W3C is a program run out of MIT that standardizes the web. HTML5 is the current web standard. HTML is how we write a webpage. On the lowest level, we can write the actual code. A simple editor such as vi could be used to compose these pages. A cheat sheet of commands can be found, [here](http://www.atmos.albany.edu/daes/atmclasses/atm350/vi_cheat_sheet.pdf). Neil tends to work at a lower level than other people, because he likes control. :)

Atom, Sublime, Geany are open editors. WYSIWYG (what you see is what you get) editing can be done from a higher level editor such as LibreOffice. It is more complex, because the editor will add code automatically that will make the code more compliant to web standards. Other, more graphical editors, such as DreamWeaver can also be used. Javascript can be used to add programs and interactivity to web pages. During the Interface programming week, we will revisit Javascript to build applications. 

CGI, PHP is used to run code on servers. These are a security risk. For modern web programming and the scope of the class, these are not needed.

Low level text editors are ancient, but good for control. Experiment with a WYSIWYG editor. Document the range of experience with these tools.

Above flat HTML are content management systems, these are frameworks for managing group sets of pages. CMS have code running on the server. Each one has assumptions of how the individuals work. They are popular and used commercially. For the Fab Academy repo, using flat HTML outside of CMS makes the results more personal and expressive.

For videoconferences, historically the class was run through an MCU which is expensive around $500k centrally. The class is now run through BlueJeans via "the cloud" and WebRTC. OBS is an open source video broadcasting studio with tools for editing.

For remote screen sharing, VNC is a standard for screen sharing. Neil is running a virtual machine on the cloud that runs VNC for screen sharing. noVNC is a viewer that can be run from a web browser.

Cloud computing, Amazon EC2 (elastic cloud computing) is a popular platform. These are useful when you need more computing capacity. Heroku is also cloud computing, but more specifically for app development.

Project Management Systems, these are more intended for managing more than one person completing more than one task. Example programs are useful such as, TaskJuggler, OpenProj, GanttProject, Trello, and Taiga. For the class, project management will be centered around GitLab.

GitLab is many different things. It manages repositories. A repository is a set of files, is the history of the files, and can have branches for multiple versions. A second thing that GitLab does is issue tracking. Each project has its own issue tracker. In GitLab you can manage notifications. If you set a certain project to "watch", you will receive email notifications of issues as they arise. The communication is threaded. These issues trackers can cut down on email spam. Workflows, GitLab runs workflows to publish student content to the web. GitLab also has kanban boards that can help manage projects. GitLab has an in-browser editor to do editing on the server. The editor is not optimal for composition. Rather, you can do quick edits.

Standard mistakes, students will produce MB of data per week; labs will produce GB per cycle. Filesize is important to check, du is a good tool for filesize checking. Do not put uncompressed images into the repo. If more than one person is working on a repo, merge first and then push to the server. 

**Project Management Principles**

There is an important distinction between demand and supply-side time management. Supply-side time management is working back from the available time. Budget in advance the time needed for specific tasks. You can learn to work to a schedule. Do not work until you can succeed in each task. instead, work with the time that you have available.

Serial vs. parallel development; rather than work through tasks serially, look for ways to manage multiple tasks in parallel. Work out the dependencies for tasks.

Spiral development; rather than working on the complete system in a series of tasks, look for ways to prototype projects iteratively. This will result in a nested series of projects that add more upon iteration.

Bottom-up vs top-down debugging; rather than taking a big thing that doesn't work, think of projects through hierarchy and modularity. If you break your system into modules, you can debug the modules in isolation and then plug them back together.

Document as you work; if you work and then document, you will fail. Ara Knaian, the product of engineering if the documentation. Record, keep a running log of work, upon the completion of the project you will only need to add the final documentation.

Insights from Mythical Man-Month; a pregnancy is an example of a task that does not scale by adding labor but has fundamental limitations on the rate that progress can happen.

Project Management is not implicit; rather it is a set of skills that will develop over the course of the cycle.

#### Jan 22 recitation: version control (Fiore Basile)

What is version control? This is a way to keep track of the work that you do on a project, especially when working with a group. Collaboration; while working on a document, historically you would work a file at a time. For complex documents, there could be many changes resulting in many different version of a document taking up hard drive space. Change can be restored in a single repository through version control. Different changes can be tracked, as well.

Making copies of files; normally you would use a function like "Save as..." that would create different versions of the same project. Instead of making multiple files, we can think of development as engaging a database. For cloud applications, the act of saving can instantiate separate versions in whcih changes are tracked and can be restored. For version control, we don't just use a single, central database. This can be done in a distributed way.

History and tools; SCCS was a way to manage version control in the 1970's. This solution was local due to the lack of robust networking solutions. CVS and Subversion came into use in the late 1980s and 90s which introduced client server communication. Mercurial was a solution used in previous cycles of Fab Academy, but had issues with merging files. Git is now an industry standard and a good skill to learn.

Git was born out of necessity. Bitkeeper was used for tracking the Linux Kernel. The company retired their free version. Linus Torvalds, creator of Linux, coded Git based on concepts borrowed from Bitkeeper.

How Git works. Snapshot vs Deltas; old version control solutions compare the difference between files. Snapshots are made for every file that are entered into a repository. Git enables local operation meaning that you do not have to connect to the network; you can instead work with all the files locally. In order to do this, you check out the project to your working directory. You can then make changes and commit the changes to then push to the repository. Entering the files into the repo essentially creates two separate versions.

After installation, you can set a local identity from `git config`. `git init` will create your repository. This will create an empty folder with a hidden folder called ".git". It is important to not delete the ".git" folder. In the initialized repository, you can create files and add with `git add`. `git status` will give you the current status of the repository; this can include tracked and untracked files. Untracked files can be added or ignored prior to `git commit`. Committing files with `git commit -m "somestatus"`, will allow you to identify changes as you add to your repository. Ignoring files is done through `.gitignore`. Ignoring helps to keep repository clean. You can also have files locally that you do not want to expose globally. `git diff "filename"` is used to output the difference between the a file and it's previously committed version. `git rm` is the proper way to remove committed files. `git mv` is used for moving and renaming files. `git log` will give a history of who did what in a certain repository or project.

Working with remote repositories; the most common way of working with your repositories is SSH. Via SSH you can transmit via any protocol, including git.

up to 47:00

#### Jan 29 recitation: gitlab (Fiore Basile)