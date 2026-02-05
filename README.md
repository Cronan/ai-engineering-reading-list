# AI in Production Engineering

A curated reading list for engineers integrating AI into production systems.

**The thesis:** The bottleneck isn't capability - it's trust. We can build AI systems that perform; we struggle to build systems we can verify, understand, and safely operate. The infrastructure that matters is [*observable, reversible, and enforceable*](https://cronyn.co.uk/writing/observable-reversible-enforceable.html).

Most AI commentary is academic theory or breathless hype. This list is neither. It's what's proved useful building production financial systems over 25 years, now with AI in the mix.

## Reading trails

Short on time? Three paths through this material:

**The Bainbridge trail** (start here)
Bainbridge → Cook → Klein → [my essay on the ironies](https://cronyn.co.uk/writing/ironies-of-automation.html)
Why automation creates the problems it was meant to solve. The foundation for everything else.

**The trust trail**
Lamport → Charity Majors → Rudin → Huyen → [observable, reversible, enforceable](https://cronyn.co.uk/writing/observable-reversible-enforceable.html)
Building systems you can verify. The framework for operational trust.

**The people trail**
Klein (both) → Allspaw → Larson → [my essay on building engineers](https://cronyn.co.uk/writing/ai-as-junior-engineer.html)
How AI changes the way engineers develop expertise.

---

## The foundational problem

**Lisanne Bainbridge - [Ironies of Automation](https://ckrybus.com/static/papers/Bainbridge_1983_Automatica.pdf)** (1983)

Written about industrial process control, but maps precisely onto AI-assisted software development. The core insight: the more advanced the automation, the more critical the human contribution, and the less likely humans are able to provide it. If you read one thing on this list, read this. I wrote about applying this to AI in [Bainbridge's Ironies of Automation, forty years on](https://cronyn.co.uk/writing/ironies-of-automation.html).

**Gary Klein - [Sources of Power: How People Make Decisions](https://mitpress.mit.edu/9780262534291/sources-of-power/)** (1998)

How experts actually make decisions under pressure. Not through analysis, but through pattern recognition built from experience. Relevant because AI changes how engineers build that pattern recognition.

**Gary Klein - [Seeing What Others Don't](https://www.hachettebookgroup.com/titles/gary-klein/seeing-what-others-dont/9781610392754/)** (2013)

Klein's follow-up to Sources of Power. This one focuses on insight: how experts notice things others miss. Relevant to understanding what expertise looks like and whether AI can replicate it.

**Erik Hollnagel & David Woods - [Joint Cognitive Systems](https://www.taylorfrancis.com/books/mono/10.1201/9781420038194/joint-cognitive-systems-erik-hollnagel-david-woods)** (2005)

Treats human and machine as a single cognitive system. The unit of analysis isn't the person or the AI, but the combination. Changes how you think about designing AI-assisted workflows.

## Safety and resilience

**Richard Cook - [How Complex Systems Fail](https://how.complexsystems.fail/)** (1998)

Eighteen propositions in four pages. Written about healthcare, applies everywhere. The core claim: failure is normal, and safety comes from how systems handle it. Pairs well with Bainbridge.

**Sidney Dekker - [The Field Guide to Understanding Human Error](https://www.routledge.com/The-Field-Guide-to-Understanding-Human-Error/Dekker/p/book/9781472439055)** (2014)

Reframes "human error" as symptom, not cause. The question isn't why people make mistakes, but why their actions made sense at the time. Useful when investigating incidents involving AI-assisted work.

**Nancy Leveson - [Engineering a Safer World](https://mitpress.mit.edu/9780262533690/engineering-a-safer-world/)** (2011)

Systems-theoretic accident model. Leveson argues accidents aren't component failures but control failures - the wrong constraints, or constraints not enforced. Relevant when AI becomes part of the control structure.

**David Woods - [Four Concepts for Resilience](https://www.researchgate.net/publication/276139783_Four_concepts_for_resilience_and_the_implications_for_the_future_of_resilience_engineering)** (2015)

Distinguishes four meanings of "resilience": rebound, robustness, graceful extensibility, sustained adaptability. Clarifies what we actually mean when we say we want resilient systems.

## Trust and verification

**Leslie Lamport - [Time, Clocks, and the Ordering of Events in a Distributed System](https://lamport.azurewebsites.net/pubs/time-clocks.pdf)** (1978)

Not about AI, but about the fundamental problem of knowing what happened and in what order. Relevant to any system where you need to understand and audit automated behaviour.

**Charity Majors - [Observability Engineering](https://info.honeycomb.io/observability-engineering-oreilly-book-2022)** (2022)

The practical guide to building systems you can actually understand in production. The "observable" in my [observable, reversible, enforceable](https://cronyn.co.uk/writing/observable-reversible-enforceable.html) framework owes a lot to this.

**Cynthia Rudin - [Stop Explaining Black Box Machine Learning Models](https://arxiv.org/abs/1811.10154)** (2019)

The argument against post-hoc explainability. If you can't understand the model, explanations of its outputs are unreliable. For high-stakes decisions, build interpretable models instead. Directly relevant to regulated environments.

**Chip Huyen - [Designing Machine Learning Systems](https://www.oreilly.com/library/view/designing-machine-learning/9781098107956/)** (2022)

The production ML book. Covers data quality, monitoring, drift detection, and the full lifecycle. Operationalises "observable, reversible, enforceable" for machine learning.

## AI in practice

**Simon Willison - [simonwillison.net](https://simonwillison.net/)**

Nobody documents their AI usage more thoroughly. His TILs and link blog are a running record of what works and what doesn't. Worth following.

**Andrej Karpathy - [Software 2.0](https://karpathy.medium.com/software-2-0-a64152b37c35)** (2017)

The framing that code is being replaced by data. Written before LLMs, but sets up the question: if the code writes itself, what does the programmer do?

**Dan McKinley - [Choose Boring Technology](https://mcfunley.com/choose-boring-technology)** (2015)

Not about AI, but about the cost of novelty. Useful counterweight when everyone wants to adopt the latest model.

## Building engineers

**John Allspaw - [The Infinite Hows](https://www.kitchensoap.com/2014/11/14/the-infinite-hows-or-the-dangers-of-the-five-whys/)** (2014)

Why root cause analysis fails and what works instead. Allspaw's Learning from Incidents work addresses how engineers develop judgement, which is the skill AI might erode.

**Will Larson - [Staff Engineer](https://staffeng.com/book)** (2021)

How senior engineers create impact beyond writing code. Useful framing for what engineers should develop toward, even as AI changes the path there. I explored the junior end of this question in [Building engineers in the age of AI](https://cronyn.co.uk/writing/ai-as-junior-engineer.html).

## Financial services context

**Andrew Haldane - [The Dog and the Frisbee](https://www.bankofengland.co.uk/speech/2012/the-dog-and-the-frisbee)** (2012)

Bank of England speech on complexity in financial regulation. The argument: simple rules often outperform complex models. Relevant to thinking about where AI helps and where it doesn't.

**Man Group Research - [Machine Learning Papers](https://www.man.com/maninstitute/)**

The Oxford-Man Institute publishes good work on machine learning in finance. Worth browsing.

**Marcos López de Prado - [Advances in Financial Machine Learning](https://www.wiley.com/en-us/Advances+in+Financial+Machine+Learning-p-9781119482086)** (2018)

Rigorous treatment of ML in finance. The chapters on backtesting pitfalls alone justify the price. Written by someone who's deployed these systems at scale.

**Emanuel Derman - [Models.Behaving.Badly](https://www.simonandschuster.com/books/Models-Behaving-Badly/Emanuel-Derman/9781439164990)** (2011)

"Theories describe what something is. Models describe what something is like." A quant philosopher on the limits of quantitative models. Useful corrective when AI predictions feel like certainty.

## My own writing

**[Observable, reversible, enforceable](https://cronyn.co.uk/writing/observable-reversible-enforceable.html)**
The framework for AI systems you can trust. What each term means, why it matters, and how to apply it.

**[Trust, not capability: the real bottleneck in AI-assisted engineering](https://cronyn.co.uk/writing/trust-not-capability.html)**
The core argument: we have capable AI, we lack the infrastructure to trust it.

**[Building engineers in the age of AI](https://cronyn.co.uk/writing/ai-as-junior-engineer.html)**
If AI handles the work that used to train junior engineers, how do we develop the next generation?

**[Bainbridge's Ironies of Automation, forty years on](https://cronyn.co.uk/writing/ironies-of-automation.html)**
Applying a 1983 paper on industrial automation to modern AI-assisted software development.

---

## About this list

I'm [Ivan Cronyn](https://cronyn.co.uk), Principal Engineer & Head of Solutions Technology at Man Group. This list reflects what I've found useful thinking about AI in production financial software. It's not comprehensive and it's not neutral - these are the things that shaped my thinking.

Suggestions welcome via issues or pull requests.

---

## Changelog

- **February 2025**: Added safety and resilience section (Cook, Dekker, Leveson, Woods). Expanded trust section (Rudin, Huyen). Added building engineers section (Allspaw, Larson). Expanded financial section (López de Prado, Derman). Restructured with reading trails and cross-references.
- **January 2025**: Initial list
