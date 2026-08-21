# Newsletter Hero Styles — Blog Units, Batch 3 (styles 23–32 of the curated set)

For each style: live preview link, short description, an AI prompt readers can paste
into any builder, and a condensed self-contained code block. Full builds live in the
`hero-*.html` files beside this document. All heroes carry the identical canonical
copy (verified hash `bdfc6df817`).

---

## 09 · Claymorphism
**Live preview:** https://claude.ai/code/artifact/6135c9dc-eeff-42cf-a865-204d9eadf14e

Claymorphism is the toy-box cousin of Neumorphism — instead of ghostly monochrome embossing, everything here is puffy, chunky 3D clay: saturated pastels (peach, baby blue, mint, lilac), thick white borders, 24px+ radii, and the signature double shadow (inset white top-light plus a colored outer drop) that makes buttons look squeezably soft. It suits newsletter writers with a playful, personal voice — education, creativity, indie products; skip it for finance, legal, or medical. Caveat: pastels flirt with low contrast, so keep body text at 4.5:1 or better.

**Prompt**
```text
Build a newsletter hero in Claymorphism style. Light pastel gradient background
(peach #FFF3EC to lilac #F3F0FF to mint #EAF7F0), rounded 36px container with a
thick 4px white border. Palette: Soft Peach #FDBCB4, Baby Blue #ADD8E6, Mint
#98FF98, Lilac #E6E6FA, dark plum text #4A3B52. Every element is puffy clay:
border-radius 20-26px, 3px borders, and a double shadow — inset 0 3px 0 white
top highlight, inset colored underside, plus a colored outer drop shadow.
Headline is heavy 900-weight rounded sans; the accent word sits in a slightly
rotated lilac clay pill. Email input is a white clay capsule with a baby-blue
border; Subscribe button is a peach gradient pill that lifts on hover with a
soft bounce (cubic-bezier 0.34,1.56,0.64,1). Floating blay blob shapes behind
the hero; white clay stat cards each bordered in a different pastel.
Respect prefers-reduced-motion; keep text contrast at 4.5:1.
```

**Code**
```html
<style>
.clay{font-family:"Nunito","Trebuchet MS",system-ui,sans-serif;color:#4A3B52;text-align:center;
  padding:56px 32px;background:linear-gradient(160deg,#FFF3EC,#F3F0FF 48%,#EAF7F0);
  border:4px solid #fff;border-radius:36px;
  box-shadow:inset 0 4px 0 rgba(255,255,255,.95),inset 0 -10px 24px rgba(173,216,230,.35),0 18px 40px rgba(154,129,187,.28)}
.clay .wm{display:inline-block;font-weight:900;font-size:20px;padding:10px 22px;background:#fff;
  border:3px solid #FDBCB4;border-radius:999px;
  box-shadow:inset 0 3px 0 #fff,inset 0 -4px 8px rgba(253,188,180,.4),0 8px 16px rgba(224,122,108,.28)}
.clay h1{font-size:clamp(34px,6vw,58px);font-weight:900;margin:24px auto 0;max-width:14ch;line-height:1.1}
.clay h1 span{display:inline-block;padding:.05em .3em .1em;color:#7C4A94;background:#E6E6FA;
  border:3px solid #fff;border-radius:22px;transform:rotate(-1.5deg);
  box-shadow:inset 0 3px 3px rgba(255,255,255,.9),inset 0 -5px 10px rgba(150,130,200,.3),0 8px 16px rgba(150,130,200,.3)}
.clay p{margin:18px auto 0;max-width:56ch;font-weight:600;color:#6B5B75;line-height:1.6}
.clay form{display:flex;flex-wrap:wrap;justify-content:center;gap:14px;margin:28px auto 0;max-width:520px}
.clay input{flex:1 1 240px;padding:16px 22px;font:inherit;font-weight:700;background:#fff;
  border:3px solid #ADD8E6;border-radius:24px;
  box-shadow:inset 0 3px 0 #fff,inset 0 -4px 10px rgba(173,216,230,.45),0 8px 16px rgba(94,156,190,.22)}
.clay button{padding:16px 34px;font:inherit;font-weight:900;color:#6B2E4E;cursor:pointer;
  background:linear-gradient(150deg,#FFD3CB,#FDBCB4 55%,#F9A79B);border:3px solid #fff;border-radius:24px;
  box-shadow:inset 0 4px 4px rgba(255,255,255,.85),inset 0 -6px 12px rgba(224,122,108,.4),0 10px 20px rgba(224,122,108,.4);
  transition:transform .2s cubic-bezier(.34,1.56,.64,1)}
.clay button:hover{transform:translateY(-3px)}
.clay small{display:block;margin-top:14px;font-weight:700;color:#6B5B75}
</style>
<section class="clay"><div class="wm">Dispatch</div>
<h1>The ideas worth your <span>inbox.</span></h1>
<p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
<form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button>Subscribe</button></form>
<small>Free forever. Unsubscribe anytime.</small></section>
```

---

## 12 · Flat Design
**Live preview:** https://claude.ai/code/artifact/05539b1b-2c4b-40a4-8c5a-593ae120e4eb

Flat Design is the cheerful 2013 reset button: every gradient, bevel, and drop shadow gets deleted, and bold saturated color blocks — turquoise, blue, orange, red on midnight navy — do all the visual heavy lifting with simple geometric shapes and chunky sans-serif type. It suits newsletter writers who want to feel fast, friendly, and product-minded: SaaS commentators, startup operators, anyone whose brand promise is clarity without fuss. AAA-capable — but only with disciplined pairs: bright flat hues fail contrast under white text, so pair them with near-black ink (#1B2631).

**Prompt**
```text
Build a newsletter signup hero in classic 2013 Flat Design (Flat UI palette).
Background: solid midnight navy #2C3E50, white bold sans-serif type, radius 3px
everywhere, absolutely no gradients, shadows, or outlines — box-shadow: none.
Palette: turquoise #1ABC9C, blue #3498DB, orange #F39C12, red #E74C3C, ink #1B2631.
Wordmark: turquoise square + bold white name. Kicker: uppercase text in a flat
#C0392B chip. Headline: 800-weight, last word turquoise. White flat input +
turquoise flat button with dark bold label; hover just darkens to #16A085;
focus = 3px #F39C12 outline. Decorate with pure-CSS flat geometry: a big
turquoise circle bleeding off the corner, a rotated blue square, a red CSS
triangle, an orange envelope. Finish with a 4-column stat strip of solid color
blocks with dark numbers and uppercase labels.
```

**Code**
```html
<style>
.flat{background:#2C3E50;color:#fff;font-family:"Segoe UI",Helvetica,Arial,sans-serif;padding:56px;border-radius:3px;overflow:hidden;position:relative}
.flat *{box-shadow:none!important}
.flat .circ{position:absolute;top:-70px;right:-70px;width:220px;height:220px;border-radius:50%;background:#1ABC9C}
.flat .wm{display:flex;gap:12px;align-items:center;font-weight:800;font-size:24px;margin-bottom:30px}
.flat .wm i{width:44px;height:44px;background:#1ABC9C;color:#1B2631;border-radius:3px;display:grid;place-items:center;font-style:normal}
.flat h1{font-size:56px;font-weight:800;line-height:1.05;margin:0 0 18px;letter-spacing:-.02em}
.flat h1 span{color:#1ABC9C}
.flat p{color:#ECF0F1;font-size:18px;line-height:1.6;max-width:56ch;margin:0 0 28px}
.flat form{display:flex;gap:12px;flex-wrap:wrap;max-width:560px}
.flat input{flex:1;border:0;border-radius:3px;padding:16px 18px;font-size:16px;background:#fff;color:#1B2631}
.flat button{border:0;border-radius:3px;padding:16px 30px;font-size:19px;font-weight:800;background:#1ABC9C;color:#1B2631;cursor:pointer;transition:background 180ms ease}
.flat button:hover{background:#16A085}
.flat input:focus-visible,.flat button:focus-visible{outline:3px solid #F39C12;outline-offset:3px}
.flat .micro{font-size:14px;font-weight:600;margin-top:12px}
</style>
<section class="flat">
  <div class="circ" aria-hidden="true"></div>
  <div class="wm"><i aria-hidden="true">D</i>Dispatch</div>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button>Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p>
</section>
```

---

## 13 · Skeuomorphism
**Live preview:** https://claude.ai/code/artifact/ac05e64a-fd07-43e3-9fe9-b9d87d565ddd

Skeuomorphism is the pre-2013 iOS philosophy of making pixels pretend to be things — stitched saddle leather, linen paper, brass rivets, and buttons so glossy you can almost feel the click. This hero sits a letterpress-embossed paper sheet on a walnut desk, with a 10-stop Aqua-blue Subscribe button and gold-foil wordmark; it suits newsletter writers selling craft, nostalgia, or premium "artisanal" positioning — letters, journals, slow media. Caveat: textures reduce readability and performance is poor, so it's a statement piece, not a fit for critical-accessibility contexts.

**Prompt**
```text
Design a skeuomorphic (2007-2012 iOS) newsletter hero. Dark walnut-wood frame
(#3C2312 base) with inline SVG grain, holding a cream linen-paper sheet
(#F3ECDA) with subtle noise and layered drop shadows. Top: a stitched leather
header bar (gradient #8A4F2D→#3E1F10, dashed cream stitching lines) with a
gold-foil serif wordmark via background-clip:text (#FDF3D0→#CAA055). On the
paper: an engraved pill kicker (inset shadow + letterpress text-shadow), a
Georgia serif headline with the accent word in oxblood gradient, an embossed
subhead. Form: inset email input plus a glossy 3D blue button — 10-stop
gradient #B6D9F2→#164A80 with a hard gloss break at 50%, inset highlights,
layered shadows; press = scale(.97). Riveted brass-cream plaques for stats.
Textures as inline SVG data URIs only; visible focus rings.
```

**Code**
```html
<style>
.skeu{font-family:Georgia,serif;text-align:center;border-radius:12px;overflow:hidden;
  background:linear-gradient(160deg,#5a3a22,#2b180c);box-shadow:0 12px 28px rgba(30,16,5,.45)}
.skeu .bar{padding:16px;background:linear-gradient(180deg,#8a4f2d,#5e3421 52%,#3e1f10);
  border-bottom:2px dashed rgba(240,214,166,.7);box-shadow:inset 0 1px 0 rgba(255,220,170,.35)}
.skeu .wm{font-size:32px;font-weight:700;background:linear-gradient(180deg,#fdf3d0,#caa055);
  -webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent;
  filter:drop-shadow(0 1px 0 rgba(0,0,0,.7))}
.skeu .paper{margin:24px;padding:36px 28px;border-radius:6px;border:1px solid #cfc3a8;
  background:radial-gradient(140% 100% at 50% 0%,#faf5e8,#e3d8bf);
  box-shadow:inset 0 1px 0 #fff,0 6px 14px rgba(25,12,4,.45)}
.skeu h1{font-size:42px;color:#40331f;text-shadow:0 1px 0 rgba(255,255,255,.85)}
.skeu h1 span{color:#8c2c15}
.skeu p{font-family:"Helvetica Neue",Arial,sans-serif;color:#5d4f38;max-width:48ch;margin:12px auto;
  text-shadow:0 1px 0 rgba(255,255,255,.7)}
.skeu form{display:flex;gap:10px;justify-content:center;flex-wrap:wrap;margin-top:20px}
.skeu input{padding:12px 14px;border-radius:8px;border:1px solid #b3a684;font-size:16px;
  background:linear-gradient(180deg,#efe9d8,#fffdf4);box-shadow:inset 0 2px 4px rgba(95,75,40,.35)}
.skeu button{padding:12px 28px;border-radius:9px;border:1px solid #1d4d79;color:#fff;font-weight:700;
  font-size:16px;text-shadow:0 -1px 0 rgba(0,40,80,.55);cursor:pointer;
  background:linear-gradient(180deg,#b6d9f2,#4f97d3 34%,#2e74b4 50%,#1f5c99 76%,#164a80);
  box-shadow:inset 0 1px 0 rgba(255,255,255,.75),inset 0 -2px 4px rgba(0,25,55,.45),0 3px 5px rgba(15,35,60,.45)}
.skeu small{display:block;margin-top:12px;color:#8b7a58;font-family:Arial,sans-serif}
</style>
<section class="skeu"><div class="bar"><span class="wm">Dispatch</span></div><div class="paper">
<h1>The ideas worth your <span>inbox.</span></h1>
<p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
<form onsubmit="return false"><input type="email" placeholder="you@example.com"><button>Subscribe</button></form>
<small>Free forever. Unsubscribe anytime.</small></div></section>
```

---

## 14 · Liquid Glass
**Live preview:** https://claude.ai/code/artifact/7fbcf0ee-03fb-4242-8fbf-dc8e14898d67

Liquid Glass is the 2020s premium successor to frosted glassmorphism: instead of a flat frozen sheet, the UI behaves like polished liquid — morphing droplet lenses on a light airy ground, specular highlights that suggest refraction, pill-shaped fluid controls with bright edge highlights, and a whisper of red-cyan chromatic aberration along every glass edge. It suits newsletter writers selling a high-end feel — premium SaaS commentary, design and luxury-brand dispatches — where the signup form itself should feel like a product demo. Caveat: text contrast over translucent layers is the weak spot, so keep ink dark.

**Prompt**
```text
Build a light-mode newsletter hero in "Liquid Glass" style (liquid lenses, not
frosted glassmorphism). Ground: airy gradient #FBFCFF→#F6EFFA with soft radial
washes of cyan, lilac, and periwinkle. Add 2-3 morphing liquid droplets:
organic border-radius blobs (animate border-radius + slight hue-rotate, 9-13s)
with iridescent fills (#7DF0FF, #C4A0FF, #FFAAD6) and a blurred white specular
highlight at top-left. Center content on a large rounded "lens" panel:
backdrop-filter blur(15px) saturate(160%), translucent white gradient, inset
white top edge, chromatic aberration via paired 2px red/cyan box-shadows.
Near-black ink #171D3A; accent word gradient-clipped #0E7490→#6D28D9→#BE185D.
Pill glass input + gradient Subscribe pill with specular cap and violet
shadow. Glass-bead stats. Reduced-motion guards; 3px focus outlines.
```

**Code**
```html
<style>
.lq{font-family:-apple-system,"Segoe UI",Roboto,sans-serif;color:#171d3a;text-align:center;padding:64px 20px;position:relative;overflow:hidden;
  background:radial-gradient(700px 400px at 10% -10%,rgba(103,232,249,.32),transparent 60%),radial-gradient(600px 380px at 90% 5%,rgba(233,168,255,.34),transparent 62%),linear-gradient(180deg,#fbfcff,#f6effa)}
.lq .drop{position:absolute;width:260px;height:230px;top:-90px;left:-70px;border-radius:58% 42% 55% 45%/52% 55% 45% 48%;
  background:radial-gradient(circle at 30% 24%,rgba(255,255,255,.95),rgba(255,255,255,0) 45%),linear-gradient(135deg,rgba(125,240,255,.3),rgba(196,160,255,.28),rgba(255,170,214,.3));
  box-shadow:inset 2px 3px 6px #fff,-1.5px 0 0 rgba(255,60,90,.16),1.5px 0 0 rgba(0,205,235,.2),0 24px 60px rgba(87,96,178,.18);animation:m 10s ease-in-out infinite alternate}
@keyframes m{to{border-radius:45% 55% 44% 56%/58% 44% 56% 42%;transform:translateY(-12px) rotate(4deg);filter:hue-rotate(20deg)}}
@media(prefers-reduced-motion:reduce){.lq .drop{animation:none}}
.lq .lens{position:relative;max-width:640px;margin:0 auto;padding:48px 32px;border-radius:48px;background:linear-gradient(168deg,rgba(255,255,255,.72),rgba(255,255,255,.4));
  backdrop-filter:blur(15px) saturate(160%);box-shadow:inset 0 2px 2px #fff,-2px 0 0 rgba(255,70,100,.1),2px 0 0 rgba(0,200,230,.12),0 30px 80px rgba(84,92,170,.2)}
.lq h1{font-size:clamp(34px,6vw,56px);letter-spacing:-.02em;line-height:1.05;margin:0}
.lq h1 span{background:linear-gradient(94deg,#0e7490,#6d28d9 55%,#be185d);-webkit-background-clip:text;background-clip:text;color:transparent}
.lq p{max-width:52ch;margin:16px auto 0;line-height:1.6;color:#3b4266}
.lq form{display:flex;flex-wrap:wrap;gap:12px;justify-content:center;margin-top:28px}
.lq input{flex:1 1 240px;height:54px;padding:0 24px;font:inherit;border:0;border-radius:999px;background:rgba(255,255,255,.85);
  box-shadow:inset 0 2px 2px #fff,-1.5px 0 0 rgba(255,70,100,.14),1.5px 0 0 rgba(0,200,230,.16),0 12px 30px rgba(84,92,170,.16)}
.lq button{height:54px;padding:0 32px;font:inherit;font-weight:700;color:#fff;border:0;border-radius:999px;cursor:pointer;
  background:linear-gradient(120deg,#6d28d9,#0e7490);box-shadow:inset 0 2px 2px rgba(255,255,255,.6),0 14px 34px rgba(88,44,190,.38);transition:transform .5s cubic-bezier(.22,.9,.32,1)}
.lq button:hover{transform:translateY(-2px)}.lq input:focus-visible,.lq button:focus-visible{outline:3px solid #6d28d9;outline-offset:3px}
.lq .micro{font-size:13px;color:#4a5177;margin-top:14px}
</style>
<section class="lq"><span class="drop" aria-hidden="true"></span><div class="lens">
<h1>The ideas worth your <span>inbox.</span></h1>
<p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
<form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button type="submit">Subscribe</button></form>
<p class="micro">Free forever. Unsubscribe anytime.</p></div></section>
```

---

## 41 · Cyberpunk UI
**Live preview:** https://claude.ai/code/artifact/30e49e75-e152-43af-8b3b-533bd32d22d6

Cyberpunk UI is the dystopian tech interface: layered neon (cyan, magenta, warning-stripe yellow, a flicker of matrix green) burned into near-black, with clipped angular panels, corner brackets, scanlines, and a headline that glitches like a failing billboard. It suits newsletter writers covering gaming, crypto, dev tools, or anything sci-fi adjacent — audiences who want their inbox to feel like a HUD, not a letter. Caveat: dark-mode only and rated "Limited" for accessibility — keep body copy near-white and confine the neon to accents.

**Prompt**
```text
Build a dark newsletter hero in Cyberpunk UI style. Background #0D0D0D with a
faint cyan grid texture and a scanline overlay. All type monospace. Center
everything in an angular panel with octagonal clip-path notched corners, thin
cyan border, neon corner brackets, and yellow/black warning-stripe bars
(#FCEE0A). Wordmark as a yellow parallelogram badge; kicker in glowing cyan
#00FFFF wrapped in magenta brackets. Uppercase headline in near-white with the
accent word in magenta #FF00FF, neon text-shadow, and a subtle skew/offset
glitch keyframe (respect prefers-reduced-motion). Dark input with cyan border,
notched corners, strong cyan focus glow. Solid #FCEE0A button, dark text,
notched corners, hover shifts to cyan. Stat tiles with different neon left
borders (magenta/cyan/yellow/green) and clipped corners.
```

**Code**
```html
<style>
  .cyb{background:linear-gradient(rgba(0,255,255,.04) 1px,transparent 1px) 0 0/32px 32px,#0D0D0D;
    color:#e8edf2;font-family:ui-monospace,Menlo,Consolas,monospace;text-align:center;
    padding:56px 20px;position:relative;overflow:hidden}
  .cyb::before{content:"";position:absolute;inset:0;pointer-events:none;
    background:repeating-linear-gradient(to bottom,transparent 0 2px,rgba(0,0,0,.22) 3px,transparent 4px)}
  .cyb .panel{max-width:760px;margin:auto;padding:40px 24px;border:1px solid rgba(0,255,255,.4);
    background:rgba(5,6,8,.7);clip-path:polygon(20px 0,calc(100% - 20px) 0,100% 20px,
    100% calc(100% - 20px),calc(100% - 20px) 100%,20px 100%,0 calc(100% - 20px),0 20px)}
  .cyb .wm{display:inline-block;background:#FCEE0A;color:#0D0D0D;font-weight:700;
    letter-spacing:.4em;text-transform:uppercase;padding:6px 16px;
    clip-path:polygon(8px 0,100% 0,calc(100% - 8px) 100%,0 100%)}
  .cyb h1{font-size:clamp(1.8rem,5vw,3rem);text-transform:uppercase;margin:16px 0 0;
    text-shadow:0 0 14px rgba(0,255,255,.3)}
  .cyb h1 span{color:#FF00FF;text-shadow:0 0 12px rgba(255,0,255,.9)}
  .cyb p{color:#cdd6de;max-width:560px;margin:16px auto;line-height:1.7}
  .cyb form{display:flex;flex-wrap:wrap;gap:10px;justify-content:center;max-width:520px;margin:24px auto 0}
  .cyb input{flex:1 1 240px;background:#07090b;color:#00FFFF;border:1px solid rgba(0,255,255,.55);
    padding:13px 15px;font:inherit;clip-path:polygon(10px 0,100% 0,100% calc(100% - 10px),
    calc(100% - 10px) 100%,0 100%,0 10px)}
  .cyb input:focus{outline:2px solid #00FFFF;box-shadow:0 0 16px rgba(0,255,255,.55)}
  .cyb button{background:#FCEE0A;color:#0D0D0D;border:0;font:inherit;font-weight:800;
    letter-spacing:.2em;text-transform:uppercase;padding:13px 26px;cursor:pointer;
    clip-path:polygon(10px 0,100% 0,100% calc(100% - 10px),calc(100% - 10px) 100%,0 100%,0 10px)}
  .cyb button:focus-visible{outline:2px solid #FF00FF;outline-offset:3px}
  .cyb .micro{font-size:12px;letter-spacing:.15em;text-transform:uppercase;color:#9aa3ad}
  .cyb .micro::before{content:">_ ";color:#00FF00}
</style>
<section class="cyb"><div class="panel">
  <div class="wm">Dispatch</div>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button type="submit">Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p>
</div></section>
```

---

## 47 · Exaggerated Minimalism
**Live preview:** https://claude.ai/code/artifact/fb6f453b-2d75-45cf-9777-b2e743dcbae6

Exaggerated Minimalism is minimalism turned up to eleven: a viewport-swallowing headline that flirts with cropping off the edge, featherweight thin type slammed against 900-weight black, oceans of empty white, and exactly one loud accent (hot orange on "inbox."). It's the fashion-agency, luxury-editorial take — perfect for writers with a strong point of view who want the design to say "we don't need to shout... except once, enormously." Holds WCAG AA; skip it for data-heavy layouts or older audiences — extreme scale and hairline weights aren't for everyone.

**Prompt**
```text
Build a newsletter hero in "Exaggerated Minimalism" (fashion-agency
bold-minimal). Pure #FFFFFF background, #000000 ink, exactly ONE accent:
#FF4D00 — only on the last headline word and focus states. Headline absurdly
oversized: clamp(3rem, 11.5vw, 12rem), letter-spacing -0.05em, line-height
0.92; first words weight 100, last words weight 900. Add a giant cropped ghost
word ("DISPATCH" at ~30vw, 5% black) bleeding off the corner via
overflow:hidden. Vast whitespace (8rem+ vertical padding, ~90vh hero). Tiny
scattered 9-10px uppercase detail text. Borderless email input with a 2px
black bottom border (orange on focus); square black Subscribe button in 12px
900-weight uppercase with 0.3em tracking. Hairline-ruled stats row at the
bottom. No shadows, no radius, no decoration — air and scale do the work.
```

**Code**
```html
<style>
  .exmin{background:#fff;color:#000;font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;position:relative;overflow:hidden;padding:8rem clamp(1.5rem,6vw,6rem) 5rem;min-height:90vh}
  .exmin .ghost::before{content:"DISPATCH";position:absolute;right:-.18em;bottom:-.24em;font-size:clamp(10rem,34vw,30rem);font-weight:900;letter-spacing:-.06em;color:rgba(0,0,0,.05);white-space:nowrap;pointer-events:none}
  .exmin h1{font-size:clamp(3rem,11.5vw,12rem);line-height:.92;letter-spacing:-.05em;font-weight:100;max-width:12ch;position:relative}
  .exmin h1 b{font-weight:900;display:block}
  .exmin h1 .accent{color:#ff4d00;font-weight:900}
  .exmin .sub{margin-top:4rem;font-weight:300;line-height:1.75;max-width:34rem;position:relative}
  .exmin form{margin-top:3.5rem;display:flex;flex-wrap:wrap;max-width:34rem;position:relative}
  .exmin input{flex:1 1 220px;font:inherit;font-weight:300;padding:1.1rem 0;border:0;border-bottom:2px solid #000;background:none;outline:none}
  .exmin input:focus-visible{border-bottom-color:#ff4d00;box-shadow:0 2px 0 #ff4d00}
  .exmin button{font:inherit;font-size:12px;font-weight:900;letter-spacing:.3em;text-transform:uppercase;padding:1.1rem 2.4rem;border:2px solid #000;background:#000;color:#fff;cursor:pointer}
  .exmin button:hover{background:#ff4d00;border-color:#ff4d00}
  .exmin button:focus-visible{outline:3px solid #ff4d00;outline-offset:3px}
  .exmin .micro{margin-top:1.4rem;font-size:10px;font-weight:300;letter-spacing:.26em;text-transform:uppercase;opacity:.55}
</style>
<section class="exmin">
  <div class="ghost" aria-hidden="true"></div>
  <h1>The ideas <b>worth your <span class="accent">inbox.</span></b></h1>
  <p class="sub">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button type="submit">Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p>
</section>
```

---

## 57 · Gen Z Chaos / Maximalism
**Live preview:** https://claude.ai/code/artifact/2df65065-7c61-44ad-8954-7f2f09275544

Gen Z Chaos is the sticker-bomb aesthetic of 2023+ internet core: a saturated conic-gradient soup layered with rotated white-bordered stickers, torn-paper strips, starbursts, outline type, and highlight strips — colors that clash on purpose and a layout that looks dragged-and-dropped but still reads top to bottom. It suits newsletter writers with a loud personal brand: culture commentary, music and fashion drops, meme-literate marketing — anyone whose unsubscribe button is a dare. Caveat: accessibility is rated Poor, so keep body copy on solid white sticker cards and honor prefers-reduced-motion.

**Prompt**
```text
Build a newsletter signup hero in Gen Z Chaos / Maximalism (sticker-bomb
collage). Background: conic-gradient mixing #FF00FF, #FF5F1F, #FFFF00,
#00FF00, #00F0FF, #0000FF with radial blobs, filter saturate(150%). Scatter
aria-hidden stickers with absolute positioning and random rotations:
starbursts via clip-path polygon, torn-paper strips, badges with 4px white
borders + 0 0 0 3px black ring + hard offset shadows, semi-transparent tape.
Wordmark as a rotated magenta pill sticker; kicker on a #FFFF00 highlight
strip with 3px black border. Headline mixes treatments: filled white words
with layered black/blue text-shadow and "inbox." as a rotated yellow sticker
chip with pink offset shadow. Subhead on a clean white rotated card so body
copy stays legible. White input + #00FF00 button, both with 4px black borders,
clashing offset shadows, counter-rotations, dashed focus outlines. Four stat
stickers in yellow/magenta/green/blue, each rotated a few degrees.
```

**Code**
```html
<style>
.gz{--pk:#FF00FF;--gr:#00FF00;--yl:#FFFF00;--bl:#0000FF;font-family:Arial,sans-serif;text-align:center;overflow:hidden;position:relative;padding:56px 20px;filter:saturate(150%);
  background:conic-gradient(from 40deg,#FF00FF,#FF5F1F,#FFFF00,#00FF00,#00F0FF,#0000FF,#FF00FF);}
.gz .star{position:absolute;width:110px;height:110px;background:var(--yl);filter:drop-shadow(4px 6px 0 rgba(0,0,0,.5));
  clip-path:polygon(50% 0,61% 35%,98% 35%,68% 57%,79% 91%,50% 70%,21% 91%,32% 57%,2% 35%,39% 35%);}
.gz .s1{top:-20px;left:-20px;transform:rotate(-14deg)}.gz .s2{bottom:-24px;right:-18px;background:var(--pk);transform:rotate(18deg)}
.gz .wm{display:inline-block;background:var(--pk);color:#fff;font-weight:900;font-style:italic;text-transform:uppercase;font-size:26px;
  padding:8px 20px;border:4px solid #fff;border-radius:12px;box-shadow:0 0 0 3px #111,6px 8px 0 rgba(0,0,0,.5);transform:rotate(-4deg)}
.gz h1{font-size:clamp(38px,8vw,80px);font-weight:900;text-transform:uppercase;line-height:1;margin:22px auto 0;max-width:16ch;
  color:#fff;text-shadow:3px 3px 0 #111,6px 6px 0 var(--bl)}
.gz h1 span{color:#111;background:var(--yl);text-shadow:none;display:inline-block;padding:.02em .18em;
  border:4px solid #111;border-radius:.18em;box-shadow:6px 6px 0 var(--pk);transform:rotate(2deg)}
.gz p{max-width:46ch;margin:24px auto 0;background:#fff;color:#222;font-weight:600;line-height:1.55;
  padding:14px 20px;border:3px solid #111;border-radius:14px;box-shadow:7px 8px 0 rgba(0,0,0,.5);transform:rotate(-1deg)}
.gz form{display:flex;flex-wrap:wrap;gap:12px;justify-content:center;margin-top:26px}
.gz input{flex:1 1 220px;font:inherit;font-weight:700;padding:14px 16px;border:4px solid #111;border-radius:12px;
  box-shadow:5px 6px 0 var(--bl);transform:rotate(-1deg)}
.gz button{font:900 16px/1 Arial;text-transform:uppercase;padding:14px 28px;background:var(--gr);color:#111;cursor:pointer;
  border:4px solid #111;border-radius:12px;box-shadow:5px 6px 0 var(--pk);transform:rotate(1.5deg)}
.gz input:focus-visible,.gz button:focus-visible{outline:4px dashed #111;outline-offset:4px}
.gz .mc{display:inline-block;margin-top:16px;background:#111;color:var(--gr);font-size:12px;font-weight:800;
  text-transform:uppercase;padding:6px 14px;border-radius:999px;border:2px solid #fff;transform:rotate(-2deg)}
</style>
<section class="gz"><i class="star s1"></i><i class="star s2"></i>
  <div class="wm">Dispatch</div>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p>One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button>Subscribe</button></form>
  <span class="mc">Free forever. Unsubscribe anytime.</span>
</section>
```

---

## 08 · Accessible & Ethical
**Live preview:** https://claude.ai/code/artifact/12ca5c26-b5ec-496a-8b24-b80dd0236c01

Accessible & Ethical is what happens when WCAG AAA stops being a checklist and becomes the aesthetic itself: deep navy on warm off-white at 12:1 contrast, 18px+ body type, 56px touch targets, and chunky two-tone focus rings worn like jewelry rather than hidden in shame. It suits newsletter writers with genuinely large, mixed audiences — policy, health, education, anyone whose credibility depends on being readable by everyone. "Accessible" here is a design stance, not a compromise: every constraint forces clarity, and clarity is the most premium look there is.

**Prompt**
```text
Build a newsletter hero in an "Accessible & Ethical" WCAG AAA style.
Background warm off-white #FBF9F4, all text deep navy #1A2B4A (≈12:1), one
accent: deep teal #005A52 (7.6:1 — AAA even at small sizes). System fonts.
Body 18-21px, line-height 1.65; headline clamp(40px,7vw,68px), weight 800,
accent word in teal plus a thick 6px underline (never color alone). Input:
white, 2px navy border, 56px tall. Button: teal, white text, 56px tall.
Signature focus states: outline 4px solid navy, outline-offset 3px, plus
box-shadow 0 0 0 3px off-white for a two-tone ring with a visible gap. 6px
navy/teal top rule; stats divided by hairlines under a 3px navy rule;
checkmark before the microcopy. Semantic HTML, aria-labels, reduced-motion
kill-switch. No decorative images, no gradients, no motion.
```

**Code**
```html
<style>
.a11y{--paper:#FBF9F4;--ink:#1A2B4A;--teal:#005A52;background:var(--paper);color:var(--ink);
  font-family:-apple-system,"Segoe UI",Roboto,Arial,sans-serif;padding:64px 24px;border-top:6px solid var(--ink)}
.a11y .wrap{max-width:820px;margin:0 auto}
.a11y .wm{font-weight:800;font-size:24px;border-bottom:4px solid var(--teal);display:inline-block;padding-bottom:2px}
.a11y .kick{margin-top:10px;font-size:15px;font-weight:600;letter-spacing:.14em;text-transform:uppercase;color:var(--teal)}
.a11y h1{font-size:clamp(38px,6vw,64px);line-height:1.08;font-weight:800;letter-spacing:-.02em;margin:28px 0 20px}
.a11y h1 span{color:var(--teal);text-decoration:underline;text-decoration-thickness:6px;text-underline-offset:8px}
.a11y p.sub{font-size:19px;line-height:1.65;max-width:58ch;margin-bottom:32px}
.a11y form{display:flex;flex-wrap:wrap;gap:12px;max-width:540px}
.a11y input{flex:1 1 240px;min-height:56px;font-size:18px;padding:0 16px;border:2px solid var(--ink);border-radius:8px;background:#fff;color:var(--ink)}
.a11y button{min-height:56px;min-width:160px;font-size:18px;font-weight:700;color:#fff;background:var(--teal);border:2px solid var(--teal);border-radius:8px;cursor:pointer}
.a11y :is(input,button):focus-visible{outline:4px solid var(--ink);outline-offset:3px;box-shadow:0 0 0 3px var(--paper)}
.a11y .micro{margin-top:14px;font-size:16px;font-weight:600}.a11y .micro::before{content:"✓ ";color:var(--teal)}
@media (prefers-reduced-motion:reduce){.a11y *{animation:none!important;transition:none!important}}
</style>
<section class="a11y"><div class="wrap">
  <span class="wm">Dispatch</span>
  <p class="kick">The Weekly Dispatch · Issue N°142</p>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p class="sub">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false" aria-label="Subscribe to Dispatch"><input type="email" placeholder="you@example.com" aria-label="Email address" autocomplete="email"><button type="submit">Subscribe</button></form>
  <p class="micro">Free forever. Unsubscribe anytime.</p>
</div></section>
```

---

## 21 · Conversion-Optimized
**Live preview:** https://claude.ai/code/artifact/99ce771d-67e8-4d89-926a-fb836dd31338

Conversion-Optimized isn't really an aesthetic — it's a discipline. Everything on the page exists to move your eye down one path: benefit headline, social proof, one unmissable green button, and nothing else competing for attention on a clean white ground. If you're a newsletter writer who cares more about your signup rate than your mood board — solo operators, paid-newsletter hopefuls, anyone A/B testing their landing page — this is the pattern that quietly converts at 12% while prettier heroes convert at 2%.

**Prompt**
```text
Build a newsletter signup hero in classic conversion-optimized landing style.
White background (#FFFFFF), near-black text (#0F172A), muted gray secondary
(#475569). Single-column F-pattern layout, max-width 640px, left-aligned. Big
bold headline (clamp 34-54px, -0.03em tracking) with one word accented in
green #16A34A. One email input + Subscribe button row: 56px tall, 10px
radius; button solid #16A34A, white text, subtle green shadow, hover darkens
to #15803D and scales 1.02. Focus: 3px green ring on input, dark outline on
button; respect prefers-reduced-motion. Add a small CSS-drawn down-arrow
pointing at the form, honest microcopy with a check icon, and a 4-column
stats row with green check dots as trust signals under a thin divider. No
urgency timers, no other colors, no distractions.
```

**Code**
```html
<style>
.cv{background:#fff;color:#0F172A;font-family:-apple-system,"Segoe UI",Roboto,Arial,sans-serif;padding:64px 20px}
.cv .w{max-width:640px;margin:0 auto}
.cv .wm{font-weight:800;font-size:20px}
.cv .wm::before{content:"";display:inline-block;width:12px;height:12px;border-radius:3px;background:#16A34A;margin-right:8px}
.cv .k{margin:24px 0 0;font-size:13px;font-weight:600;letter-spacing:.12em;text-transform:uppercase;color:#475569}
.cv h1{margin:12px 0 0;font-size:clamp(34px,6vw,52px);line-height:1.06;letter-spacing:-.03em;font-weight:800}
.cv h1 span{color:#16A34A;box-shadow:inset 0 -.14em 0 0 rgba(22,163,74,.25)}
.cv .s{margin:16px 0 24px;font-size:17px;line-height:1.6;color:#475569;max-width:54ch}
.cv form{display:flex;gap:10px;max-width:600px}
.cv input{flex:1;min-width:0;height:56px;padding:0 18px;font-size:16px;border:2px solid #CBD5E1;border-radius:10px}
.cv input:focus{outline:none;border-color:#16A34A;box-shadow:0 0 0 3px rgba(22,163,74,.3)}
.cv button{height:56px;padding:0 32px;font-size:17px;font-weight:700;color:#fff;background:#16A34A;border:none;border-radius:10px;cursor:pointer;box-shadow:0 2px 6px rgba(22,163,74,.35)}
.cv button:hover{background:#15803D}
.cv button:focus-visible{outline:3px solid #0F172A;outline-offset:2px}
.cv .m{margin:12px 0 0;font-size:14px;color:#475569}
@media(max-width:560px){.cv form{flex-direction:column}.cv button{width:100%}}
</style>
<section class="cv"><div class="w">
  <span class="wm">Dispatch</span>
  <p class="k">The Weekly Dispatch · Issue N°142</p>
  <h1>The ideas worth your <span>inbox.</span></h1>
  <p class="s">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button type="submit">Subscribe</button></form>
  <p class="m">Free forever. Unsubscribe anytime.</p>
</div></section>
```

---

## 67 · Chromatic Aberration / RGB Split
**Live preview:** https://claude.ai/code/artifact/b2205c49-997d-428a-87b4-f56621519ad8

Chromatic Aberration turns a broken lens into a brand: everything sits on a near-black charcoal ground while red and cyan channel ghosts fringe the type, as if the signal never quite locked in. Instead of decoration, the misalignment itself is the design — a rare, sparse glitch slices through the headline, scanlines drift, and the button's RGB shadow spreads on hover. It suits music, gaming, and creative-tech newsletters that want an edgy analog-error vibe; skip it for corporate, healthcare, finance, or accessibility-critical audiences — the effect can cause eye strain, so keep splits off body text and honor reduced-motion.

**Prompt**
```text
Build a dark newsletter hero in a chromatic aberration / RGB split style.
Ground: near-black charcoal #0B0B0E, white text #F2F2F2, monospace
kicker/wordmark, bold sans headline. The RGB split IS the design language —
no gradients, grids, or HUD elements. Headline: text-shadow -3px 0 #FF0000
and 3px 0 #00FFF9; accent word gets a doubled offset plus 0 2px
rgba(0,255,0,.5). Add aria-hidden ghost layers (content: attr(data-text),
mix-blend-mode: screen) in pure red/blue that jitter and clip-path-slice for
~0.3s once every 4s. Overlay subtle CRT scanlines (1px lines every 4px at
~10% opacity, slowly drifting). Input: dark #131318 with focus ring as split
box-shadow (-3px 0 red, 3px 0 cyan); white Subscribe button whose red/blue
drop shadows widen on hover. Keep subhead shadow-free for readability;
disable all glitch animation under prefers-reduced-motion.
```

**Code**
```html
<style>
  .rgb-hero{background:#0b0b0e;color:#f2f2f2;font-family:-apple-system,"Segoe UI",Arial,sans-serif;
    text-align:center;padding:64px 24px;position:relative;overflow:hidden}
  .rgb-hero::before{content:"";position:absolute;inset:0;pointer-events:none;opacity:.1;
    background:repeating-linear-gradient(to bottom,rgba(255,255,255,.05) 0 1px,transparent 1px 4px)}
  .rgb-wm{font-family:Menlo,Consolas,monospace;letter-spacing:.4em;text-transform:uppercase;font-weight:700;
    text-shadow:-2px 0 #ff0000,2px 0 #0000ff}
  .rgb-hero h1{font-size:clamp(2.2rem,6vw,4rem);font-weight:800;margin:18px auto 0;line-height:1.05;
    text-shadow:-3px 0 #ff0000,3px 0 #00fff9}
  .rgb-hero h1 .accent{text-shadow:-5px 0 #ff0000,5px 0 #00fff9,0 2px rgba(0,255,0,.5)}
  .rgb-sub{max-width:560px;margin:20px auto 0;line-height:1.6;color:#c9c9d1}
  .signup{margin-top:28px;display:flex;gap:10px;justify-content:center;flex-wrap:wrap}
  .signup input{padding:12px 16px;background:#131318;border:1px solid #34343e;color:#f2f2f2;
    font-family:Menlo,monospace;border-radius:2px}
  .signup input:focus-visible{outline:none;border-color:#f2f2f2;box-shadow:-3px 0 0 #ff0000,3px 0 0 #00fff9}
  .signup button{padding:12px 24px;background:#f2f2f2;color:#000;border:0;border-radius:2px;cursor:pointer;
    font-family:Menlo,monospace;font-weight:700;text-transform:uppercase;letter-spacing:.08em;
    box-shadow:-2px 0 0 #ff0000,2px 0 0 #0000ff;transition:box-shadow .15s}
  .signup button:hover{box-shadow:-5px 0 0 #ff0000,5px 0 0 #0000ff,0 3px 0 rgba(0,255,0,.55)}
  .rgb-micro{margin-top:12px;font-family:Menlo,monospace;font-size:.72rem;letter-spacing:.12em;
    text-transform:uppercase;color:#9a9aa2}
</style>
<section class="rgb-hero">
  <div class="rgb-wm">Dispatch</div>
  <h1>The ideas worth your <span class="accent">inbox.</span></h1>
  <p class="rgb-sub">One email every Friday. Big ideas, clear thinking, and zero noise — for 24,000 readers who like their insights sharp and their inboxes calm.</p>
  <form class="signup" onsubmit="return false"><input type="email" placeholder="you@example.com" aria-label="Email address"><button type="submit">Subscribe</button></form>
  <p class="rgb-micro">Free forever. Unsubscribe anytime.</p>
</section>
```
