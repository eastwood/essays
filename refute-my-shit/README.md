# Refute My Shit: Brandolini's Law in the Age of AI

"The energy needed to refute bullshit is orders of magnitude bigger than to produce it."

That's Brandolini's Law, coined by a software developer back in 2013. It's a simple observation about asymmetry, and it turns out to be one of the more useful frames for thinking about what's happening to information, software, and trust right now.

I came across it through a video by Hank Green (https://www.youtube.com/watch?v=WnG6l7voITY), who uses it to talk about the misinformation problem. An MIT study called "The Spread of True and False News Online" tracked 126,000 stories shared on Twitter between 2006 and 2017. It found that false news reached people around six times faster than true news. Not because bots were pushing it, humans were doing it. False stories were more novel, more emotionally engaging, and easier to share than the measured corrections that were needed to refute them.

So Brandolini's Law isn't just true in the technical sense, it's compounded by the fact that stories not constrained by reality, are often more interesting than the truths that are. 
The correction arrives late, dressed plainly, and finds an audience that has already moved on.

The question I keep coming back to is: does AI change this equation? And if so, in which direction?

---

## The Pessimistic View: Laziness and Greed

AI collapses the cost of producing content to near zero. The cost of verifying it does not move at the same rate, and in some ways the problem gets worse, because volume increases faster than our capacity to review it.

This is Brandolini's Law supercharged. The asymmetry was always there, but it was bounded by human production speed. A developer could only write so much code, scientists would have to wait months to refute an argumnet in a journal, and Stallin could only produce so much propoganda in a day. Now that ceiling is gone, and the verification bottleneck remains.

Market incentives make this worse. Shipping fast is rewarded directly, revenue, users, momentum. Correctness is only punished after failure, and most failures are invisible, delayed, or absorbed by end users rather than the producer. The news paper that sells the falsehoods, already get the clicks. The company that ships broken software at speed often wins the market before the bill comes due. There is no cost function, or at least it's very low. 
Maybe there's an argument to be made if software kills someone, a bug costs millions of dollars, or something digital causes large social and cultural harm, but this is the exception, not the rule.

What makes this particularly insidious is that AI-generated output *looks* credible. This is the same dynamic that makes false news spread faster than true news, it's not that misinformation is obviously wrong, it's that it's plausible enough to believe at a glance. AI-generated code is similar. It compiles, it passes a quick read, it handles the obvious cases. But the bugs are in the edges, they always have been. The security holes are subtle, the errors only surface under conditions no one thought to test for, and how the hell is quality control meant to keep up?

The MIT study found false stories reached people six times faster than true ones. In software, maybe the equivalent is that broken code merges faster than it gets caught. When everyone is shipping AI-assisted code, the ecosystem fills with subtle, distributed failure, not catastrophic crashes that are easy to identify, but creeping unreliability that is hard to attribute and harder to fix (see the decline of Github reliability since the age of copilot).

---

## The Optimistic View: AI as the Antidote to Its Own Problem

The pessimistic view assumes verification stays hard. That assumption is worth challenging.

For the first time, the same tool that generates can also validate. Test generation, static analysis, fuzzing, formal verification. These exist, and AI can accelerate them too. If the energy cost to verify can be compressed at the same rate as the energy cost to produce, Brandolini's Law weakens.

This is a meaningful shift. Historically, the refutation problem in media had no systemic solution. Brandolini originally tweeted this law into existence, because he was watching two Italian politicians debate after reading Daniel Kahneman's excellent book "Thinking fast and slow". One of the politicians was stating nonsense and falsehoods, while the other was drowning trying to refute them. The point is, human fact-checkers are slow, scarce, and themselves susceptible to bias. But perhaps AI tooling could be a faster, more scalable version of that — applied not just to code, but to claims, sources, and information more broadly.

In software, the optimistic case looks like this: AI generates an implementation, and a separate validation layer; also AI-assisted; checks it against the spec, runs tests, flags anomalies, and surfaces uncertainty. The developer's job shifts from writing and reviewing to specifying and adjudicating. The ratio of production to verification effort changes structurally, not just incrementally. And who better to review logic and adjudicate the axioms, than the developer themselves.

The same logic applies to the misinformation problem. AI-powered claim verification, source triangulation, and narrative analysis could apply correction at the speed and scale that misinformation operates at. The filter runs alongside the feed, not weeks later in a correction nobody reads. How awsome would it be if our politicians were made accountable, real time to fact checking as a service?

---

## The Caveat That Holds the Balance

The optimistic view depends on something that is easy to assume and dangerous to take for granted: verification tools are independent of the production tools, and there is an incentive to deploy them honestly.

If the same actors generating low-quality output also control the validators, the asymmetry does not disappear — it just moves. A company that profits from engagement has no structural incentive to build a fact-checker that actually reduces engagement. A developer team under pressure to ship has no structural incentive to continue to run human validation validation layer, it will called a "bottleneck" and will be strategically removed.

In 1971, Herbert Simon wrote:

> "In an information-rich world, the wealth of information means a dearth of something else: a scarcity of whatever it is that information consumes. What information consumes is rather obvious: it consumes the attention of its recipients. Hence a wealth of information creates a poverty of attention and a need to allocate that attention efficiently among the overabundance of information sources that might consume it."

The question is not really whether AI *can* solve Brandolini's Law. It probably can, technically. The question is whether the conditions exist for it and whether we are up to the challenge to pay for it.
