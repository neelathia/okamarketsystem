
---

**The week everything contradicted itself**

Three conversations. One week. Three completely different answers to the same question.

Monday: _"We need detailed 5-page how-tos."_ Wednesday: _"AI is going to need this documentation."_ Friday: _"Just steps and screenshots — keep it simple."_

I was an OCM analyst on a major EAM implementation. My job was to support training and knowledge transfer as Hexagon replaced a legacy Maximo system across a complex railcar maintenance operation. Straightforward enough.

Except nobody could agree on what the knowledge was actually _for._

---

**The moment I stopped writing**

I could have picked a template and moved on. Most people do.

Instead I sat with the contradiction and asked a different question: _why does it matter what format we use?_

That led me to an enterprise architecture diagram — a sprawling Excel sheet mapping every system, every integration, every process flow across the operation. UMLER. Oracle eShift. BizTalk. Databridge. Hexagon talking to all of them.

I wasn't supposed to be reading that document. But once I did, I couldn't unsee it.

The how-to documents we were arguing about weren't documentation. They were the _instruction layer_ of how work actually gets done — and they were being designed with no awareness of the system they lived inside.

For example, when a campaign was activated in Asset Hub, it didn't just complete a step — it triggered updates in UMLER and depended on upstream configurations being correct. None of that showed up in the how-to.

---

**The real problem**

An experienced technician reading a how-to already carries context. They know the system, the sequence, the exceptions. They need steps and screenshots — confirmation, not explanation.

An AI system reading the same document has none of that. It needs explicit logic. Dependencies. Validation rules. What must be true _before_ a step executes. What happens when it doesn't.

The same document cannot serve both — not without being structured differently at the source.

Nobody was asking that question. So I started asking it.

---

**What I built**

I defined two distinct knowledge types — human-facing and system-facing — and started designing a routing layer: a structure that delivers the right form of knowledge based on who or what is consuming it.

In practice, that meant separating step-by-step instructions from the underlying logic — dependencies, triggers, and validation — instead of forcing both into the same document.

TTX wasn't ready to implement it fully. That's honest. But I could see clearly what was coming: AI wouldn't just retrieve this knowledge. Eventually it would _execute_ from it. And execution requires a different kind of structure than communication does.

---

**What I learned**

I didn't go looking for a knowledge architecture problem. I found it by refusing to accept that a formatting disagreement was actually about formatting.

The real question was never _how long should a how-to be._

It was _what is knowledge for when machines are doing the work._

---

Clean. The campaign example does exactly what it needs to — one sentence that makes the abstract system dependency suddenly real. And the "in practice" sentence in the build section closes the abstraction gap without over-explaining.

This version is done. Don't edit it again.