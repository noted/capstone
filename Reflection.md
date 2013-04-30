### Abstract

For custom capstone, I looked at the problems that students have that could be solved by a web application and I created Noted, a service that helps organize and collaborate on research projects. Initially, I had lofty goals for what Noted could be, but as time went on and I fell further and further behind, I started stripping away extraneous features and created a site that is simpler and better at what it _does_ do. Notes are central to Noted, and less so are your citations. Rather than focus on the source of your information, it is understanding and  retaining that information that is important. Noted aims to make this skill easy to anyone who goes to the site, despite their age.

### Noted

For custom capstone, I chose the innovation pathway and created Noted, a web service that allows for students to organize and collaborate on research projects. I set out with the goal to take away the pain students associate with note taking and citing sources by making the interface disappear — it should be easy for anyone to see the site and instantly know what to do.

I have quite a bit of previous experience with web design and development. Over the past two summers, I was a technology intern at Fanzter, a Unionville-based web startup that has multiple products that are used by thousands of people. I also created the Farmington High School Clock, replacing a nearly ten-year-old system that displays the day's schedule, current information, and time.

The idea for Noted came from frustration with current solutions to the problem of research management. Initially, I had high hopes for the features I could add that would potentially help students like Google Docs and Dropbox integration, line-by-line commenting on notes, and others. However, as time progressed, I realized how little time I actually had — experienced web development teams could not finish the website I envisioned in the time allotted. Therefore, I had to begin stripping away features. Overall, I believe this is a good thing for the service — the less there is, the less the end-user has to comprehend.

> Good design is as little design as possible. Less is more – because it concentrates on the essential aspects and the products are not burdened with non-essentials. Back to purity, back to simplicity.
> 
> — _Dieter Rams_

Internationally-acclaimed industrial designer Dieter Rams laid the principles of modern aesthetics. He believes that less is more — by stripping away what is unnecessary, you create a better user experience.

I used this mindset as I continued work on Noted. This shaped my work in both the user-facing design and website as well as the code I wrote. In Scholar, the external library I created to deal with the creation of MLA citations, I embodied this ideal — I made it easy for someone else to look at the code and instantly understand what every piece does.

Scholar was the toughest piece of the site to write. I first had to understand MLA citations and how they are structured: no easy task, considering how inconsistent and ever-changing they are. With this in mind, I set out to create a code library that was extensible and modular — it's fundamentally easy to add pieces to the library. In particular, it is easy add different source types (like books, websites, magazines, etc). Anyone could add or modify a definition file with the following components.

1. The order in which each attribute of the source is listed. For example, a citation for a book lists the authors, then the title, then the editors, and so forth).
2. What formatting should be carried out on each attribute. For instance, the title of a book should be italicized.

This erases the various quirks MLA citations have. I released Scholar as a free-to-use open source project on GitHub, so hopefully someone else can benefit from the work I did.

The user interface evolved significantly with the help of Mr. Procko. I do not nearly have as much experience with design as I do with development, and having a second pair of eyes on the site was extremely helpful.

I adopted a visual style that is called "flat design" within the web design community. By not including gradients, faux-textures, and skeumorphism, I reduce the clutter of the interface. "Good" flat design is hard to achieve — without visual cues, it is up to the designer to make actions the user can do obvious. Many web designs in the past have made buttons rounded, have shadows and look like — well — buttons, in order to signify that that box on a screen is indeed and button, and can be pressed. Flat design does not include these hints, and needs to be simplified.

The web development community is large, and the amount of resources that are available to the community is larger still. A multitude of web communities have sprung up over the years to cater to programmers, most notably [GitHub](https://github.com) and [Stack Overflow](http://stackoverflow.com).

At the very fundamental level, GitHub is an interface to the version-control system Git (a way for programmers to keep track of the history and changes in their code). But, a community has flourished around GitHub. Their emphasis on open-source makes it easy for anyone to create a project and show it to the world. There is also a push for collaboration between users, and everyone is encouraged to contribute to their favorite projects.  The wealth of code on GitHub (nearly 5 million code projects) makes it easy for me to look and see solutions to problems that I wouldn't be able to solve on my own. It is also for me to get help on my code — if I wanted to show someone my code, I can just pull up the GitHub project and they can browse the code. Additionally, people can contribute to my project. For example, I requested help of Dirk Gadsden, another web developer, with Scholar, and he was able to write code and contribute to my project.

Stack Overflow is another community for programmers, but instead of code hosting, it is a question and answer site. Chances are, someone else has had the same problem you've had and had it answered on Stack Overflow. If I am particularly stumped on a problem, I can ask on Stack Overflow for help and get a solution within hours.