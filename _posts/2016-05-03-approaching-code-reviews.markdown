---
layout:     post
title:      "Approaching Code Reviews"
subtitle:   "a few hints" 
abstract:   Code review or peer review is a process in which code written by developer is examined by another person in order to highlight possible mistakes, with the primary objective of improving the overall software quality, however code review provides greater benefits... 
date:       2016-05-03 12:00:00
author:     "Giuseppe Vallarelli"
header-img: "img/post-bg-01.jpg"
comments:   true
tags:
  - code reviews
  - development practices
---

During my work experience at [GEM Foundation][1] and [RedHat][2] I had the
chance of working in teams which make use of the practice of code review.
Having some fresh set of eyes looking over code allow to prevent bugs or even
improve what has been written, but that isn't the most valuable aspect.
What makes code review a terrific practice are its social implications.
Code that gets reviewed is written with a reader in mind and has higher
quality because is going to be evaluated by a coworker, so there is healthy
*social pressure*, everybody wants to do good work. The end result is code
that is neater and much more understandable.

Another big benefit of code review is that it allows to share knowledge
among coworkers. Usually software developers are spread among different
software components or even projects, so it's very easy to create some
knowledge silos, meaning that only one or a few people are knowledgeable and
capable of continuing work on a specific project, this problem is also known
as [Bus Factor][3], which denotes the number of people that can be lost
(literally hit by a bus) before bringing the project to a halt. Using
code review makes sure that at least a couple of people (writer and reviewer)
are familiar with the codebase. It is also very effective in bringing up
to speed new hires on developement practices shared among team members or
mentoring junior developers, I've learned a good deal both by having my
code reviewed or reviewing code of more senior developers.

Doing code review require some practice, sometimes it's very tempting to
propose some changes that alter the proposed solution in a significant way,
this can can lead to frustruation and hard feelings. As long as the proposed
solution is correct and sound you shouldn't propose a significant change that
alter the original design, given the same problem it's highly unlikely that
two developers produce the same solution. The objective is to prevent bugs
to slip in the codebase not to compete with or make a coworker crossed at you.
If everything looks good, thumbs up! No need of nitpicking.

![Man finger pointing](/img/Anger-Man-Pointing-Finger.jpg)
*Avoid heated debates, they damage teammates morale and harm trust.*

Another aspect worth considering is the way the feedback is provided.
I realized over the time that asking open questions challenging the assumption
made in the solution helps in understanding the problem better and leads
to a better solution. It's very important not be harsh with the solution's
author, we all tend to be on the defensive when criticized which doesn't
help to focus on the problem at hand, besides we all make mistakes.

Last but not least important is the time requested for a code review,
ideally code reviews should happen quickly, in order to increase
the odds it's very important that the proposed changeset has a manageable
size and represents possibly only one logical change.

[1]: http://www.globalquakemodel.org/
[2]: https://www.redhat.com/
[3]: https://en.wikipedia.org/wiki/Bus_factor
