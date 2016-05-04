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

Code Review some positive side effects
--------------------------------------

During my work experience at [GEM Foundation][1] and [RedHat][2] I had the
chance of working in teams which make use of the practice of code review.
Having some fresh set of eyes looking over code allow to prevent bugs or even
improve what has been written, but that isn't the most valuable aspect.
What makes code review a terrific practice are its social implications.
Code that gets reviewed is written with a reader in mind and with much more
care because is going to be evaluated by a teammate, so there is healthy
*social pressure*, everybody wants to produce work deemed of good quality.
The end result is code that is neater and much more understandable.

Another big benefit of code review is that it allows to share knowledge
among team memebers. Usually software developers are spread among different
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

Doing a good code review requires some practice. You have to provide feedback
that is contextual and valuable to the work being reviewed in a way that
enriches the developer; the purpose is to improve the worked code and learn
from mistakes. It's very important to be careful in the way provide feedbacks,
and their substance.

On the form
-----------
![Man finger pointing](/img/Anger-Man-Pointing-Finger.jpg)
*For one finger pointing forward, there are three pointing backwards.*

Feedbacks are better listened when they’re framed as [open questions][4]:
“What happens if this method takes a negative integer as input value?”
sounds different than “Your code is not enough robust it breaks with negative values”,
even if both comments highlight the same issue, the first one considers the human factor involved and focus on the issue,
the second one focus the attention on the reviewee (“You silly sausage!”),
nobody likes being accused of writing bad code, although sometimes we all write some nasty code.
We’re humans, we make mistakes, bad code can be the result of inexperience
which can be translated in lack of knowledge, time constraints or simply an awful day.
Asking open-ended questions is also useful to clarify intentions, perhaps reviewers lack of some information
or they can be simply wrong, reviewers are humans too :-).

On the substance
----------------

Feedbacks should be constructive, the goal is to educate, avoiding make the same mistake in the future,
so spend some time explaining, for example, why some code is not reusable in different contexts
and how you can address that issue; when improving the code being worked requires substantial refactoring,
do help to achieve the suggested improvement, so the reviewee will experience the improvement not as a form
of punishment (more work on a task he/she considered completed) but as learning positive experience.
When doing a code review, never ever ever being pushy about a specific approach to use,
you’ll be seen like a jerk suggesting “the one true way” of doing things, otherwise the reviewee will change
his/her attitude toward a defensive one, where no matter how good and objective your arguments are,
emotions will prevail and an occasion of learning and working better together will be wasted.
As a final point, we should modify our mindset, we as developers should be fearless, accepting our mistakes
without worrying about other people’s judgments, we should care more about how we can gather feedback and use
them effectively improving ourselves. Mistakes happen, let’s not waste any of them.
Don’t be afraid of mistakes, laugh about them, learn, move on.

[1]: http://www.globalquakemodel.org/
[2]: https://www.redhat.com/
[3]: https://en.wikipedia.org/wiki/Bus_factor
[4]: https://en.wikipedia.org/wiki/Socratic_method
