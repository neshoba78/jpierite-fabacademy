# Principles and Practices, Project Management

#### Have you:

* [ ] made a website and described how you did it

* [ ] introduced yourself

* [ ] described and made a sketch of your final project

* [ ] documented steps for uploading files to archive

* [ ] pushed to the class archive

In a previous life, I was an Internet Marketing Specialist for Mohegan Sun in Uncasville, CT. I helped manage six of their company websites using proprietary content managements systems and flat HTML. I got comfortable with working first with a local copy and pushing content to a server that was scheduled to cache every four hours.

These are some of the websites that I worked on:

[Mohegan Sun](https://mohegansun.com/)

[Mohegan Sun Pocono Downs](https://mohegansunpocono.com/)

[Mohegan Tribal Gaming Authority](http://newsroom.mtga.com/)

[The Fab Foundation](http://www.fabfoundation.org/)

[FAB11](http://fab11.fabevent.org/)

I started class work for Fab Academy in 2015. Back then, we used Mercurial for version control. Repositories were divided by region. Continuing my work after FAB12 with Fab Lab Wgtn, I started to work in the git repository under a network folder with a very binary student ID.

Originally, I built my website with a local copy of Wordpress. I triple booted my work computer, “Mama Rosie”, and installed the CMS on an Ubuntu partition. As I made updates to my website, I mirrored it with httrack to make flat HTML files. This was a workflow that I used through Fab Academy 2015 and 2016.

As part of my job deploying fab lab inventory to new fab lab installations, I work out standard procedures for dual or triple booting computers and installing all the necessary freeware. Recently, we started to get requests for computers with Windows 10. Dual booting these machines wasn't working out too well. There was an issue with Ubuntu corrupting wireless networking drivers on the Windows side. We resolved with those fab labs like Fab Lab NOLA to run Ubuntu in VirtualBox.

I decided to try the same setup with Mama Rosie. I had to migrate the local Wordpress installation from the Ubuntu partition to the Vbox installation. I then mirrored and flattened the site. Even under VirtualBox, the workflow was pretty slow. To scan and flatten the site took up to 30 minutes, each time. I also had to go to The Fab Foundation office to work on my documentation.

It was after the first lecture for this cycle of Fab Academy that I worked out a procedure that would allow me to work from multiple devices. I cloned the repository to Mama Rosie's desktop. Eclipse is an editor that I was comfortable with using from my previous web work. I could work on the code locally and push to the server. To solve the need for a local copy, I turned on a localhost server on Mama Rosie. I then copied my student folder to a subfolder of the local WebServer. In order to keep the code up to date, I tried some solutions for file synchronization. Unison was one option that we covered in the lecture. This solution needed a couple dependencies and some edits to config files. After a couple attempts, the build still failed on OS X El Capitan. It was then that I resolved, when we cover topics we aren't exactly mandated to use the options covered. Unison and rsync are recommendations, but I needed a currently supported app that would synchronize the contents of two local folders. I found Sync Folders on the App Store. This not only works with Mama Rosie running El Capitan, but also with my home laptop which runs Lion. I can sync folders and push to the repository much faster.

Overall, I would still compose a website originally in CMS, mirror and flatten to HTML. Instead of regular updates, it's better to set a template and then edit the HTML from Eclipse. There is some housekeeping to do, but I'm happy with the current workflow.

On to spending some mental cycles sketching my final project...

