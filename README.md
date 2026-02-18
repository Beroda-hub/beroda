# Derek Manning
Breaking things. Fixing things. Writing down what I learned, one mistake at a time.

It’s a living document of things I’ve broken, fixed, misunderstood, optimized, and learned the hard way. I’m a cybersecurity student, but a lot of what I’ve learned hasn’t come from lectures — it’s come from troubleshooting at weird hours, staring at logs, and realizing the problem wasn’t what I thought it was.

I’m building this repo as something I’ll keep adding to over the years and something i can look back on and remember.

---

## Servers & Virtualization

I started diving deep by managing virtual machines on ProxMox. 

Things I ran into:
- Tick lag and CPU MHz bottlenecks.
- Misunderstanding that allocated CPU isn’t always usable CPU.
- Broken Linux packages and repository errors.
- Backup and restore processes for persistent services.

**What I learned:**  
Virtualization hides complexity but doesn’t remove it. Logs tell the more than dashboards.

---

## JVM & Launch Scripts

While working with modded servers, I had to manually edit startup scripts and JVM arguments when things didn’t launch correctly.

Challenges:
- Broken runtime paths.
- Incorrect Java references.
- Arguments pointing to files that didn’t exist.

**What I learned:**  
Trace execution. Read the scripts. Understand what’s actually being run before hitting “reinstall.”

---

## VPN & System Boundaries

Setting up Global Protect (for school) led me into an embedded browser authentication loop that just kept crashing.  

Root cause: system-level browser defaults — not the VPN client itself.

**What I learned:**  
Most problems live at the boundaries between systems, not inside the obvious component.

---

## Security Thinking

I’ve studied both theory and real-world breaches:
- Key exchange protocols
- Malware mechanics (viruses vs worms)
- Information hiding
- CAPTCHAs
- Threat and vulnerability modeling
- Shannon entropy and information measurement

I also analyzed Target's breach. Breaking it down taught me that failures aren’t flashy; they’re chains of tiny oversights.

---

## Math & Foundations

Calculus and logic might seem abstract, but they show up everywhere:
- Chain rule, implicit differentiation, higher-order derivatives
- Newton’s method, Mean Value Theorem
- First and second derivative tests
- Boolean algebra, canonical forms
- Linked list deletion and time complexity
- Entropy calculations

**What I learned:**  
Math explains how systems behave. Once you see the connection, it stops being abstract.

---

## Optimization Mindset

Even in games I analyze systems:
- Modded Minecraft server performance
- CPU allocation and tick-rate behavior
- Talent builds and gear synergy in complex RPGs

I naturally look for trade-offs, efficiency curves, and constraints. Optimization mindset transfers everywhere.

---

## Patterns in My Failures

Things I used to do:
- Assume the obvious cause was the real cause
- Reinstall instead of investigate
- Change multiple variables at once
- Blame hardware immediately

Things I try to do now:
- Reproduce issues
- Change one variable at a time
- Verify assumptions
- Look at boundaries between systems
- Ask what layer I’m actually debugging

Methodical beats fast every time.

---

## Current Focus

Right now, I’m interested in:
- Defensive security engineering
- Systems reliability
- Infrastructure performance
- Cryptography and math behind security

Expect this page to grow and evolve as I learn more
