# Noted

Ethan Turkeltaub


## Abstract

For Custom Capstone, I looked at the problems that students have that could be solved by a web application. I created Noted, a service that helps organize and collaborate on research projects. Initially, I had lofty goals for what Noted could be, but as time went on and I fell further and further behind, I started stripping away extraneous features and created a site that is simpler and better at what it _does_ do. Notes are central to Noted, and less so are your citations. Rather than focus on the source of your information, it is understanding and  retaining that information that is important. Noted aims to make this skill easy for anyone who goes to the site, despite their age.

## Introduction

For custom capstone, I chose the innovation pathway and created Noted, a web service that allows for students to organize and collaborate on research projects. I set out with the goal to take away the pain students associate with note taking and citing sources by making the interface disappear — it should be easy for anyone to see the site and instantly know what to do. I wanted to expand my previous knowledge of web design by seeing a product from its infancy to being live for people to use — I had never done so, and I believe it was a worthwhile, eye-opening experience.

## Prior Experience

I have quite a bit of previous experience with web design and development. Over the past two summers, I was a technology intern at Fanzter, a Unionville-based web startup that has multiple products that are used by thousands of people. I also created the Farmington High School Clock, replacing a nearly ten-year-old system that displays the day's schedule, current information, and time.

## Research

The idea for Noted came from frustration with current solutions to the problem of research management. NoodleTools, the product we currently use, is very unintuitive. It is a tedious process to do any work on the site, and consistently frustrates students and teachers alike.

Initially, I had high hopes for the features I could add that would potentially help students, such as Google Docs and Dropbox integration, line-by-line commenting on notes, and others.

I spoke with faculty and students to see what exactly they wanted from a research management tool. The answers were varied, but a common theme was that both groups wanted it to be easier for them, rather than the other group — the faculty wanted to make it easier to quickly browse through their class's projects, and the students wanted it easier to take notes or cite sources and move on. After some deliberation, I decided to focus the site for use by the students. To be fair, they are the ones who are ultimately doing the research. However, tried to make the use case for the service as ambiguous as possible: this means that the service does not have a specific way you "should" use it. It is simply up to the user as to how they use the tools given to them. It should be a good tool for students, as well as researchers — for most users, the teachers tools would not be necessary.

I began to create a list of features that I will actually implement in the site. This needed to be a realistic list of what I could actually get done in nine months — I could not simply list my "dream" features. This is important, especially in web development. Avoiding the "feature creep" of a project is a skill that many professional web development firms have trouble with, so I had to learn to do my best to keep on task.

## "Good" Design

As time progressed, I realized how little time I actually had — experienced web development teams could not finish the website I envisioned in the time allotted. I had underestimated the time necessary for each piece of the site. I learned that in computer science, you should take the time you _think_ is necessary for a task, and quadruple it. Needless to say, I had to begin stripping away features. Overall, I believe this is a good thing for the service — the less there is, the less the user has to comprehend. This is where I decided I would distinguish my product from the competition: NoodleTools aims to be an all-purpose research tool, whereas I strive for simplicity and clarity.

> Good design is as little design as possible. Less is more – because it concentrates on the essential aspects and the products are not burdened with non-essentials. Back to purity, back to simplicity.
> 
> — _Dieter Rams_

Internationally-acclaimed industrial designer Dieter Rams laid the principles of modern aesthetics. He believes that less is more — by stripping away what is unnecessary, you create a better user experience.

I kept this quote in mind as I continued tow work. This shaped my progress in both the design and website as well as the code I wrote. In Scholar, the external library I created to deal with the creation of MLA citations, I did my best to embodied this ideal — I made it easy for someone else to look at the code and instantly understand what every piece does. Knowing how to strip away features until you're left with the bare essentials is important in nearly every web project.

## Scholar

Scholar was the toughest piece of the site to write. I first had to understand MLA citations and how they are structured: no easy task, considering how inconsistent and ever-changing they are. With this in mind, I set out to create a code library that was extensible and modular — it's fundamentally easy to add pieces to the library. Essentially, each piece of the code can live on it's own, and it is easy to add on pieces. In particular, it is easy add different source types (like books, websites, magazines, etc). Anyone could add or modify a definition file with the following components;

1. The order in which each attribute of the source is listed. For example, a citation for a book lists the authors, then the title, then the editors, and so forth).
2. What formatting should be carried out on each attribute. For instance, the title of a book should be italicized.

This process is one of the key skills of computer science. The ability to take a problem and break it down into smaller, manageable pieces is a something that is absolutely essential in tackling large projects like Noted.

## User Interface

The user interface evolved significantly with the help of Mr. Procko, my advisor. I do not nearly have as much experience with design as I do with development, and having a second pair of eyes on the site was extremely helpful. He pointed out some parts of the site that users would have trouble with, and gave suggestions on how to improve the overall design.

Eventually, I adopted a visual style that is called "flat design" within the web design community. By not including gradients (transitions from color to color), faux-textures, and skeumorphism (fake realism), I reduce the clutter of the interface. "Good" flat design is hard to achieve — without visual cues, it is up to the designer to give users an idea of what they can do. For example, many older websites make buttons look like they would in real life — with texture, shadow, and a glossy-type effect. However, flat design does not include these hints, and it must be clear to the user that something like a block of color with text in it is indeed something you can click.

## Resources

The web development community is large, and the amount of resources that are available to the community is larger still. A multitude of web communities have sprung up over the years to cater to programmers, most notably [GitHub](https://github.com) and [Stack Overflow](http://stackoverflow.com).

At the very fundamental level, GitHub is an interface to the version-control system Git (a way for programmers to keep track of the history and changes in their code). But, a community has flourished around GitHub. Their emphasis on open-source makes it easy for anyone to create a project and show it to the world. There is also a push for collaboration between users, and everyone is encouraged to contribute to their favorite projects.  The wealth of code on GitHub (nearly 5 million code projects) makes it easy for me to look and see solutions to problems that I wouldn't be able to solve on my own. It is also for me to get help on my code — if I wanted to show someone my code, I can just pull up the GitHub project and they can browse the code. Eventually, they may contribute to that project. For example, Dirk Gadsden, another web developer who lives in Charleston, was able to add code to Scholar.

Stack Overflow is another community for programmers, but instead of code hosting, it is a question and answer site. Chances are, someone else has had the same problem you've had and had it answered on Stack Overflow. If I am particularly stumped on a problem, I can ask on Stack Overflow for help and get a solution within hours.

Another vital resource was the engineers at Fanzter, the startup I've worked at the past two summers. They are seasoned experts in high-traffic web applications, and were able to point out holes in my code and ways I can improve the user experience.

## Conclusion

My goal for capstone was to hone the skills I had acquired from my own learning. Through the process of creating the website, I did just that. I picked up some new techniques along the way, but on the whole, I did not learn anything _new_, I simply sharpened my the skills I already had. That, I believe, is one of the most important skills of all — to take something that you think you know a lot about and expand that knowledge.

Guiding a product from start to finish was something that I had never done before, especially on this scale. Each stage had something to add to my knowledge, from the initial brainstorming to making the finished product available on the web.

Though it was indeed a lot of work, I think this experience was worth it — and enjoyable. It is something that I have done and would like to continue to do in the future.


## Bibliography

_GitHub_. GitHub, Inc., n.d. Web. 06 May 2013. <http://github.com/>.
_StackOverflow_. Stack Exchange, Inc., n.d. Web. 06 May 2013. <http://stackoverflow.com/>.
