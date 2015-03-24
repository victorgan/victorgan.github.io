---
layout: post
title: Calculating Taxes
---
It's tax season yay!

I've started filling out my forms, and even though I'm living in British
Columbia, on December 31st I was in Ontario, which means I'd file for Ontario
taxes.

It turns out, there's not much difference for a non-scholarship gross income of
around $300. Go figure. But calculating actual tax rates is actually not obvious
due to marginal tax structures. It also varies widely depending on where you
live, so it's probably a good idea to see what effects taxes have on your gross
salary if you're comparing jobs in different regions. I could see myself working
in Ontario, British Columbia, Alberta, Washington state and California.

So, I did some number crunching. Here's the effective tax rates and the actual
dollar amounts, plotted against gross income.

![Taxes]({{ site.url }}/assets/posts/2015-03-23-taxes.png)
![Taxes]({{ site.url }}/assets/posts/2015-03-23-taxes2.png)

Note that there's no currency conversion going on; California and Washington use
US dollars. Interestingly, California, Ontario and British Columbia all have
pretty similar tax rates (ignoring currency differences), which converges to
Alberta's. Washington, because it has no state income tax, means you'll likely
save around 4-10 grand from the tax person.

Code: [https://github.com/victorgan/effective-tax-rates](https://github.com/victorgan/effective-tax-rates)

[This analysis](http://tgeonetta.com/cost-of-living-vs-salary-best-cities-for-software-developers-and-engineers/)
on how far your dollar goes does something similar and also includes the cost of
living.

For completeness, here's a plot of the effective tax rates for all the Canadian
provinces.

![Taxes]({{ site.url }}/assets/posts/2015-03-23-taxes3.png)

Ouch, Quebec gets taxed like crazy.
