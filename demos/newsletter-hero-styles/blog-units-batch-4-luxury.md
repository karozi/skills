# Newsletter Hero Styles — Batch 4: Luxury Editorial (6 styles)

The "expensive and luxurious" editorial set. For each style: live preview link, short
description, an AI prompt readers can paste into any builder, and a condensed code
block. Full builds live in the `hero-*.html` files beside this document. All heroes
carry the identical canonical copy (verified hash `bdfc6df817`).

---

## 50 · Swiss Modernism 2.0
**Live preview:** https://claude.ai/code/artifact/dd6a9757-8bf8-4e4a-88a0-c820e60cf2aa

Swiss Modernism 2.0 takes the 1950s International Style — the strict 12-column grid, Helvetica, mathematical spacing — and refines it into something a Basel museum would print in its exhibition catalog: warm gallery off-whites instead of stark paper white, featherweight 300-weight type at enormous sizes beside tiny letterspaced captions, and a single deep ultramarine doing all the emotional work. It feels expensive precisely because nothing shouts; the visible hairline grid, numbered "Fig. 01" captions, and underlined form field signal a design that was measured, not decorated. Perfect for newsletter writers covering architecture, design criticism, strategy, or finance.

**Prompt**
```text
Build a newsletter hero in refined Swiss Modernism ("museum catalog" grade).
Background warm gallery off-white #F3F1EC, ink #1C1B18, secondary grey #6E6A61,
hairlines #DAD6CC, ONE accent: deep ultramarine #2036A8 (no red, no gradients).
Font: Helvetica Neue/Inter system stack. 12-column CSS grid, 24px gap, faint
visible column hairlines behind content. Header: small wordmark left with a tiny
ultramarine square after it; uppercase letterspaced kicker right; hairline rule.
Headline ~80px, weight 300, letter-spacing -0.025em, spanning columns 1-8; one
accent word in ultramarine. Form: borderless input with a 1px bottom hairline
(thickens ultramarine on focus), square uppercase letterspaced ultramarine
button; microcopy captioned "Fig. 01 —". Stats as a right-rail hairline-divided
stack with tiny ultramarine indexes (01-04) via CSS counters.
```

**Code**
```html
<style>
  .sw2{background:#F3F1EC;color:#1C1B18;font-family:"Helvetica Neue",Helvetica,Inter,Arial,sans-serif;
    display:grid;grid-template-columns:repeat(12,1fr);gap:24px;padding:56px 32px;}
  .sw2 .wm{grid-column:1/5;font-size:19px;}
  .sw2 .wm::after{content:"";display:inline-block;width:8px;height:8px;background:#2036A8;margin-left:8px;}
  .sw2 .kick{grid-column:8/13;justify-self:end;font-size:11px;letter-spacing:.16em;text-transform:uppercase;color:#6E6A61;}
  .sw2 hr{grid-column:1/13;border:0;border-top:1px solid #DAD6CC;width:100%;margin:0 0 32px;}
  .sw2 h1{grid-column:1/9;margin:0;font-size:clamp(40px,6.6vw,80px);font-weight:300;line-height:1.02;letter-spacing:-.025em;}
  .sw2 h1 span{color:#2036A8;}
  .sw2 .sub{grid-column:1/7;font-size:16px;line-height:1.65;color:#46433C;max-width:52ch;}
  .sw2 .signup{grid-column:1/7;display:flex;gap:16px;flex-wrap:wrap;}
  .sw2 input{flex:1 1 220px;font:inherit;background:none;border:0;border-bottom:1px solid #8B8779;padding:12px 2px;color:#1C1B18;}
  .sw2 input:focus{outline:none;border-bottom:2px solid #2036A8;}
  .sw2 button{font:inherit;font-size:12px;letter-spacing:.18em;text-transform:uppercase;
    background:#2036A8;color:#F3F1EC;border:0;padding:14px 40px;cursor:pointer;}
  .sw2 button:focus-visible{outline:2px solid #1C1B18;outline-offset:3px;}
  .sw2 .micro{grid-column:1/7;font-size:11px;letter-spacing:.12em;text-transform:uppercase;color:#6E6A61;}
  .sw2 .micro::before{content:"Fig. 01 \2014  ";color:#2036A8;}
</style>
<section class="sw2">
  <div class="wm">Dispatch</div><div class="kick">The Weekly Dispatch · Issue N°142</div><hr>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p class="sub">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form class="signup" onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button>Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p>
</section>
```

---

## 78 · Bold Typography (Poster)
**Live preview:** https://claude.ai/code/artifact/4a8cec5f-d359-48ed-ad2a-d836e1f575d4

This is the newsletter hero as a limited-edition exhibition broadsheet: a stacked, near-condensed 900-weight headline printed edge-to-edge in rich ink-black on warm paper, with vermillion used the way a letterpress shop uses a second ink — once for "inbox.", once for the subscribe plate, and nowhere else. It feels expensive because everything is typographic furniture rather than decoration: thick-and-thin rule pairs, a monospace folio strip of stats, an outlined middle headline row, and zero border-radius anywhere. Perfect for essayists, culture critics, and design-world writers whose newsletter is closer to a printed periodical than a product.

**Prompt**
```text
Build a newsletter hero styled as an ink-dense editorial broadsheet poster.
Warm paper #F3EDE2, ink #100E0B, single accent vermillion #E3350D; zero
border-radius everywhere. Masthead: thick 7px rule + thin 1.5px companion
rule, centered 900-weight condensed caps wordmark ("Arial Narrow" stack) with
.32em letter-spacing. Kicker as a black bar with monospace uppercase text.
Headline stacked in three uppercase lines at clamp(3.4rem,13.5vw,10.2rem),
line-height .86; middle line as outline type via transparent color + 2.5px
-webkit-text-stroke; last word vermillion. Subhead with a thick vermillion
left border, next to an inverted ink-black panel (vermillion top border)
holding a square email input + vermillion SUBSCRIBE button. Bottom: full-bleed
stats strip under a thick/thin rule pair — condensed 900 numbers over
letterspaced monospace labels. Vertical monospace edition line down the right edge.
```

**Code**
```html
<style>
  .poster{background:#F3EDE2;color:#100E0B;font-family:"Arial Narrow","Helvetica Neue Condensed","Helvetica Neue",Arial,sans-serif;font-stretch:condensed;padding:2.5rem clamp(1rem,5vw,3rem)}
  .poster *{margin:0;box-sizing:border-box;border-radius:0}
  .rule{border-top:7px solid #100E0B;box-shadow:0 5px 0 -3.5px #100E0B;margin-bottom:1rem}
  .kick{display:inline-block;background:#100E0B;color:#F3EDE2;font:700 .68rem/1 ui-monospace,monospace;letter-spacing:.3em;text-transform:uppercase;padding:.5rem .85rem}
  .poster h1{font-size:clamp(3.2rem,13vw,9.5rem);font-weight:900;text-transform:uppercase;line-height:.86;letter-spacing:-.022em;margin:1.2rem 0 1.6rem}
  .poster h1 .ln{display:block}
  .poster h1 .ln2{color:transparent;-webkit-text-stroke:2.5px #100E0B}
  .poster h1 .acc{color:#E3350D}
  .poster .sub{font-weight:600;font-size:1.15rem;line-height:1.55;max-width:34ch;border-left:.55rem solid #E3350D;padding-left:1rem}
  .panel{background:#100E0B;color:#F3EDE2;border-top:.5rem solid #E3350D;padding:1.5rem;margin-top:1.5rem;max-width:34rem}
  .signup{display:flex}
  .signup input{flex:1;min-width:0;border:2px solid #F3EDE2;background:#F3EDE2;color:#100E0B;font:1rem ui-monospace,monospace;padding:.85rem 1rem}
  .signup button{background:#E3350D;border:2px solid #E3350D;color:#FFF7EE;font:900 1rem "Arial Narrow",sans-serif;letter-spacing:.14em;text-transform:uppercase;padding:.85rem 1.5rem;cursor:pointer}
  .signup :focus-visible{outline:3px solid #F3EDE2;outline-offset:3px}
  .micro{font:.68rem ui-monospace,monospace;letter-spacing:.18em;text-transform:uppercase;color:#CFC6B6;margin-top:.9rem}
</style>
<section class="poster">
  <div class="rule"></div>
  <p class="kick">The Weekly Dispatch · Issue N°142</p>
  <h1><span class="ln">The ideas</span><span class="ln ln2">worth your</span><span class="ln acc">inbox.</span></h1>
  <p class="sub">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <div class="panel">
    <form class="signup" onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button type="submit">Subscribe</button></form>
    <p class="micro">Free forever. Unsubscribe anytime.</p>
  </div>
</section>
```

---

## 71 · Modern Dark (Cinema)
**Live preview:** https://claude.ai/code/artifact/698c2822-59c1-43bc-bee6-fe5aec8857b3

Modern Dark (Cinema) is the hush after the lights go down: a deep charcoal-black stage washed in slow-drifting indigo ambient light, framed by true letterbox bars and a soft vignette. It feels expensive because it whispers — featherweight 200-weight type, wide-tracked small-caps credits, one italic serif accent glowing like a projector beam, and a low-opacity glass signup panel instead of loud color. It suits newsletter writers with prestige-drama energy: film and culture critics, longform essayists, and anyone whose Friday email should land like a festival premiere, not a push notification.

**Prompt**
```text
Build a dark cinematic newsletter hero, like a prestige streaming title card.
Background: vertical gradient #0A0A0F to #020203 (never pure #000), with two
huge blurred radial "ambient light" blobs in rgba(94,106,210,.2) and violet,
drifting very slowly (35-45s). Letterbox bars top and bottom (#010102) and a
radial vignette. Type: wordmark and kicker in 11-13px uppercase with
0.3-0.55em letter-spacing (kicker in muted indigo #9BA4E0); headline
clamp(38-64px) at weight 200 in #F2F2F5, one word in italic Georgia colored
#AEB6F2 with a soft indigo glow. Signup: frosted glass panel
(rgba(255,255,255,.05), 1px hairline border, blur(20px), radius 16px) holding
a near-black input and a #5E6AD2 button with tracked uppercase label and
indigo glow. Stats as a 4-column "end credits" strip with rgba-white
hairlines. One accent only, no neon, reduced-motion disables the drift.
```

**Code**
```html
<style>
.cin{position:relative;overflow:hidden;text-align:center;padding:88px 24px;color:#EDEDEF;
  background:linear-gradient(180deg,#0a0a0f,#050506 45%,#020203);
  font-family:"Helvetica Neue","Segoe UI",Arial,sans-serif}
.cin::before,.cin::after{content:"";position:absolute;left:0;right:0;height:24px;background:#010102}
.cin::before{top:0}.cin::after{bottom:0}
.cin .glow{position:absolute;top:-20%;left:15%;width:60%;padding-top:60%;border-radius:50%;filter:blur(70px);
  background:radial-gradient(circle,rgba(94,106,210,.2),transparent 70%)}
.cin>*{position:relative}
.cin .kick{font-size:11px;letter-spacing:.34em;text-transform:uppercase;color:#9BA4E0}
.cin h1{margin:18px auto;font-size:clamp(38px,6vw,60px);font-weight:200;color:#F2F2F5}
.cin h1 span{font-family:Georgia,serif;font-style:italic;color:#AEB6F2;
  text-shadow:0 0 34px rgba(94,106,210,.35)}
.cin .sub{max-width:52ch;margin:0 auto;font-weight:300;line-height:1.75;color:#A6AAB4}
.cin form{display:flex;gap:10px;max-width:440px;margin:34px auto 0;padding:10px;border-radius:16px;
  background:rgba(255,255,255,.05);border:1px solid rgba(255,255,255,.08);backdrop-filter:blur(20px)}
.cin input{flex:1;min-width:0;padding:13px 16px;border-radius:10px;color:#EDEDEF;
  background:rgba(2,2,3,.55);border:1px solid rgba(255,255,255,.08)}
.cin input:focus{outline:none;border-color:#5E6AD2;box-shadow:0 0 0 3px rgba(94,106,210,.25)}
.cin button{padding:13px 26px;border-radius:10px;border:1px solid rgba(255,255,255,.14);cursor:pointer;
  background:#5E6AD2;color:#fff;font-size:13px;letter-spacing:.18em;text-transform:uppercase;
  box-shadow:0 0 28px rgba(94,106,210,.35)}
.cin .micro{margin-top:16px;font-size:11.5px;letter-spacing:.14em;text-transform:uppercase;color:#8A8F98}
</style>
<section class="cin"><i class="glow"></i>
  <p class="kick">The Weekly Dispatch · Issue N°142</p>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p class="sub">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button>Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p>
</section>
```

---

## 49 · Parallax Storytelling
**Live preview:** https://claude.ai/code/artifact/bfa5b7e2-c225-4b19-89d6-58cf042cce25

Parallax Storytelling builds its drama from depth: a midnight-forest wash, ghosted mid-plane ornaments (a giant italic "N°142", a gold hairline ring, a heritage ampersand), and a gilt-cornered content card all drift on independent clocks, so the hero breathes like the opening spread of a premium annual report. The luxury comes from restraint — serif display type, champagne ink on deep green, and nothing thicker than a one-pixel gold line. It suits newsletter writers with gravitas: long-form essayists, finance and strategy dispatches, heritage brands telling their own story.

**Prompt**
```text
Build a newsletter hero in "parallax storytelling" style — heritage
annual-report luxury. Background #0B1613 deep forest-navy with radial glows of
#14362C and faint gold (#C8A45C at 13%). Three depth planes, each with its own
slow float animation: background wash drifting over 26s, mid layer over 14-21s
(outlined giant italic "N°142" text-stroke ornament, a 1px gold hairline ring,
a ghost ampersand, a gold gradient rule), foreground card floating gently over
11s. Foreground: centered card, 1px #C8A45C border plus offset outline, gilded
corner ticks via pseudo-elements. Georgia serif; small-caps gold wordmark
letter-spaced .5em; huge serif headline in ivory #F2EBD9 with the accent word
italic gold #DDBB74; email input + gold gradient Subscribe button in one
bordered row. Freeze all animation under prefers-reduced-motion.
```

**Code**
```html
<style>
.px-hero{position:relative;overflow:hidden;font-family:Georgia,serif;color:#F2EBD9;text-align:center;
  padding:72px 24px;background:radial-gradient(58% 72% at 78% 18%,rgba(200,164,92,.13),transparent 62%),
  linear-gradient(158deg,#0E1F1A,#0B1613 46%,#08100D)}
.px-hero .orn{position:absolute;top:0;right:-2%;font-size:220px;font-style:italic;line-height:1;
  color:transparent;-webkit-text-stroke:1px rgba(200,164,92,.16);animation:midf 18s ease-in-out infinite alternate}
.px-hero .orn::before{content:"N°142"}
.px-hero .card{position:relative;max-width:640px;margin:0 auto;padding:56px 48px;
  background:rgba(9,18,15,.94);border:1px solid rgba(200,164,92,.38);outline:1px solid rgba(200,164,92,.1);
  outline-offset:6px;box-shadow:0 40px 90px -30px rgba(0,0,0,.75);animation:fgf 11s ease-in-out infinite alternate}
.px-hero .wm{font-size:14px;letter-spacing:.5em;text-transform:uppercase;color:#C8A45C;font-weight:700}
.px-hero h1{margin:20px 0 0;font-size:54px;font-weight:400;line-height:1.06}
.px-hero h1 span{font-style:italic;color:#DDBB74}
.px-hero p{margin:20px auto 0;max-width:50ch;font-size:17px;line-height:1.65;color:#CFDAD1}
.px-hero form{display:flex;max-width:440px;margin:28px auto 0;border:1px solid rgba(200,164,92,.45)}
.px-hero input{flex:1;min-width:0;padding:14px 18px;border:0;background:transparent;color:#F2EBD9;font:inherit}
.px-hero button{padding:14px 26px;border:0;cursor:pointer;background:linear-gradient(180deg,#D5B26A,#C09A4E);
  color:#12100A;font:700 13px Georgia,serif;letter-spacing:.22em;text-transform:uppercase}
.px-hero .micro{font-size:12.5px;font-style:italic;color:#A9BCAF}
@keyframes midf{from{transform:translateY(-18px)}to{transform:translateY(22px)}}
@keyframes fgf{from{transform:translateY(-4px)}to{transform:translateY(5px)}}
@media(prefers-reduced-motion:reduce){.px-hero .orn,.px-hero .card{animation:none}}
</style>
<section class="px-hero"><span class="orn" aria-hidden="true"></span>
 <div class="card"><div class="wm">Dispatch</div>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button>Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p></div></section>
```

---

## 62 · Interactive Cursor Design
**Live preview:** https://claude.ai/code/artifact/74111afb-cff3-4b7a-997c-d6ee32f77685

Interactive Cursor Design turns the pointer itself into the brand: the default cursor disappears and is replaced by an ink dot with a lagging hairline ring that grows gold over the Subscribe button (which magnetically drifts toward you), tints champagne over the accent word, and inverts to ivory over the dark stats band. It feels expensive precisely because the canvas stays restrained — warm ivory, light Didot serif, hairline rules — and all the money goes into micro-interaction, the signature move of award-winning luxury agency sites. It suits newsletter writers selling taste — design, brand strategy, fashion, high-end business commentary. One caveat: the whole trick only exists on desktop; on touch devices it degrades to a still-handsome static editorial hero.

**Prompt**
```text
Build a luxury editorial newsletter hero where the cursor is the design.
Ground: warm ivory #F7F3EB, ink #141210, accents champagne #C6A75E and bronze
#8A6D2F. Type: light Didot/Bodoni serif headline (clamp 44-92px), italic
bronze accent word, mono uppercase kicker, hairline 1px rules, generous
centered whitespace. Cursor: set cursor:none via a JS-added class only (no-JS
keeps the default); render two fixed aria-hidden divs — a 6px ink dot
(instant) and a 36px hairline ring following via requestAnimationFrame lerp
(pos += (mouse - pos) * 0.16). Hover states via data-cursor attributes: ring
grows to 64px gold over the button, bronze tint over the accent word, ivory
border over the dark stats band. Magnetic button: within 110px, translate the
button by 18% of the offset. Degrade under (pointer:coarse); reduced-motion
makes the follow instant; keep :focus-visible outlines.
```

**Code**
```html
<style>
.hero{background:#F7F3EB;color:#141210;font-family:Georgia,serif;text-align:center;padding:80px 24px 0}
.hero h1{font:300 clamp(40px,7vw,84px)/1.05 "Didot","Bodoni MT",Georgia,serif;max-width:14ch;margin:0 auto}
.hero h1 span{color:#8A6D2F;font-style:italic}
.hero .sub{max-width:52ch;margin:24px auto;line-height:1.65;color:#4A443B}
.signup{display:flex;max-width:440px;margin:0 auto;border:1px solid rgba(20,18,16,.35)}
.signup input{flex:1;border:0;background:none;padding:15px;font:italic 15px Georgia,serif}
.signup button{border:0;background:#141210;color:#F7F3EB;padding:15px 28px;letter-spacing:.2em;text-transform:uppercase;font:500 12px monospace;transition:transform .18s}
.micro{font-size:12.5px;color:#6E6558;margin:14px 0 60px}
.dot,.ring{position:fixed;top:0;left:0;border-radius:50%;pointer-events:none;display:none;z-index:99}
.dot{width:6px;height:6px;margin:-3px;background:#141210}
.ring{width:36px;height:36px;margin:-18px;border:1px solid rgba(20,18,16,.6);transition:width .25s,height .25s,margin .25s,border-color .25s}
.ring.big{width:64px;height:64px;margin:-32px;border-color:#C6A75E;background:rgba(198,167,94,.12)}
.cur .hero,.cur .hero *{cursor:none}.cur .dot,.cur .ring{display:block}
@media(pointer:coarse){.dot,.ring{display:none!important}}
</style>
<section class="hero"><h1>The ideas worth your <span>inbox.</span></h1>
<p class="sub">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
<form class="signup" onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button>Subscribe</button></form>
<p class="micro">Free forever. Unsubscribe anytime.</p>
<div class="dot" aria-hidden="true"></div><div class="ring" aria-hidden="true"></div></section>
<script>
(function(){if(!matchMedia("(pointer:fine)").matches)return;
var d=document.querySelector(".dot"),r=document.querySelector(".ring"),b=document.querySelector(".signup button"),
e=matchMedia("(prefers-reduced-motion: reduce)").matches?1:.16,mx=0,my=0,x=0,y=0;
document.documentElement.classList.add("cur");
addEventListener("mousemove",function(ev){mx=ev.clientX;my=ev.clientY;
var c=b.getBoundingClientRect(),dx=mx-c.left-c.width/2,dy=my-c.top-c.height/2,near=Math.hypot(dx,dy)<110;
r.classList.toggle("big",near);b.style.transform=near?"translate("+dx*.18+"px,"+dy*.18+"px)":""});
(function f(){x+=(mx-x)*e;y+=(my-y)*e;d.style.transform="translate("+mx+"px,"+my+"px)";
r.style.transform="translate("+x+"px,"+y+"px)";requestAnimationFrame(f)})()})();
</script>
```

---

## 26 · Trust & Authority (Private Bank)
**Live preview:** https://claude.ai/code/artifact/903aaf2d-2673-442c-b498-2719475e0020

Trust & Authority is usually rendered as corporate SaaS — badge grids, green checkmarks, SOC2 logos. This version translates the same credentials-and-metrics playbook into private-bank language: deep navy, ivory serif, a hairline-engraved crest monogram, and the four stats set into a gold-ruled plaque row like brass credentials on a mahogany door. It feels expensive because nothing shouts — the authority comes from symmetry, hairline gold rules, and unhurried spacing, which makes it perfect for finance, strategy, and premium analysis newsletters whose whole pitch is "we know what we're talking about."

**Prompt**
```text
Build a newsletter hero in private-bank luxury style. Deep navy ground
(#0A1F33, subtle gradient to #081A2C) with ivory text (#F2EDE3) and
champagne-gold accents (#C6A55C) — gold only for accents and rules, never body
text. Centered, strictly symmetrical. Wordmark in wide-tracked uppercase
Georgia (letter-spacing .34em) beneath a pure-CSS crest: a circle with a
double hairline gold ring and an engraved serif initial via ::after. Hairline
gold rules (1px gradient fading at both ends, tiny rotated gold diamond at
center) separate sections. Kicker in 11px small-caps sans, gold. Headline in
large Georgia (~64px, weight 400) with the last word italic gold. Signup as a
single gold-keyline bar: transparent input + solid gold button with navy
uppercase letterspaced label; 2px gold focus outlines. Stats as an engraved
plaque row: 1px gold top/bottom borders, four columns divided by hairline gold
rules, serif ivory numbers with a faint engraved text-shadow over small-caps
gold labels. No shadows, no badges, no rounded corners — trust through restraint.
```

**Code**
```html
<style>
.pb-hero{background:linear-gradient(180deg,#0B2138,#081A2C);color:#F2EDE3;font-family:Georgia,serif;text-align:center;padding:80px 24px}
.pb-hero .crest{width:72px;height:72px;margin:0 auto 14px;border-radius:50%;border:1px solid #C6A55C;position:relative;display:flex;align-items:center;justify-content:center}
.pb-hero .crest::before{content:"";position:absolute;inset:4px;border-radius:50%;border:1px solid rgba(198,165,92,.45)}
.pb-hero .crest::after{content:"D";font-size:28px;color:#C6A55C}
.pb-hero .wm{letter-spacing:.34em;text-transform:uppercase;font-size:22px;text-indent:.34em}
.pb-hero .rule{width:280px;height:1px;margin:24px auto;background:linear-gradient(90deg,transparent,#C6A55C,transparent)}
.pb-hero h1{font-size:clamp(36px,6vw,60px);font-weight:400;line-height:1.12;max-width:15ch;margin:0 auto}
.pb-hero h1 span{color:#C6A55C;font-style:italic}
.pb-hero p{max-width:56ch;margin:18px auto 0;line-height:1.75;color:#D9DDD2}
.pb-hero form{display:flex;max-width:500px;margin:32px auto 0;border:1px solid rgba(198,165,92,.7)}
.pb-hero input{flex:1;min-width:0;background:transparent;border:0;padding:15px 16px;color:#F2EDE3;font:16px Georgia,serif}
.pb-hero button{background:#C6A55C;color:#0A1F33;border:0;padding:15px 24px;font:600 12px/1 Helvetica,Arial,sans-serif;letter-spacing:.22em;text-transform:uppercase;cursor:pointer}
.pb-hero input:focus-visible,.pb-hero button:focus-visible{outline:2px solid #C6A55C;outline-offset:2px}
.pb-hero .micro{font:11px Helvetica,Arial,sans-serif;letter-spacing:.2em;text-transform:uppercase;color:#A9B6C4;margin-top:12px}
</style>
<section class="pb-hero">
  <div class="crest" aria-hidden="true"></div>
  <div class="wm">Dispatch</div>
  <div class="rule" aria-hidden="true"></div>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button type="submit">Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p>
</section>
```
