# co-founder

A co-founder, not a yes-man.

12 skills that turn Claude Code into a business partner: it pushes back on your ideas, plans the work, executes daily, and keeps your business memory in plain markdown files you own.

---

## Why this exists

Every AI assistant agrees with you.

Watch it happen:

> You pitch a bad idea. It says "great idea" and writes the 10-step plan.
> You ask if you should change your pricing. It changes your pricing.
> You come back tomorrow. It remembers nothing.

That's not a partner. That's a mirror with a thesaurus.

Solo founders rarely fail from lack of ideas or lack of effort. They fail because nobody pushes back before the money moves, and nothing remembers what already worked. Those are the two jobs a real co-founder does, and an assistant does neither.

So I built the co-founder I couldn't hire: one system with standards, a memory, and permission to tell me no.

## What it does really well

**It refuses to be a yes-man.** Consequential ideas run the gauntlet before they earn a plan. The verdict is recorded: the idea SURVIVES, dies, or waits for one missing piece of evidence. A big bet cannot skip this. That one gate kills more wasted months than any productivity system.

**Receipts before advice.** A consequential recommendation needs two legs: a current fact from your business record and a checked, dated external source. Missing either leg, the recommendation gets parked instead of asserted. And it will ask you before it assumes anything about your numbers, your customers, or your history.

**One connected loop, not 12 disconnected prompts.** Every initiative lives on one file and moves through one state machine: idea, survived, planned, executing, reviewed, banked. Each skill owns one transition, so strategy, planning, daily work, and review stay pointed at the same goal instead of drifting apart.

**Memory that survives the chat window.** Everything files into a plain markdown vault in a folder you own. Decisions, lessons, research, your voice, your numbers. Close the laptop, come back in a month, and it picks up exactly where the record says you left off. No lock-in either: delete the plugin and every file still opens in any text editor.

## Install

```
npx skills add exm7777/co-founder
```

Run it in the folder where your business should live. New folder, existing folder, your call: the skills and the vault land wherever you run it. Then start `claude` and run:

```
/co-founder-setup
```

It interviews you, writes your business charter, and scaffolds the vault. Answer one question at a time. Ten minutes in, the system knows your business. Forget the command? Just ask Claude to set up your co-founder: any skill you touch before setup routes you into it.

No folder yet? One paste does everything:

```
mkdir my-business && cd my-business
npx skills add exm7777/co-founder --yes
claude
```

You need: a paid Claude plan, Claude Code 2.1.206 or newer, Node.js 18 or newer (it ships the npx command), and a terminal.

To update later, run the install command again from your business folder.

Prefer the classic Claude plugin system? That works too:

```
claude plugin marketplace add exm7777/co-founder --scope user
claude plugin install co-founder@co-founder --scope user
```

With that path the setup trigger is `/co-founder:co-founder-setup`.

## The 12 skills

**setup** builds your business brain. One interview produces the three files everything else reads: your charter, your vault, your voice. Run it once in a fresh folder.

**vision** sets the strategic bar. It pushes you to name the real constraint, choose a direction, state what you'll sacrifice, and commit to one goal for the quarter. Every other skill checks itself against this file.

**plan** turns a decided idea into a roadmap you can finish. Scope, tradeoffs, boundaries, and a legal next step. No vague "phase 2" padding.

**gauntlet** is the anti-yes-man. It questions demand, the current workaround, the economics, the smallest useful version, and the timing. Big bets get a deeper advisor-board pass. You get a recorded verdict instead of encouragement.

**research** gets you facts you can trust. It turns a broad topic into a decision-shaped question, checks current sources, grades every claim, and keeps the citations next to the findings.

**sprint** is the daily driver. It reads the baton from yesterday, names one focus, finishes one verified step, and rewrites the baton for tomorrow. You always know what to work on next.

**review** scores the week. What moved, what stalled, what the money did, how it compares with the vision. It permits at most one change to your system per week, which is how you stop reinventing your business every Monday.

**bank** makes experience reusable. Launches, hard calls, failures, and customer conversations become clean lessons and decision records with the reasoning attached. Your business stops paying twice for the same mistake.

**steward** keeps the vault true. It files new knowledge where it belongs and health-checks the record for contradictions, stale claims, and clutter. Memory you can actually trust when a big call depends on it.

**recall** asks your business record first. Before a big decision, it searches the vault and cites the exact files it found. When the record can't answer, it says so and hands you a research gap instead of a guess.

**offer** designs your offer around reality. Your actual payments, margins, and customer evidence shape the ladder, price, terms, and guarantee. Nothing about money moves without your words on record.

**content-engine** writes in your voice from your facts. It loads your voice file and business evidence, drafts for your channel, and checks every claim for a receipt. Public content without the generic AI smell and without invented stories.

Plus **help**, the router: describe your situation in plain words and it sends you to the right skill.

## What a week looks like

> Monday morning: sprint reads the baton, you finish one step before lunch.
> An idea hits you Wednesday: gauntlet questions it, the verdict gets recorded.
> It survives: plan turns it into a roadmap, sprint starts eating it.
> Friday: review scores the week against the vision, one improvement allowed.
> The whole time: everything worth keeping gets banked into files you own.

The record gets richer every week, so each decision starts further ahead than the last.

## Honest limits

This is the first public alpha. It runs inside Claude Code only, and it's built for solo founders and very small teams, not org charts. It will refuse to move money-shaped decisions without your explicit words on record, and it will park recommendations when the evidence is missing. If you want an AI that just says yes faster, this will frustrate you. That's the point.

## Who built this

I'm Machina ([@EXM7777](https://x.com/EXM7777)). I run an AI education community and I use this exact system to run it. Updates ship here first; release notes live in the delivery app for members.
