# Principles and Practices, Project Management

#### Have you:

* [x] made a website and described how you did it

* [x] introduced yourself

* [x] described and made a sketch of your final project

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

**What is Digital Fabrication**

There are three digital revolutions. Phones used to degrade with distance. Now we use the Internet to talk. Computers used to degrade with time. 

Moore's Law, ["Cramming more components onto integrated circuits"](https://www.cs.utexas.edu/~fussell/courses/cs352h/papers/moore.pdf). Concept of doubling scale. From components and transistors to "Lass' Law" which plots the doubling of fab labs within the International Fab Lab Network.

Connecting computers to machines was invented at MIT in 1952. The Whirlwind was the first real time computer. Around that time, jet aircraft were emerging. The parts were too hard to make by hand. The idea was that a real time computer could be connected to a machine to "turn the crank".

Vannevar Bush, he made the first analog computer at MIT. Claude Shannon was frustrated with using a computer that accumulated errors over time. ["A Symbolic Analysis of Relay and Switching Circuits"](https://dspace.mit.edu/handle/1721.1/11173) proves that Boolean algebra could be used to simplify the arrangement of relays used for communication. Shannon's work was applied by von Neumann to computation. Digital is a scaling property. By using a symbol representing the linear increase in the use of resources, whether in computation or communication; the error rate drops exponentially. 

Digital fabrication was "invented" four billion years ago. Humans are constructed from 20 amino acids which work like molecular Lego. Amino acids have properties. Ribosomes are assemblers that bolt together amino acids. Human bodies are then constructed "digitally".

On the surface level, digital fabrication is using a computer and a tool to make something. The deeper meaning is creating the code to make the thing.

MIT's Center for Bits and Atoms facilitates a ten million dollar "fab lab", which is a suite of research tools. There was a bottle neck on instruction of how to use the tools. This lead to the creation of "How to Make (almost) Anything". Projects from this class answered not so much "how" but "why" to do digital fabrication.

Following the parallel of development of computation, the Whirlwind was transistorized into the MIT TX-0 computer. The birth of modern computing happened at Bell Labs with the PDP, this was reflected in a scaling down physically of equipment from a building scale to a room. Ken Olsen was skeptical about the personal computer stating, "There is no reason for any individual to have a computer in his home". The killer app for computing ultimately became personal computing. The parallel discovered in the HTMaA class was that digital fabrication could be used to make products for a market of one, personal fabrication.

Educational outreach from CBA lead to the Fab Lab programming. The community-based Fab Lab is analogous to the PDP in scale. Filling the room, it is one machine or system for digital fabrication. One machine cannot make almost anything. The collection of fab lab machine can rather output any such projects.

Need to follow up: Haakon, nomadic herding and land use applications.

The International Fab Lab Network is part of the broader Maker movement. It is a more curated facet of the movement. No one is pushing populations to build fab labs, the labs are pulled into remarkable settings around the world. 

Fab Academy is distributed education, distinct from learning at the institution or online instruction. Participating Fab Lab nodes are an extension of the campus. A number of the class projects become businesses all came out of homework assignments in the Fab Academy.

How to Grow (alomost) Anything came from a collaboration with George Church.

Fabricademy is digital fabrication meeting textiles. 

MIT is a mainframe. Online classes are still centrally facilitated from a mainframe. Fab Academy is a distributed educational network. It is not so much controlled centrally.

Seymour Papert, fab labs lead to the literacy of not just how to use technology, but how to also build technology.

Fab Labs in Barcelona, fab labs could be used to start a business. Fab labs can also be used to make what people consume. The connection is open globally for knowledge. The atoms, matter stays within Barcelona for production. Fab Cities initiative is about local governments pledging to take on self-sufficiency. This does not lead to the creation of traditional jobs, but it does empower consumers to produce what they consume.

Personal manufacturing will ultimately replace traditional manufacturing.

Global Humanitarian Lab; instead of managing relief by physically sending solutions, the global network could send data and solutions could be manufactured locally.

FABx events; 11 was when the network descended upon MIT. FAB12 took the event to Shenzhen, China. Mass manufacturing plays a role in producing tools needed to create solutions locally.

Fab Foundation manages capacity. FabLabs.io is a social network for fab labs. If anybody can make anything, anywhere; what are the organizations to help manage that ability? Similar to ICANN and sister organizations on Internet Architecture Board.

Scale; we are now going from 1,000 to 1,000,000 fab labs. One million is the number of towns in the world. To go from one point of scale to another, How to Make Something That Makes (almost) Anything was developed. Modular software and modular hardware helps to rapidly make machines. Nadya Peek, ["Making Machines that Make: Object-Oriented Hardware Meets Object-Oriented Software"](http://infosyncratic.nl/peek-making-machines.pdf). Jens Dyvik built upon the work of modular machines. The idea is to make a machine that would be capable of making its own parts. The next step of fab labs is to be able to composed and design parts for machines that make.

From one million to one billion; this is the number of people on Earth. The supply chain needs to be deprecated. How can materials be digitized?

From one billion to one trillion, this is the Internet of Things but for a manufacturing application. Ribosomes are slow they make complex structures at one molecule per second. Ribosomes also construct other ribosomes. Hierarchy in biology is parallel in engineering. Blending communication and computation for fabrication output. John von Neumann, ["Theory of Self-Reproducing Automata"](http://cba.mit.edu/events/03.11.ASE/docs/VonNeumann.pdf).

Manufacturing is going from a mainframe to a minicomputer (fab lab) to a personal computer (mtm) to ubiquitous (Star Trek Replicator). Research to reach ubiquitous takes fifty years, we are currently in the middle of that path, the "mini computer" era. The class is teaching digital fabrication, but also asks what is: business, education, governance, and how does the world change?

**Designing Reality**

