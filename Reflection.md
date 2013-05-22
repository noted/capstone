# Noted

Ethan Turkeltaub


## Abstract

For Custom Capstone, I looked at the problems that students have that could be solved by a web application. I created Noted, a service that helps organize and collaborate on research projects. Initially, I had lofty goals for what Noted could be, but as time went on and I fell further and further behind, I started stripping away extraneous features and created a site that is simpler and better at what it _does_ do. Notes are central to Noted, and less so are your citations. Rather than focus on the source of your information, it is understanding and  retaining that information that is important. Noted aims to make this skill easy for anyone who goes to the site, despite their age.

## Reflection

For custom capstone, I chose the innovation pathway and created Noted, a web application to help students organize and collaborate on research projects.

Prior to the course, I knew that I wanted to make a website that benefited the school. Given my background, I knew that I would have some knowledge of how to build it, but building a full-scale product would require more growth on my part. I started to think about a technical aspect of Farmington High School that could be improved upon, and my mind immediately went to NoodleTools.

NoodleTools is the product we currently use at Farmington for research management, but it frustrates most people that use it. Essentially, you create projects, and associate citations and notes with those projects. However, the user interface (the design of the site and how people interact with it) is unintuitive — it is difficult to do simple tasks, like create notes. Students get easily irritated,  and teachers lose class time when they have to help students instead of teach. This is the problem I wanted to solve — I wanted to create a site with similar features that makes the process of organizing your projects and collaborating with others easier.

I have quite a bit of previous experience with web design and development. Over the past two summers, I was a technology intern at Fanzter, a Unionville-based web startup that has multiple products that are used by thousands of people. I also created the Farmington High School Clock, replacing a nearly ten-year-old system that displays the day's schedule, current information, and time. I do not, however, have experience with creating large-scale websites from scratch. Websites that are the size of Noted are extremely complex. The amount of time that is required to perfect every aspect of such a site is extraordinary. Additionally, there are considerations that need to be made, such as security, reliability, and speed, that I do not have experience with.

To begin the process of developing Noted, I spoke with faculty (Mrs. Burr, Ms. Bevz, and Mrs. Carlson) and students (including students from different grade levels) to see what exactly they wanted from a research management tool. I have never done user research for a website, so trying to find the right questions to ask was challenging. For most of the interviewees, I ended up just having a casual discussion about their current experiences with NoodleTools, and then what exactly they would want as an alternative. This proved effective, as I uncovered many grievances that other users had with NoodleTools, especially with teachers. Unbeknownst to me, what teachers saw when they logged into the website was entirely different than what students saw. This was an aspect of the site I had not known about, and hadn't planned on building.

Instead of following the path that NoodleTools took, I decided to make what everyone saw when they logged into the site the same, regardless if that person was a student or a teacher. This makes the use case as ambiguous as possible — everyone can use the site how they want to. This opens the site up to a large audience, including individual students and researchers.

From the interviews, I began to create a list of features that I would actually implement in the site. This needed to be a realistic list of what I could actually get done in nine months — I could not simply list my "dream" features. This is important, especially in web development. Avoiding the "feature creep" of a project is a skill that many professional web development firms have trouble with, so I had to learn to do my best to keep on task.

I planned out, on paper, just how each piece of the site would interact with each other. This ended up being a very good idea — had I continued with my original plan, I would run into issues later on that would cause me to have to rewrite quite a bit of code.

Actual work on the site started later than I had anticipated. I wanted to use a programming technique called "test-driven development", wherein you create tests for your code before your actual code. You write the test code, run it, watch as it doesn't work, and then you write the actual code necessary to make that test code work. 	I had previously never used test-driven development for an entire project, and I wanted to see the results of doing so. However, as I found out, this process is quite slow. I produced cleaner, more efficient code, but it was taking me twice as long to do what I needed to do. About half-way into the development process, I abandoned test-driven development and worried about the test code later — a decision I have come to regret.

The quality of the code I write is important to me. I strive for understandability and organization — ultimately, this makes it easier for me and others to look at it and know exactly what it does without explanation. With test-driven development, I was writing code that made sense to both me and others who looked at it. After abandoning this, my code degraded into "spaghetti code". It was messy and confusing, and even I had trouble going back and understanding what each piece did. I sacrificed understandability for speed of development, and this is a mistake that I will not make again.

Even though I was working faster at this point, I still wasn't going to be finished in time for the due date. I therefore needed to strip away features. Anything that wasn't necessary to the core feature set of the product were gone — everything except projects, collaboration, and citations were thrown away. In hindsight, I believe that this was a positive thing for the product.

> Good design is as little design as possible. Less is more – because it concentrates on the essential aspects and the products are not burdened with non-essentials. Back to purity, back to simplicity.
> 
> — _Dieter Rams_

Internationally-acclaimed industrial designer Dieter Rams laid the principles of modern aesthetics. He believes that less is more — by stripping away what is unnecessary, you create a better user experience.

I kept this quote in mind as I continued to work. This shaped my progress in both the design and website as well as the code I wrote. In Scholar, the external library I created to deal with the creation of MLA citations, I did my best to embody this ideal — I made it easy for someone else to look at the code and instantly understand what every piece does. Knowing how to strip away features until you're left with the bare essentials is important in nearly every web project.

Scholar was the toughest piece of the site to write. I first had to understand MLA citations and how they are structured: no easy task, considering how inconsistent and ever-changing they are. With this in mind, I set out to create a code library that was extensible and modular — it's fundamentally easy to add pieces to the library. Essentially, each piece of the code can live on it's own, and it is easy to add on pieces. In particular, it is easy add different source types (like books, websites, magazines, etc). Anyone could add or modify a definition file with the following components;

1. The order in which each attribute of the source is listed. For example, a citation for a book lists the authors, then the title, then the editors, and so forth).
2. What formatting should be carried out on each attribute. For instance, the title of a book should be italicized.

This process is one of the key skills of computer science. The ability to take a problem and break it down into smaller, manageable pieces is a something that is absolutely essential in tackling large projects like Noted.

The user interface evolved significantly with the help of Mr. Procko, my advisor. I do not nearly have as much experience with design as I do with development, and having a second pair of eyes on the site was extremely helpful. He pointed out some parts of the site that users would have trouble with, and gave suggestions on how to improve the overall design.

Eventually, I adopted a visual style that is called "flat design" within the web design community. By not including gradients (transitions from color to color), faux-textures, and skeumorphism (fake realism), I reduce the clutter of the interface. "Good" flat design is hard to achieve — without visual cues, it is up to the designer to give users an idea of what they can do. For example, many older websites make buttons look like they would in real life — with texture, shadow, and a glossy-type effect. However, flat design does not include these hints, and it must be clear to the user that something like a block of color with text in it is indeed something you can click. I have dabbled in flat design before with the Clock, but I had never created entire websites with the style.

At this point in the process, the website is almost complete. A good majority of the design is complete, and all of the major features are finished. All I have left are a lot of small tweaks, some of which I'll need to consult the engineers at Fanzter for. I plan to open up the site for a limited test period after my presentation at http://beta.getnotedapp.com.

Guiding a product from start to finish was something that I had never done before, especially on this scale. Each stage had something to add to my knowledge, from the initial brainstorming to making the finished product available on the web. This experience opened my eyes to the fine details of creating a website for consumers, and I will not forget it.

### Resources 

The web development community is large, and the amount of resources that are available to the community is larger still. A multitude of web communities have sprung up over the years to cater to programmers, most notably [GitHub](https://github.com) and [Stack Overflow](http://stackoverflow.com).

At the very fundamental level, GitHub is an interface to the version-control system Git (a way for programmers to keep track of the history and changes in their code). But, a community has flourished around GitHub. Their emphasis on open-source makes it easy for anyone to create a project and show it to the world. There is also a push for collaboration between users, and everyone is encouraged to contribute to their favorite projects.  The wealth of code on GitHub (nearly 5 million code projects) makes it easy for me to look and see solutions to problems that I wouldn't be able to solve on my own. It is also for me to get help on my code — if I wanted to show someone my code, I can just pull up the GitHub project and they can browse the code. Eventually, they may contribute to that project. For example, Dirk Gadsden, another web developer who lives in Charleston, was able to add code to Scholar.

Stack Overflow is another community for programmers, but instead of code hosting, it is a question and answer site. Chances are, someone else has had the same problem you've had and had it answered on Stack Overflow. If I am particularly stumped on a problem, I can ask on Stack Overflow for help and get a solution within hours.

Another vital resource was the engineers at Fanzter, the startup I've worked at the past two summers. They are seasoned experts in high-traffic web applications, and were able to point out holes in my code and ways I can improve the user experience.

### Bibliography

_GitHub_. GitHub, Inc., n.d. Web. 06 May 2013. <http://github.com/>.
_StackOverflow_. Stack Exchange, Inc., n.d. Web. 06 May 2013. <http://stackoverflow.com/>.
