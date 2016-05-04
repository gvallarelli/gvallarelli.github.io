---
layout:     post
title:      "Approaching Code Reviews"
subtitle:   "a few hints" 
date:       2016-05-03 12:00:00
author:     "Giuseppe Vallarelli"
header-img: "img/post-bg-01.jpg"
comments:   true
tags:
  - code reviews
  - development practices
---

Doing a good code review is not easy. You have to provide feedback that
is contextual and valuable to the work being reviewed in a way that enriches
the developer; the purpose is to improve the worked code and learn from mistakes,
hopefully not redoing them again, but doing different ones instead.
Code review is a wonderful tool which helps to fix problems,
when the needed fix is still cheap and favors knowledge sharing on both sides (reviewers / reviewee).
Important aspects of code reviews, are the way you provide feedbacks, and their substance.

On the form
-----------
![Man finger pointing](/img/Anger-Man-Pointing-Finger.jpg)
*For one finger pointing forward, there are three pointing backwards.*

Feedbacks are better listened when they’re framed as [open questions][1]:
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

[1]: https://en.wikipedia.org/wiki/Socratic_method
