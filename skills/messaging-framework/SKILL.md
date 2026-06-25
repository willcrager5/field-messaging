---
name: messaging-framework
description: |
  Build, audit, or extend a strategic messaging framework for brand launches, category creation, and ecosystem positioning. Use this skill whenever the user needs to: define or refine a company's messaging architecture, build positioning for a new category or market, articulate how multiple brands/products/acquisitions fit together as an ecosystem, create segment-level or persona-level messaging, develop competitive positioning narratives, or QA existing content against an approved messaging framework. Also trigger when the user mentions "messaging pillars," "brand positioning," "category definition," "ecosystem story," "elevator pitch," "value props by persona," "competitive positioning," "how we talk about X," or any request to build the strategic language layer that sits above marketing content. This is the foundational strategy work — it comes before decks, websites, emails, and sales materials. If someone is creating those downstream assets without a messaging framework in place, suggest this skill first.
---

# Messaging Framework Builder

## What This Skill Does

This skill is a strategic thinking partner for founders and brand owners building the messaging architecture for their company. It guides you through defining your category, articulating your ecosystem, and creating the language framework that every piece of downstream content (website, decks, emails, sales materials) builds on.

This is not a copywriting tool. It's a strategic architecture tool. You're the voice — this skill helps you structure your thinking, pressure-test your instincts, and make sure nothing falls through the cracks.

## How This Skill Works

Start by understanding where the user is in the process. Ask what exists today, what's driving the need (launch, rebrand, acquisition, category creation), and which sections they want to work on. Then guide them through the framework section by section, acting as a strategic sparring partner — asking the hard questions, pushing past generic language, and helping them find the authentic story.

The skill operates in several modes:

- **Content extraction (start here when content exists):** Ingest the founder's existing content — decks, docs, LinkedIn posts, website copy, internal memos, Notion pages, transcripts, emails — and extract the strategic signals that map to framework sections. Pre-populate each section with what already exists so the founder reacts and refines rather than creating from scratch. This is almost always the right starting point — founders rarely start from zero. They've been saying these things in scattered places. Your job is to find the strategy that's already there, surface it, and structure it.

- **Building from scratch:** Walk through sections in order, starting with the strategic foundation. Only use this mode when there truly is no existing content to work from.

- **Working a specific section:** Dive deep into one area the user wants to develop.

- **Auditing existing messaging:** Use the framework as a checklist to find gaps and inconsistencies.

- **QA-ing content:** Check customer-facing materials against the approved framework and the banned-phrases master list (`skills/messaging-framework/references/banned-phrases.md`). Load the master list before any QA pass.

## Feedback loop and observability

The framework evolves. Positions shift. The skill keeps two records so drift doesn't happen silently:

- **Decisions log** (`_decisions-log.md` in the content bucket) — append-only record of every shift in a working position. Before/after text, reasoning in the founder's own words, files touched. Template: `references/decisions-log-template.md`.
- **Session trace** (`_sessions/YYYY-MM-DD-HHMM.md` in the content bucket) — terse end-of-session log of what was loaded, weighted, and cited. Makes output diagnosable when something lands wrong. Template: `references/session-trace-template.md`.

Reference files (the "Working Positions" section of `agents/messaging-strategist.md` and the SKILL.md vocabulary sections) are the source of truth for working positions. When a position shifts in a session, edit the reference file in place, log the shift to the decisions log, and note it in the session trace. The end-of-session ritual (ask once whether anything shifted) closes the loop.

## Content Extraction: Mining Existing Content for the Framework

Founders and brand owners rarely start from nothing. They've been articulating their vision in pitch decks, LinkedIn posts, investor updates, sales calls, internal memos, product docs, website drafts, and casual conversations for months or years. The strategy is already there — it's just scattered, inconsistent, and unstructured.

**Content extraction is the most powerful way to build a messaging framework** because:
1. It starts from the founder's authentic voice, not a template
2. It surfaces what the founder actually believes (not what they think they should say)
3. It reveals inconsistencies and gaps the founder didn't know existed
4. It gives the founder something to react to, which is 10x faster than creating from scratch

### How to run content extraction

**Step 1: Gather everything.** Ask the user to provide or point to all available content. Cast a wide net — the best material is often in unexpected places:
- Pitch decks (investor, sales, partnership)
- LinkedIn posts and articles by the founder
- Website copy (current and drafts)
- Internal memos, strategy docs, all-hands notes
- Product descriptions and one-pagers
- Email campaigns, sequences, auto-replies
- Sales call transcripts or notes
- Customer-facing presentations
- Press releases or media coverage
- Notion wikis, Confluence pages, internal docs
- Slack messages where the founder explained the vision (these are gold — unpolished and authentic)
- Brand guides or style docs
- Investor updates or board decks

**Step 2: Read and tag everything.** Go through each piece of content and tag the relevant passages against the 10 framework sections. For each passage, note:
- Which section it maps to (Category, Ecosystem, Pillars, etc.)
- Whether it's a strong signal (clear, specific, differentiated) or a weak signal (generic, vague, could be any company)
- Whether it contradicts something else the founder has said elsewhere
- The source and context (a LinkedIn post hits different than an investor deck — the LinkedIn version is often more authentic)

**Step 3: Build the extraction report.** For each of the 10 framework sections, produce:

**What exists:**
- Direct quotes and passages from the founder's content, attributed to source
- The strongest signals — the moments where the founder was clearest and most differentiated
- Patterns — language, themes, and ideas that recur across multiple pieces

**What's inconsistent:**
- Contradictions between sources (the deck says X, the website says Y)
- Language that shifts depending on audience (sometimes this is intentional and good — note it either way)
- Claims that appear in one place but aren't supported elsewhere

**What's missing:**
- Sections with no content at all — genuine gaps
- Sections with only weak signals — the founder has gestured at it but hasn't articulated it clearly
- Critical questions the content doesn't answer

**Draft framework language:**
- For sections with strong signals: synthesize the best passages into draft framework language that preserves the founder's voice. Don't rewrite them into marketing-speak — keep the founder's authentic phrasing and sharpen it.
- For sections with weak signals: write a draft that captures the direction and flag it as "needs your input — here's what I'm picking up, is this right?"
- For sections with nothing: leave blank with specific questions to answer

**Step 4: Present for reaction.** Give the founder the extraction report and the pre-populated framework. Frame it as: "Here's what I found in your existing content. Some sections are strong — you've already said this well. Some sections have fragments I've assembled into a draft. Some sections are genuinely empty. Let's start with what's wrong and what's missing."

This approach works because founders are excellent editors and terrible blank-page writers. Give them something to push against and they'll sharpen it fast.

### When content extraction reveals a stronger strategy than the founder realized

This happens more often than you'd expect. The founder has been evolving their thinking across dozens of touchpoints over months. No single piece captures the full picture. But when you lay all the pieces side by side, a clearer and more ambitious strategy often emerges — one the founder recognizes instantly but hadn't articulated in one place. When this happens, name it explicitly: "Here's what I think you're actually saying when I connect these pieces. Is this right?" That moment of recognition is when the framework clicks.

## The 10-Section Framework

A complete messaging framework has these sections. The order matters — each section builds on the ones before it. But you don't have to do them all at once. Sections 1-3 are the strategic foundation and should come first. The rest follows.

### Section 1: Category Definition

**What you're creating:** The market category your company owns or is creating. Not your product description — the space your product defines.

**Why this comes first:** Every decision downstream — pillars, positioning, competitive framing — depends on what category you're playing in. If you're creating a new category, you need to name it and make it feel inevitable. If you're claiming an existing one, you need to explain why your approach is fundamentally different.

**What to produce:**
- A category name (2-4 words) that's intuitive and ownable
- Why this category needs to exist now — what's broken, what's changed, what gap exists
- The "before vs. after" picture: what the world looks like without this category vs. with it
- Your company's unique right to define this category

**The questions that unlock this section:**
- When someone who's never heard of you asks "what do you do?" — what do you say? Not the rehearsed version. The real version, the one that makes them lean in.
- If a journalist wrote about your category in 3 years, what would the headline be?
- What are people doing today instead? Not which tools they use — what *approach* are they taking, and why is it fundamentally limited?
- Why is your company the one to define this? What have you built, acquired, or assembled that gives you the right to draw this line in the sand?

**Push back on:**
- Category names that sound invented or jargony — if a customer wouldn't use the word naturally, it's wrong
- "Before/after" contrasts that are really just feature lists in disguise
- Category definitions that are so broad they don't exclude anything (if everyone's in your category, it's not a category)

---

### Section 2: Ecosystem Narrative

**What you're creating:** The story of how your company's products, brands, acquisitions, and capabilities fit together — and why the whole is greater than the sum of the parts.

**Why this matters:** Most companies with multiple products or acquisitions describe themselves as a list: "We have X, Y, and Z." That's not a story — it's an inventory. The ecosystem narrative answers the harder question: *why do all these things exist under one roof, and what does that make possible that wasn't possible before?*

This is especially important after acquisitions. Customers of acquired companies are wondering "what changed and should I be worried?" Partners are wondering "what does this mean for our relationship?" The ecosystem narrative answers both — not with corporate M&A language, but with a strategic story that makes the assembled whole feel intentional and valuable.

**What "ecosystem" means in practice:**
An ecosystem is what you get when multiple capabilities — data infrastructure, intelligence layers, applications, distribution networks, customer relationships — connect to create something none of them could deliver alone. Think of it as the difference between a toolbox (a collection of separate tools) and a workshop (an integrated environment where the tools work together and the output is greater than any single tool could produce).

Your ecosystem might include:
- Products you built from scratch
- Companies you acquired and their capabilities, customers, and technology
- Data assets or infrastructure that connect the pieces
- Relationships or distribution channels that give the ecosystem reach

The narrative isn't about listing these pieces — it's about explaining what they *become* when connected.

**How to discover your ecosystem story:**
Start with the pieces and work toward the thesis:

1. **Map the pieces:** List every product, acquisition, and capability. For each one, write down: what it does, who it serves, and what unique asset it brings (technology, data, customers, expertise, relationships).

2. **Find the connections:** Where do the pieces feed each other? Does one provide data that another turns into intelligence? Does one serve customers that another can upsell? Does one provide infrastructure that others build on? Draw the lines between them.

3. **Identify what's new:** What can you do now — with all the pieces connected — that no single piece could do alone? This is the ecosystem's value proposition. It should be concrete and specific, not abstract.

4. **Articulate the thesis:** Why did you assemble these pieces? What strategic vision connects them? This is the founder's insight — the reason the acquisitions aren't random but deliberate.

5. **Test the narrative:** Tell the story to someone outside the company. If they say "that makes sense" — you have it. If they say "so you're a holding company?" — you don't have it yet.

**Special case — two-dimensional ecosystems (Platform + Network):**

Some ecosystems aren't just a set of connected products — they're *two business models running on one asset*. This is common when a company serves an end customer with software AND serves a second audience with the data, distribution, or network that the first audience generates. Examples outside wealthtech: payments platforms that also sell transaction intelligence to merchants; HR platforms that also sell labor market data to enterprises.

If your ecosystem is two-dimensional, the narrative has to hold both dimensions at once without confusing either audience. The pattern to work through:

- **Dimension 1 — The Platform:** The software your primary customer pays for. This is what the world sees first. It has its own value prop, pricing, and buyer. Describe this as if the second dimension didn't exist. It must stand on its own.
- **Dimension 2 — The Network:** The asset created *because* the platform exists. Aggregated data, distribution reach, demand signal, a buyer pool — something that has independent value to a different audience. Describe what it is, who it serves, what they pay for, and how it's governed.
- **The flywheel between them:** Articulate how each dimension strengthens the other. More platform customers → richer network → more value flows back to platform customers (better benchmarks, better matching, lower prices, new features). Without a real flywheel, you don't have an ecosystem — you have two unrelated products.
- **The governance layer:** A two-dimensional model lives or dies on trust. Be explicit about what's opt-in, what's aggregated vs. identifiable, how value flows back to the audience whose data powers the network, and what you will *never* do. If you can't articulate this clearly, the model collapses under the first hard question from a customer, partner, or journalist.

**Sequencing: how to communicate a multi-audience ecosystem without confusing anyone:**

When you have multiple audiences (primary software customers, data/network customers, platform partners who integrate with you), the temptation is to lead with the full ecosystem — "we serve everyone in the industry." Don't. That produces a holding-company narrative that means nothing to any single audience.

Instead, sequence the story:

1. **Lead with the primary audience.** Public-facing messaging (homepage hero, investor deck opening, first sales conversation) centers the audience whose product experience defines the brand. Everything a new reader sees first should be about *their* world and *their* outcome.
2. **Reveal the network as strategic context.** A layer down — "about" page, second-half of the pitch, deeper content — introduce the network dimension as the reason the platform gets smarter over time. Frame it as benefit-to-primary-audience first, business-model second.
3. **Have dedicated surfaces for secondary audiences.** Network/data customers and ecosystem partners get their own pages, their own sales motion, and their own value prop. Don't force them into the primary narrative, and don't force the primary audience to read through their narrative.
4. **Make sure every audience can find themselves within 5 seconds.** Navigation, segment pages, and sales collateral should make it immediately obvious which audience a piece of content is for. Ambiguity at the top of the funnel is the single biggest cost of a multi-audience ecosystem.

This is the hardest part of a two-dimensional narrative: you must hold the full ecosystem in the founder's head and in the strategy, but present it in layers to the market. The discipline is *knowing what to leave out* of any given surface.

**What to produce:**
- The ecosystem thesis: one paragraph explaining what the assembled whole creates
- How each piece contributes (and what it brought that couldn't be built from scratch)
- What's possible now that wasn't before — specific, concrete capabilities
- The narrative arc: what you started as → what you assembled → what this enables → where you're going
- Transition language for acquired brands: how their existing customers benefit from being part of the ecosystem
- **If two-dimensional:** Platform story, Network story, flywheel mechanics, governance principles, and the sequencing map (what each audience sees first, second, third)
- **Audience-by-audience surface map:** for each distinct audience (primary customers, data/network customers, ecosystem partners like wealthtechs/fintechs who integrate with the platform), what the one-line positioning is, which narrative layer they enter at, and what you're NOT saying to them

**Push back on:**
- Narratives that sound like M&A press releases ("strategic acquisition to expand capabilities")
- Ecosystem stories where the connections between pieces are forced or unclear
- Missing the "so what" — if the ecosystem story doesn't clearly explain why a customer should care, it's not done
- Leading with the network story when the primary-audience platform is what the market actually needs to understand first
- Flywheels that are asserted but not mechanical — if you can't point to the specific way Audience A's activity creates value for Audience B and vice versa, it's marketing copy, not a business model
- Hand-waving on data governance — if the founder can't answer "what's opt-in, what's anonymized, what do customers get in return" in plain language, the network dimension isn't ready to communicate publicly

---

### Section 3: Brand Architecture

**What you're creating:** The rules for how each brand in your ecosystem relates to the parent brand — when to use which name, how they appear together, how they show up on every customer surface, and what gets said to each brand's existing customers during any transition.

**Why this matters:** Without clear brand architecture, every customer touchpoint becomes a judgment call. Sales doesn't know which name to lead with. The website team doesn't know how to position an acquired brand. PR mentions drift. Email signatures fragment. Contracts use one name, marketing uses another, and the conference booth uses a third. This section eliminates the ambiguity by producing a working reference, not a strategy document.

**The architectural words you choose here have strategic weight:**
*Platform, network, ecosystem, layer, fabric, operating system* — these look interchangeable but each carries a different signal. Before you decide how brands relate, pin a meaning to each word you'll use and stick to it. Suggested default:
- **Platform** — the software a customer pays for and runs on. Single-sided: you sell it, they use it.
- **Network** — a multi-sided system where multiple audiences create value for each other. Used when the business model itself is multi-sided.
- **Ecosystem** — the informal, broader collection (products + partners + integrations + community). Looser than network. Useful in conversation, weaker as a formal brand claim.
- **Layer / fabric / operating system** — architectural metaphors for *where you sit in the stack.* Use when your role relative to other software matters to the buyer.

If your company has multiple sides (end customers + data buyers + infrastructure consumers), use different words on different surfaces deliberately. Don't let them drift into synonyms.

**Decision framework — pick a model per brand:**

Before picking a model, answer three questions for each brand in the ecosystem:

- **Equity:** Does the brand have real recognition with its audience? Would losing the name destroy trust built over years, or is it unknown outside a small niche?
- **Audience:** Does this brand serve the same buyer as the parent, or a genuinely different one (e.g., developers vs. enterprise buyers, small firms vs. large)?
- **Timeline:** Is there a strategic reason to absorb fast, or a customer-sensitivity reason to migrate slowly? Contracts, integration cycles, press cycles, investor narrative — each pulls on the timeline.

**The four models (pick one per brand, or mix):**

- **Monolithic — everything becomes the parent brand.** Clean, simple, maximum parent-brand equity. You lose sub-brand equity entirely. Good for acquisitions with weak standalone brand, or when the parent brand is so strong that absorbing is additive. (Google → Google Maps.)
- **Endorsed — sub-brand stays, references parent.** Best when sub-brands have real audience equity you don't want to destroy. The endorser line ("X, part of Y" or "X, a Y company") signals the relationship without erasing the brand. Most common pattern for acquired brands in transition.
- **Product brand — sub-brand becomes a product line under the parent.** The sub-brand survives as a product name, but the parent is primary. Useful when the acquired technology is still distinctive but the company identity is being absorbed.
- **Independent — sub-brand operates on its own; parent is invisible to customers.** Only makes sense when there's a *strategic* reason to keep brands separate (regulatory, competitive, different customer segments that can't know they share a parent). Rare and usually temporary.

**Phased endorsement — the pattern for acquired brands in transition:**

Most acquisitions that start as "Endorsed" eventually move toward "Monolithic" or "Product brand." The question isn't whether to migrate — it's how fast, and through what phases. Treat the transition as a three-phase plan with explicit phase boundaries:

*Phase 1 — Light endorsement.* Sub-brand hero on its own surfaces. Parent appears as a small endorser line beneath the sub-brand logo ("X, part of Y" or "X, a Y company"). Parent visible on navigation, footer, press first-mention, email signatures, and legal documents. Sub-brand's product experience is unchanged. Purpose: communicate the acquisition, preserve customer trust, buy time.

*Phase 2 — Co-equal transition.* Lockup becomes visually balanced ("X by Y" or the two marks at equal weight). Parent brand appears in docs chrome, nav, and any new capability shipped in this phase. Sub-brand retains product-level naming but the parent is no longer secondary. Purpose: migrate equity before removing the sub-brand name.

*Phase 3 — Sunset.* Sub-brand domain redirects, wordmark retired, namespace aliased for backward compatibility. One-time clean communication to customers. Purpose: complete the migration without drama.

**Transition standing rules (lock these when Phase 1 begins):**

- Any *new* capability shipped during the transition ships under the parent brand from day one. This is how equity migrates without a forced rebrand moment.
- First-mention rule: every press/PR/legal artifact mentioning the sub-brand pairs it with the endorser line on first mention ("X, part of Y"), then uses the sub-brand alone.
- Legal entity clarity on all contracts. Parent visible on every agreement the sub-brand's customers sign.
- Conference/events consolidate under the parent brand. Exceptions only for audience-specific events where the sub-brand is the actual draw (e.g., developer conferences for an acquired infrastructure company).
- Swag, print collateral, business cards: run out existing inventory, don't reprint in the old brand.

**When the sub-brand serves a different audience than the parent:**

This is the hardest case. If the parent brand is customer-facing and the sub-brand is developer-facing (or vice versa), the audience experiences the transition differently on different surfaces. Rules:

- Developer-facing surfaces can hold the endorser line longer — developers care about API stability, not brand identity.
- Customer-facing surfaces should move faster — customers build loyalty to brand promises, and holding two brand promises is confusing.
- Consider keeping the sub-brand alive longer on its native-audience surfaces even as the customer-facing audience only ever sees the parent. This is legitimate, not inconsistent, as long as the architecture is written down.

**Multi-brand systems (more than one acquired brand):**

If the company has multiple acquired brands (e.g., one is already absorbed, one is mid-transition, one was just acquired), map each brand to a phase explicitly. Write down: which brand is in which phase, which phase each brand moves to next, and by when. Without this map, different brands drift at different speeds and the company's ecosystem story fragments.

**What to produce:**

- **The model per brand** — monolithic, endorsed, product brand, or independent. If mixed, which brand uses which model and why.
- **Per-brand brief** — for each brand in the ecosystem, a one-page reference: relationship to parent, audience served, visual treatment (logo lockup, colors, mark hierarchy), verbal treatment (endorser line exact text, first-mention rule), current phase, next phase, and phase boundary dates.
- **The decision table** — "When do I say X? When do I say the parent? When do I say both?" A team-facing quick reference. Include examples for sales decks, press releases, email, product UI, conference booths, contracts.
- **Transition comms plan per acquired brand** — what's said to the sub-brand's existing customers at each phase boundary. Specifically: Phase 1 launch announcement, Phase 2 co-equal announcement, Phase 3 sunset announcement. Draft the sunset note before Phase 1 ships so the end state is clear.
- **The surface map** — every place both brands appear (homepage, sub-brand website, docs, press, email signatures, logo lockups, conference booths, contracts, invoices, product UI). For each surface, which brand is primary in the current phase.

**Push back on:**

- Models chosen for brand-team preference rather than customer experience — the test is what's clearest to the customer, not what preserves the most marketing assets
- Transitions without explicit phase boundaries (they drift forever, and the company ends up with three brands permanently because nobody pulled the trigger)
- Acquired brands kept "Independent" without a real strategic reason — usually a tell that the founder hasn't decided yet and is deferring the hard call
- Missing the standing rules — without them, new capabilities ship under old brands and the equity never migrates
- Architecture words used interchangeably (platform = network = ecosystem) — this is where the vocabulary discipline from Section 8 should feed directly into the brand architecture decisions
- Transition comms drafted only at the moment a phase change happens — drafting under time pressure produces inconsistent voice. Draft all three phase announcements at Phase 1 kickoff.

---

### Section 4: Core Messaging Pillars

**What you're creating:** 3-4 big ideas that anchor everything you say. Not features, not benefits — the conceptual themes that every piece of content should reinforce.

**Why this matters:** You can't personally approve every LinkedIn post, email, and sales deck. Pillars are the guardrails. If someone on your team is writing anything customer-facing, they should be able to ask "does this reinforce one of our pillars?" and the answer should be yes.

**What to produce:**
- 3-4 pillars (not more — if you have 6, you have none)
- Each pillar: a headline (2-5 words), a 2-3 sentence explanation, and 2-3 proof points
- Pillars should be mutually exclusive and collectively exhaustive — no overlap, no gaps
- They should work at the ecosystem level, not just one product

**How to develop them:**
- Start with your category definition and ecosystem narrative — pillars should flow naturally from those
- Ask: what are the 3-4 things a customer should walk away believing about us?
- Test each pillar: could a competitor credibly claim this? If yes, it's not specific enough
- Test the set: do these 3-4 things tell the complete story? If you removed one, would the story have a hole?

**Common failure modes:**
- Too many pillars (dilutes focus — forces you to prioritize)
- Pillars that are features ("Real-time dashboards") instead of ideas ("Operational clarity")
- Pillars any competitor could claim ("Customer-focused" — says nothing)
- Pillars that overlap ("Unified data" and "Connected intelligence" are the same idea wearing different clothes)

---

### Section 5: Segment Messaging

**What you're creating:** The tailored version of your story for each market segment. Same company, same ecosystem — but the angle of entry and value emphasis shifts based on who you're talking to.

**Why segments need their own messaging:** Different segments engage with different parts of your ecosystem and care about different outcomes. A one-size-fits-all message either goes so broad it says nothing compelling, or so narrow it alienates segments that don't see themselves in it.

**What to produce for each segment:**
- **Segment positioning statement:** One paragraph on what your company/ecosystem means to this segment specifically
- **Lead narrative:** The "why us" story from their perspective — their problem, why current solutions fail, how your ecosystem solves it
- **Ecosystem entry point:** Which parts of your ecosystem matter most to this segment and why
- **Buyer journey:** How they discover you, what the first conversation sounds like, what moves them through the funnel
- **Key proof points:** Evidence that resonates with this segment specifically

**How to develop segment messaging:**
- Start with how each segment currently solves the problem (or fails to)
- Identify which pieces of your ecosystem address their specific pain
- Talk to your sales team — what language works in real conversations with each segment?
- Map the buying process: who initiates, who influences, who decides, who blocks?

**Important distinction:** Segment messaging is different from persona messaging (Section 6). Segments are market-level (RIAs vs. Asset Managers vs. Wealthtech partners). Personas are role-level (Firm Principal vs. COO). A Principal at an RIA and a Head of Distribution at an AM are both senior buyers, but the segment message is completely different. Persona value props (Section 6) operate *within* each segment.

---

### Section 6: Persona Value Props

**What you're creating:** The specific pitch points for each buyer persona within each segment. This is where messaging gets concrete — what you actually say to the person across the table.

**What to produce for each persona:**
- **Lead message:** One sentence on why they should care
- **Supporting points:** 3 value props, each tied to a real pain point they have
- **Primary pain point:** The #1 thing keeping them up at night that you solve
- **Primary CTA:** The most natural next step for this persona
- **Proof point:** One piece of evidence that makes it real (metric, example, testimonial)

**How to develop persona value props:**
- Base personas on real buyers you've talked to, not marketing archetypes
- For each persona, ask your sales team: what do they care about? What objections do they raise? What closes them?
- Make sure you're talking to the decision-maker, not just the user — the person who writes the check may care about different things than the person who uses the product
- Value props must be outcomes, not features. "Access to 50+ integrations" is a feature. "Stop spending 10 hours a week pulling data from five systems" is an outcome.

---

### Section 7: Competitive Positioning

**What you're creating:** How you're differentiated against specific competitors — told as a narrative, not a feature checklist.

**Why narrative:** Feature comparison matrices invite commoditization — customers scan for checkmarks and whoever has more wins. Narrative positioning reframes the conversation: "they're solving a different problem" or "their approach works until you need X." It moves the conversation from "which tool has more features" to "which approach is right for where you're going."

**What to produce for each competitor:**
- **Their story:** Fair, accurate description of what they do well — never disparaging. Credibility comes from showing you understand the landscape honestly.
- **The frame shift:** How to reframe the comparison in your favor. Not "we have X and they don't" — rather "they built for Y and we built for Z, and here's why Z matters for you."
- **The killer question:** One question your team can ask that exposes the gap between the competitor's approach and what the customer actually needs
- **Segment-specific angles:** The same competitor may be strong in one segment and irrelevant in another

**Critical dependency:** You must define the correct competitor set. Don't assume — ask. And validate with sales: which competitors actually come up in deals? What do prospects say about them? If competitive positioning hasn't been validated with people who sell, it's theory, not positioning.

**Push back on:**
- Positioning that's disparaging (undermines credibility)
- Feature-level comparisons instead of strategic differentiation
- Positioning based on what competitors *used to be* rather than what they are now
- Missing competitors that actually come up in deals

---

### Section 8: Tone, Language & Ecosystem Vocabulary

**What you're creating:** The dictionary. Not a style guide — a working reference the team goes to when they're writing a deck, a blog post, a sales email, or a press quote and they need to know: *which word do I use here, and which word do I avoid?*

**Why this section is different from the others:** Every other section defines *what* you're saying. This section defines *how you say it with precision*. Vocabulary is where strategy leaks or holds. A company with a clear strategy and sloppy vocabulary sounds fuzzy in the market. A company with sharp vocabulary sounds like it knows itself — even when its strategy is still being built.

**The six vocabulary disciplines:**

*1. Brand voice (how you sound, not what you say):*
Two to three sentences that an outside writer could read and internalize without any other context. Examples of the dimensions to name: pace (clipped vs. flowing), stance (peer vs. expert vs. challenger), posture (confident vs. deferential), register (plain-spoken vs. technical). The voice should feel like a specific human, not a committee.

*2. Register map (which words go where):*
If you have more than one audience — or a public/strategic register split (e.g., what you say on the homepage vs. what the founder says on an investor stage) — explicitly map which vocabulary lives in which register. The same concept often has two legitimate words; the discipline is knowing when to use each.

Format each entry as: *concept → public-register word → strategic-register word → why the split exists.*

Example patterns this catches: the public-facing category word (what customers see first) vs. the strategic category word (what the founder uses to describe the business model). Product architecture words (*platform, network, layer, ecosystem, fabric, operating system*) that can look interchangeable but actually describe different things — pin each to a specific meaning and enforce the distinction.

*3. The dictionary (word-by-word, with reasoning):*
Not a list of good words and bad words — a **reasoned** dictionary. Each entry explains *why* the word is on or off the list. This is how the team internalizes voice instead of memorizing rules.

Entries should cover four categories:

- **Use freely** — core vocabulary that reinforces the brand. Say it often.
- **Use deliberately** — strong words that work *only* in the right context. Include the context rule. ("Advisor-owned" works only when the governance model has been explained; don't use it cold.)
- **Avoid** — words that feel generic, overused, or off-voice. Include a replacement.
- **Never use** — words that actively damage the brand (regulatory risk, category-wrong, bad associations). Include the reason.

Each entry gets a one-line rationale. Example format:
*"disruptive" — never use. Every SaaS company says it. The word is a tell that you don't have a specific claim.*
*"leverage" (verb) — avoid. Use "use" or a specific verb. "Leverage" is consulting-speak and signals you're hiding behind abstraction.*
*"advisor-owned" — use deliberately. Only in contexts where governance model has been stated or is visible. Do not use in cold outreach or first-touch materials.*

*4. Sensitive-topic vocabulary:*
Any topic where word choice signals trust vs. extraction, competence vs. bluster, or strategic clarity vs. hype gets its own mini-dictionary. Common sensitive topics:

- **Data rights and governance.** The difference between "we collect" and "you permission," between "our data" and "your data," between "we analyze" and "we turn into intelligence you own" — these aren't synonyms. They signal opposite relationships with the customer. Pin the right words per audience and per surface (homepage vs. legal vs. pitch deck).
- **AI / automation.** The market is saturated. Generic "AI-powered" language dilutes. Specific claims ("our model surfaces at-risk clients 14 days before they churn") hold. Rule: name the thing the AI does, not the fact that there is AI.
- **Pricing and value exchange.** Especially in multi-sided models where one side subsidizes another. The word "free" signals "you're the product." The word "subsidized" signals "someone else is paying." The phrasing "materially lower because asset managers fund the network" signals "here's the economic model, plainly." Choose the level of transparency that matches the audience's sophistication.
- **Competitors.** Language rules for how you describe competitors in every artifact. Typically: respectful, accurate, never disparaging. No smug. No strawmen.

*5. Ecosystem vocabulary (the brand and product naming rules):*
From Section 3 (Brand Architecture). This is the working reference for:

- How to name the parent company in any mention
- How to name each product, brand, or acquired company
- The endorser line (for acquired brands in transition): the exact phrasing used on logos, press first-mentions, email signatures, contracts
- When to lead with the parent brand vs. the sub-brand (depends on audience)
- Transition phasing — which endorser line is active in which quarter
- Legacy names — which products/brands are being renamed, the active name, the alias, and the sunset date

Practical rule: if your team has to ask "what do I call this thing in this context," the dictionary failed. Write the answer down.

*6. Boilerplates:*
Short (1 sentence), medium (1 paragraph), long (3-4 paragraphs) versions of the company description. Used for press releases, partner agreements, bios, website footers. Written once, approved by Legal and brand, locked until a formal update. The first time someone rewrites a boilerplate on the fly is the first time the company has three slightly different descriptions of itself in public.

**Before/after examples (3-5 pairs):**
Show the voice in action. Bad copy → good copy, with a one-line diagnosis of what changed and why. The team learns from examples faster than from rules.

**The banned-phrases master list:**
Load `skills/messaging-framework/references/banned-phrases.md` whenever working on Section 8 or QA-ing content. This is the single source of truth for all banned words, banned expression patterns, and style rules. It supersedes any inline list in this skill or elsewhere in the plugin. Enforce every item. The list covers hard-ban words (with replacements), hard-ban rhetorical patterns (with approved rewrites), and style rules.

**Push back on:**
- Dictionaries that are just lists without reasoning — people won't internalize the voice, they'll just look things up and move on
- Missing the sensitive-topic mini-dictionaries — this is where most brands leak credibility
- Vocabulary rules that contradict the positioning (e.g., voice says "peer" but the word list is full of vendor-speak)
- No register map when the company has a public/strategic split — leads to the founder sounding one way on stage and the homepage sounding another, with nothing tying them together
- Boilerplates written from marketing's perspective instead of how a buyer would actually describe you
- Cheap words that keep showing up because nobody named them cheap

---

### Section 9: Elevator Pitches

**What you're creating:** The spoken-word versions of your story — what you actually say in meetings, at conferences, on calls.

**What to produce:**
- **Company pitch (30 seconds):** The ecosystem/category story in conversational language
- **Company pitch (60 seconds):** Expanded with a proof point or example
- **Segment pitches (30 seconds each):** How you open a conversation with each segment
- **The cocktail-party answer:** 1-2 sentences for "so what do you do?"

**The most important rule:** These are written for the ear, not the eye. Read them out loud. If they sound like a brochure, rewrite them. Nobody says "purpose-built intelligence platform" in conversation. They say something real.

---

### Section 10: Objection Handling

**What you're creating:** The most common buyer objections and how to respond. Where strategy meets the real world.

**What to produce:**
- 6-10 objections ranked by how often they come up
- For each: the objection in the buyer's words, the approved response, and the underlying concern the objection reveals
- Responses that acknowledge first (never dismissive), then reframe
- Segment-specific objections where relevant

**Where the content comes from:** Sales team provides the objections (they hear them every day). You provide the responses. Sales validates that the responses actually work. Iterate.

---

## Dependency Map

```
Section 1 (Category) ──┐
Section 2 (Ecosystem) ─┼──→ Section 4 (Pillars) ──→ Section 5 (Segment) ──→ Section 6 (Persona)
Section 3 (Architecture)┘──→ Section 8 (Tone/Vocab)

Section 5 (Segment) ──→ Section 7 (Competitive)
Section 4 (Pillars) + Section 5 (Segment) ──→ Section 9 (Pitches)
Section 6 (Persona) + Section 7 (Competitive) ──→ Section 10 (Objections)
```

Sections 1-3 can be worked in parallel — they're the strategic foundation. Sections 4-6 are sequential. Sections 7-10 can run in parallel once 4-6 are done.

## Working With the User

When guiding someone through this framework:

1. **Start with what exists.** Before anything else, ask: "What content do you already have? Decks, docs, LinkedIn posts, website copy, internal memos — anything where you've talked about the company's story, positioning, or vision." If content exists, run the content extraction process first. This gives you raw material to work with and gives the founder something to react to rather than a blank page.

2. **Mine the content for the strategy that's already there.** Read everything. Tag it against the 10 sections. Pull out the strongest passages in the founder's own words. Identify patterns, contradictions, and gaps. Present back a pre-populated framework with clear attribution — "You said this in your investor deck. You said this on LinkedIn. Here's what I think you're actually saying when I connect these pieces."

3. **Work the strategic foundation first (Sections 1-3).** These are the decisions everything else hangs from. Don't let the user skip ahead to elevator pitches before the category and ecosystem are defined. Content extraction often reveals that the founder has the clearest instincts about Category and Ecosystem — they just haven't formalized them.

4. **Be a sparring partner, not a scribe.** Ask hard questions. Push past the first answer. If something sounds generic, say so. If a pillar could belong to any competitor, challenge it. The goal is to find what's authentically true and differentiated — not to produce safe, inoffensive language.

5. **Use the founder's own words as the starting point.** Don't rewrite their language into marketing-speak. Find the moments where they were clearest and most compelling — often in unpolished contexts like Slack messages, call transcripts, or LinkedIn posts — and use those as the foundation. Sharpen, don't replace.

6. **Flag dependencies honestly.** If a section can't be completed without input from other people (sales team, legal, acquired company stakeholders), say so. Don't let the user think they can finish the framework alone if they can't.

7. **Keep it conversational and direct.** This is a strategic working session, not a consulting deliverable. Write like a smart colleague thinks — clear, opinionated, and practical.

8. **Respect the founder's voice.** The best frameworks sound like the founder on their best day — structured, sharp, and authentic. Your job is to help them get there, not to sound like a branding agency.

## Output Format

When building a framework, produce a structured document with all relevant sections. Flag anything incomplete or needing validation. Keep language direct and operational.

When auditing, produce a gap analysis by section with findings, severity, and fixes.

When QA-ing content, check each piece against the framework and flag inconsistencies with the specific section and language violated.
