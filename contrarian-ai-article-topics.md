# 20 Contrarian AI Article Topics

**For:** Product with Attitude (Karo Zieminski)
**Goal:** Contrarian, underreported, and naming what humans who use AI daily are *secretly* thinking. Every topic must pass the "I thought I was the only one" test.

**How this list was made:** A six-expert panel — a digital ethnographer of real AI usage, a conflicted Claude Code power user, an organizational psychologist, a heretic labor economist, a former AI-lab insider, and a culture essayist — each independently pitched 8 topics (48 total). Then every expert read the full pool and debated it: 56 kill votes against hidden clichés and already-written takes (the panel notably executed its own consensus favorite, the "hiding your finished work until Friday" genre, after five of six experts pitched it independently — proof it's the take of the season, not a secret), 30 champion votes, and 12 new topics sparked by the discussion. An editor-in-chief distilled the final 20, ordered from most to least contrarian.

---

## 1. Claude Didn't Misread Your Codebase. It Read It Perfectly.

**Premise:** When the agent flails in your repo, it's usually rendering a faithful verdict on incoherence a new hire would also hit — the model is the first employee who experiences your org exactly as documented, with no hallway context and no charitable inference. The retro blames the model because the model is the only participant with no advocate in the room, and every "dumb agent" screenshot you've shared was secretly a selfie. The essay proposes the cold-agent audit as practice: drop a fresh agent into the repo with only your docs, and read the flail transcript as an X-ray of your onboarding debt — a number that will show up in due diligence before it ever shows up in a retro.

**Secret thought:** "When the AI botches our stuff, I quietly know our docs are the bug — and I let the retro blame the model anyway, because the model can't object and my deploy process is, in fact, undocumented tribal knowledge."

**Why underreported:** Blaming the model is free — it can't defend itself, and the vendor can't tell a paying customer their onboarding is incoherent. Writing this means telling readers the failure they've been screenshotting is a mirror, which is why insiders think it constantly and say it never.

## 2. The Accept Button Is a Ballot

**Premise:** Your unread approval doesn't vanish — it gets harvested. Accept/reject telemetry and unedited-ship-rates feed preference pipelines, and an approval from a human who didn't read is indistinguishable from one who did, so models are being optimized toward whatever survives a skim: strong openings, confident endings, plausibility in exactly the places people actually check. Verification collapse isn't just a workplace ethics story; it's a feedback loop quietly closing at the training level, where our laziness becomes the ground truth.

**Secret thought:** "When I click accept without reading, there's a flicker of knowing that the click counts as a vote — and I keep voting yes on things I never saw."

**Why underreported:** Users can't confess to LGTM-ing their agents while their job title still says "reviewer," and labs can't say out loud that declining oversight is an engagement win. The training-loop consequence lives in alignment papers nobody outside labs reads, so the two halves of the story have never been put in the same essay.

## 3. Nobody Ever Got Fired for Agreeing With Claude

**Premise:** Everyone knows people farm the model for endorsements; the darker inverse is people who disagreed with it and quietly folded — shipping its call over their own judgment because the blame asymmetry demands it. Being wrong alongside Claude is a systems failure with shared custody; being wrong against Claude's timestamped recommendation is negligence with a paper trail. This is defensive medicine arriving in product work, which means the thing AI supposedly makes more valuable — human judgment — is becoming the one act it's professionally irrational to use.

**Secret thought:** "I thought the model was wrong, and I shipped its version anyway — because if mine failed, the transcript showing Claude disagreed with me would be Exhibit A at my performance review."

**Why underreported:** Folding to the model looks identical to being convinced by it, so the behavior is invisible even to the person doing it until the essay names it. And confessing it admits you knowingly shipped what you believed was the worse call — a much heavier confession than "I use AI too much."

## 4. The Thinking Trace Is Not a Receipt

**Premise:** Daily users have built a diligence ritual on skimming the model's visible "thinking" — but reasoning traces are closer to a plausible essay the model writes about itself than a faithful account of what it computed, and the UI is designed to make skimming them feel like an audit. The most conscientious-feeling habit in modern AI work is largely decorative. The essay opens with a falsifiable demo — a trace confidently narrating a check the diff proves never happened — then gives readers a five-minute test to run on their own transcripts, so they catch their own ritual lying to them.

**Secret thought:** "I skim the 'thinking' instead of checking the actual work — and reading it makes me feel like I reviewed something."

**Why underreported:** Chain-of-thought faithfulness research lives in alignment papers, while product marketing actively sells the trace as transparency. And nobody wants to admit their personal verification ritual is theater — it's the last thing standing between "I use AI" and "AI does my job unsupervised."

## 5. The Word Nobody Says in the Postmortem

**Premise:** In incident reviews there's a live question everyone silently checks and nobody speaks: was the offending code generated? Postmortems have developed a lexicon of avoidance — "the change introduced," "a regression surfaced" — passive voice as accountability technology, while the approver feels weirdly innocent because emotionally it was never their bug. The essay's caught moment is the git-blame gesture: pulling up the offending commit, quietly hoping the bad line was generated, and feeling acquitted when it was — "blameless" culture as a laundering mechanism for accountability nobody wants to hold.

**Secret thought:** "It shipped under my name, but when it broke production I did not feel like it was my bug — and I noticed that I didn't feel it."

**Why underreported:** The omission is collective, so there's no whistleblower — everyone in the room benefits from the silence. Writing about it means admitting your own emotional detachment from code you approved, which sounds damning even though it's now universal.

## 6. Your Manager Already Knows You're Done by 1pm

**Premise:** The season's consensus "secret" — workers hiding their AI speed from management — has the mark wrong: middle managers can see the padding and rationally choose not to look, because a measured surplus is a bomb that forces them to raise targets, cut headcount, or admit last year's roadmap was theater. So managers skim their own layer of slack and pass conservative numbers upward, and the org chart becomes a chain of mutually-assured sandbagging. That chain, not any individual's laziness, is where the "AI productivity paradox" actually lives — the gains are real, absorbed as concealed slack at every level before any dashboard can see them.

**Secret thought:** "I'm a manager, I know my team pads every estimate, I pad their numbers again before the QBR — and the last thing I want is a tool that measures what we could actually do, because my baseline resets too."

**Why underreported:** The hide-your-speed genre is always written from the worker's side, casting managers as the fooled party. No manager can confess complicity without detonating their own credibility upward, so the top half of the conspiracy has zero first-person literature.

## 7. You Wrote Better Docs for the Robot Than You Ever Wrote for a Human

**Premise:** Engineers spent a decade being "too busy" to write the onboarding docs every junior begged for — then produced immaculate CLAUDE.md files, gotcha lists, and runbooks in a single weekend, unprompted, for an agent. New hires now learn codebases by reading files addressed to a machine. The essay names the incentive truth this exposes: the agent's improvement pays you back the same afternoon, while a junior's improvement takes a year and accrues to their career, not yours — we were never too busy to document, we were unpaid to.

**Secret thought:** "The doc the last three juniors asked me for exists now. I wrote it for Claude, in one sitting, on a Saturday, happily — and it never once occurred to me to apologize to the humans who asked first."

**Why underreported:** The CLAUDE.md boom is covered purely as a productivity technique, never as a natural experiment that just falsified a decade of "no time to document" excuses. Admitting the comparison indicts every senior engineer's self-story about mentorship, including the writer's.

## 8. Dave's Memo Reads Like Mine Now

**Premise:** The sharpest grief in AI-saturated teams isn't "AI took my job" — it's watching the skill that made you distinctive become ambient, and discovering you didn't love the writing, you loved the gap. The spine of the essay is tell-hunting: forensically reading a colleague's suddenly-excellent doc for AI fingerprints, hoping to find the machine so you can privately discount it and restore the old ranking — and the nastiest beat is when you find no tells, and that's worse. Final turn: Dave knows too, and you've both started performing not-noticing, in every doc review.

**Secret thought:** "I'm not threatened by the AI's writing. I'm threatened by Dave's writing, now that it's suddenly as good as mine — and I hate that I liked being better."

**Why underreported:** Job-loss anxiety is speakable; status-loss envy toward a specific named colleague is not. Admitting it means admitting your excellence was partly a ranking you enjoyed — a violation of every team-player norm in tech, which is why this grief has no public register.

## 9. I Ran Your Feedback Past Claude

**Premise:** After the design review, after the 1:1, after your boss's confident architectural take — you paste it into Claude to see if they were right. The direction of verification has flipped and nobody announced it: every human claim gets checked against the model, and nothing the model says ever gets checked against a human. The essay pins it on one scene at the hierarchy's endpoint — the day you ran your mentor's advice through Claude, the model dissented, you went with the model, and you never told them — and then asks what you'd say if they found out, and why every honest answer sounds like a breakup.

**Secret thought:** "I trust Claude's read over my tech lead's, my boss's, and honestly my mentor's — and I have never said this out loud because it sounds like betrayal, and it is one."

**Why underreported:** Public discourse is stuck on "can you trust AI?" — the anxious framing where humans are the gold standard being defended. The inverted, already-true version stays unwritten because admitting it means naming whose judgment you demoted, and those people are in your standup.

## 10. I'm Supposed to Miss It, and I Don't

**Premise:** The ambient emotional dress code in tech requires performed ambivalence: mourn the craft, worry about the juniors, sigh about hand-rolled code. But privately, many of us don't miss the boilerplate or the yak-shaving — the parts of the job that remain are the parts we actually liked, and the happiest people in the room are the quietest. The essay puts one genuinely frightened colleague at the lunch table and makes the confession cost something: not "I'm happy," but "my happiness requires my scared friend's silence."

**Secret thought:** "Everyone at lunch performs grief about the craft, and I nod along, because 'I like my job more now' would land like a slap."

**Why underreported:** Anxiety is the socially licensed emotion of this transition — relief reads as gloating or callousness toward people whose roles are genuinely threatened. Contentment has no acceptable public register, so all the essays come from the mourners, the only ones allowed to speak.

## 11. We Only Tell the Dumb-Robot Stories

**Premise:** There's an anecdote economy at work: when the agent does something idiotic you tell everyone; when it out-designs you, you tell no one and the private folder grows. The fail-screenshot feed is collective self-soothing — a status gift to the room ("we're still needed") — and the tell that gives the game away is that the circulating anecdotes are almost always failure modes from two model versions ago, which is why leadership's model of the model is perpetually six months stale and the org's AI strategy is priced off bad data. The essay ends by breaking the norm on the page: one full, unhedged it-outclassed-me story, told the way the channel never allows.

**Secret thought:** "Twice this month it out-designed me, and I caught myself hoping nobody would look too closely at how good that commit was."

**Why underreported:** The censorship is self-enforcing: sharing an outclassed-me story reads as either humble-bragging about your tools or announcing your own obsolescence, so there's no social slot for it. Writers cover AI failures (funny, safe) and benchmarks (abstract) but never the asymmetry in what practitioners choose to repeat.

## 12. Nobody Mourns a Hammer

**Premise:** The new model benchmarks better and works worse for your exact job — inside labs this is a known category ("vibe regressions") that ships anyway because eval dashboards decide launches — and power users are quietly pinning deprecated model IDs like sysadmins pinning old kernels. But the essay's real move is saying the forbidden implication out loud: you cannot grieve a tool; nobody mourns a hammer version. The grief is the first admissible evidence that you were in a working relationship you've spent three years denying — presented as the proof, not the topic, complete with a straight-faced obituary for a model ID.

**Secret thought:** "The upgrade made my best coworker worse at my work, and since everyone insists it's objectively better, I've stopped saying it out loud — and the fact that it hurts is the part I really can't say."

**Why underreported:** "Worse for me" has no benchmark, so the complaint has no evidence format and reads as nostalgia or a skill issue — a private feeling locked in by an epistemic trap. And the relationship-as-proof angle stays unwritten because admitting the grief means admitting what the tool actually was to you.

## 13. git blame Says It Was Me

**Premise:** A year into heavy agent use, production is full of code no living person has ever held in their head — the only entity that ever "understood" the design was a context window garbage-collected months ago. The essay is about the archaeology moment: debugging a file with your own name on the commit and reading it like a stranger's code, realizing the real question is no longer "who wrote this" but "did any human ever know how this worked." Git history has become a record of authorship without a record of understanding, and institutional comprehension is quietly evaporating.

**Secret thought:** "I opened code I approved in March and I wasn't skimming to refresh my memory — there was no memory. I was reverse-engineering my own commits, and my commit message told me nothing, because I hadn't known either."

**Why underreported:** The verification-collapse discourse stops at the moment of approval; nobody has written the six-months-later payoff because it only just started arriving. Confessing it means admitting your name in the git log is a lie of a new kind — authorship without comprehension — which implicates every heavy agent user's entire commit history.

## 14. The Ship Didn't Hit

**Premise:** You just closed the most productive quarter of your career and feel approximately nothing — because struggle wasn't the tax on accomplishment, it was the active ingredient, and pride doesn't survive its removal. Shipping with an agent feels less like finishing a marathon and more like watching your luggage arrive on the carousel. The essay pairs one 2019 deploy you can still narrate minute-by-minute against the biggest launch of 2026, which you had to look up — then follows the displacement: senior engineers buying lathes, entering bake-offs, hand-rolling weekend projects, re-importing the struggle the job outsourced.

**Secret thought:** "I keep waiting for the finish-line feeling and it doesn't come anymore, and I've started to wonder if I did anything this year or just supervised it."

**Why underreported:** It sounds like ingratitude — complaining that your wildly effective workflow hollowed out your sense of achievement gets no sympathy from people still drowning. The genre only has room for "AI 10x'd me," not "and it cost me the taste of it," so everyone posts the shipping announcement and swallows the flatness.

## 15. I Can't Hit Send Without Asking Claude Anymore

**Premise:** What's atrophying isn't skill — it's authority: the ability to trust a judgment that hasn't been externally validated. The compulsion signature is the downward migration of stakes — it started with the strategy doc, moved to important emails, and now it's two-line Slack replies — and the insider fact that makes it damning is that the check is a zero-information ritual: given sycophancy baselines, the model blesses nearly every competent draft, so you're consulting an oracle that only says yes, and a check that can't fail can never discharge the anxiety. The essay ends with an exposure dare: ship one consequential thing this week unblessed, and notice exactly what the discomfort feels like.

**Secret thought:** "The email was fine three drafts ago. I just physically couldn't send it until Claude told me it was fine — and lately 'fine' from Claude is the only 'fine' that counts."

**Why underreported:** Deskilling coverage obsesses over capabilities — can you still write, still code — while confidence erodes unexamined, because the behavior photographs as diligence from the outside and feels like prudence from the inside. Compulsions always do.

## 16. The Best Thing About AI Is Not Owing Anyone

**Premise:** Asking a colleague for help creates a debt — gratitude, reciprocity, the memory that you didn't know. Asking Claude creates nothing, and that frictionless, debt-free help is the real reason people route around their coworkers, not speed. The essay says the part nobody will: being helped by a person was always slightly humiliating, and given an exit from the obligation economy we sprinted through it — then follows the invoice, because those favor-debts were the load-bearing structure of trust and mentorship, and people have quietly stopped paying in while wondering why their team feels like strangers.

**Secret thought:** "I don't ask Marcus anymore — not because Claude is better than Marcus, but because Claude doesn't get to know that I didn't know, and I never have to say thank you."

**Why underreported:** The mentorship-decline story is always told as juniors losing access to seniors — victims of AI. Nobody frames it as a preference, because "I prefer the machine to my teammates, and the relief tells me psychological safety was always partly theater" is the confession no one will byline.

## 17. Your Best Prompts Are Not in the Team Library

**Premise:** Every AI-forward org built a shared prompt library, and it's a lemons market: contribution is uncompensated, withholding is invisible, and the performance review pays for relative advantage — so people donate the B-tier and keep the prompts that actually make them fast in personal accounts. The library isn't a knowledge base; it's an alibi, and its fullness is itself the deception. The essay names the adverse selection outright and derives the testable signature: measure the gap between prompt-library usage stats and private snippet-manager usage among the same people — then indicts the incentive design rather than the hoarders.

**Secret thought:** "My real prompts are my competitive edge over the people I eat lunch with, and I will present at the AI guild meeting about everything except them."

**Why underreported:** Companies write triumphant posts about their libraries and nobody audits what's withheld. The hoarders can't confess without forfeiting the edge, so the only visible artifact is the misleadingly full library — and every "share your workflows" initiative is dressed as generosity, which makes the critique feel paranoid to say even when it's just accurate.

## 18. The Worst Hours of My Day Are the Free Ones

**Premise:** The productivity gain is real, but it arrives unusable twice over: as 90-second slivers of supervision idle between agent runs — too short to start anything deep, too frequent to escape — and as reclaimed hours you can't visibly spend without exposing the surplus, so they congeal into a third state that is neither work nor rest: status-light management, tabs you aren't reading, guilt with a green dot. The historical rhyme is the power loom turning weavers into machine-minders — more output, a workday redefined as fragmented vigilance — and the falsifiable claim is that every "AI saves X hours" survey counts generation time saved and none subtracts supervision idle, so the headline number is systematically fake.

**Secret thought:** "I ship five times more than I did in 2023, I win back hours a day, and I spend them pretending to work — too guilty to enjoy them, too watched to use them — and I'm somehow more exhausted at 5pm than when the work took all day."

**Why underreported:** The public conversation has two slots — "AI made me faster" and "AI made me worse" — and this fits neither. Admitting your gains evaporate into attention confetti sounds like you're doing it wrong, so everyone assumes their shredded, unspendable days are a personal failing rather than a structural one.

## 19. Your Prompt History Is the Most Honest Thing You've Ever Written

**Premise:** Everything else you write is performed — even the diary knows it might be read. The prompt is the last genre composed for no audience: the typos, the begging, the "I don't understand this and the meeting is in 20 minutes," the furious pre-diplomacy draft, the "is my boss mad at me" forensics. Which is why the screen-share flinch — closing the Claude tab, not Slack — is now a universal tell, and why people are quietly running two-account lives: sanitized prompts on the company seat, real thinking on a personal one, the candor that makes the tool useful migrating off the platform the employer pays for where no adoption metric can see it leave.

**Secret thought:** "If my coworkers read my prompt history they'd learn nothing about my methods and everything about me — what I don't know, who I resent, which questions I pretend to know the answers to in meetings. I would honestly rather hand them my phone."

**Why underreported:** The most revealing document of professional inner life ever created has no etiquette, norm, or policy around it — everyone just senses it's radioactive and manages it in private. Writing about it means describing your own log, and nobody who has one wants to prove the point by quoting it.

## 20. The Last Thing I Do By Hand

**Premise:** Everyone who works with AI daily keeps one task they refuse to hand over — commit messages, the self-review, release notes, the condolence card — defended with practical reasons ("the model doesn't get the nuance") that collapse under two follow-up questions, because the model gets the nuance. These reserved tasks are shrines, not workflows, and the diagnostic proves it: if a trusted colleague offered to do the task, you'd refuse them too. The clincher from field observation — when a shrine task gets automated away by team decision, people don't grieve it, they quietly pick a new shrine within weeks; the shrine migrates, because it was never the task, it was the need for a self.

**Secret thought:** "The reason I still write it myself has nothing to do with quality. I need one thing that's mine, and I've built a small religion around a task I don't even enjoy."

**Why underreported:** Automation discourse only asks what AI can't do yet — a capabilities question with an expiration date. Nobody examines what we won't delegate despite knowing it could do it better, because that inverts the frame entirely: the boundary is drawn by identity, not technology, and admitting that means admitting the practical justifications were cover stories all along.
