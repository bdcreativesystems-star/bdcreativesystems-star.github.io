---
title: "Why RiskLens CI Almost Broke Me (And the One Phrase That Fixed Everything)"
date: 2026-03-21
tags: [AI, DevOps, GitLab, Automation, RAG, MachineLearning]
---

## The Beginning Looked Simple

When I started building **RiskLens CI**, the idea actually made sense to me.

- Trigger on a GitLab merge request  
- Analyze code changes  
- Return risk level, issues, and recommendations  

Conceptually… I understood it.

But the system itself? Completely different story.

![RiskLens Initial State](/assets/images/risklens-start.png)

It was running. The endpoint responded.

And I thought… *okay this should be working.*

It wasn’t.

---

## This Felt More Advanced Than Anything I’ve Built

I’m going to be real here — this project felt advanced for me.

Not because I couldn’t understand the idea…

But because:
- The system behavior was unfamiliar  
- The feedback loop wasn’t obvious  
- And small mistakes didn’t break things — they just made them worse  

That part messed with me.

---

## The “Almost Working” Stage Is the Worst

Everything looked like it was firing correctly:

- Webhook → ✅  
- Backend → ✅  
- AI processing → ✅  

But the results?

- Slightly off  
- Missing detail  
- Not as “smart” as I expected  

That’s when frustration really started setting in.

Because nothing was clearly broken.

---

## Risk & Predictive Systems Are Not Forgiving

This is something I didn’t expect:

> Risk assessment systems and predictive outputs are extremely sensitive.

If you’re not precise:
- The risk score becomes meaningless  
- The issues feel generic  
- The recommendations lose value  

And that’s exactly what I was seeing.

It wasn’t wrong… it just wasn’t useful.

---

## What I Was Missing (And Didn’t Realize)

This is what took me the longest to understand:

> I wasn’t missing logic — I was missing *language*

Sometimes it was:
- One phrase in the prompt  
- One missing instruction  
- One unclear expectation  

And that tiny gap changed everything.

---

## When It Finally Clicked

This is when it started to feel real:

![RiskLens Terminal Output](/assets/images/risklens-terminal.png)

Now I was getting:

- 🔺 **Risk Level: HIGH (75/100)**  
- Clear summary of what was happening  
- Real issues tied to configuration + authentication  
- Recommendations that actually made sense  

This wasn’t just output anymore.

This felt like a system.

---

## What Changed Everything

I stopped thinking:

> “Why isn’t this working?”

And started thinking:

> “What EXACTLY am I not telling the system?”

That shift helped me:

- Tighten my prompts  
- Be explicit about output format  
- Remove assumptions  
- Treat the AI like a strict executor  

And that’s when everything came together.

---

## The Frustration Was Real

There were moments where I felt like:

- I was going in circles  
- The system was reacting but not improving  
- I was right there… but couldn’t see what was missing  

That “almost working” phase is exhausting.

But it’s also where everything starts to click.

---

## What I Learned

### Precision > Complexity  
Even simple ideas break without clear instructions.

### AI Doesn’t Guess  
If you don’t say it, it won’t do it.

### Predictive Systems Require Control  
You can’t be vague with risk analysis — you have to define everything.

---

## Final Thoughts

If you’re building AI systems and feel stuck…

You’re probably not far off.

You might just be missing:
- one phrase  
- one instruction  
- one piece of clarity  

And once you find it — everything changes.

---

## What’s Next

I’m continuing to evolve RiskLens CI into:

- AI-powered code review assistant  
- Multi-agent analysis workflows  
- Automated fix + deployment previews  

This is just the beginning.

---

*If you're building something and it feels frustrating — especially with AI — you're not alone. You're probably closer than you think.*