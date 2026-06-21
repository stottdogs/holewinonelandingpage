# Brand Sheet Scope

_Started 2026-06-21 09:40 UTC_

---

## User

<system-info comment="Only acknowledge these if relevant">
Project title is now "Untitled"
The project currently has no files except possibly dotfiles — a `list_files` on the project root would return nothing else.
Current date is now June 21, 2026
</system-info>

<default aesthetic_system_instructions>
The user has not attached a design system. If they have ALSO not attached references or art direction, and the project is empty, you must ASK the user what visual aesthetic they want. Use the questions_v2 tool to ask about preferred vibe, audience, colors, type, mood, etc. Do NOT just pick your own visual aesthetic without getting the user's aesthetic input -- this is how you get slop!

Once answered, use this guidance when creating designs:
- Choose a type pairing from web-safe set or Google Fonts. Helvetica is a good choice. Avoid hard-to-read or overly stylized fonts. Use 1-3 fonts only.
- Foreground and background: choose a color tone (warm, cool, neutral, something in-between). Use subtly-toned whites and blacks; avoid saturations above 0.02 for whites.
- Accents: choose 0-2 additional accent colors using oklch. All accents should share same chroma and lightness; vary hue.
- NEVER write out an SVG yourself that's more complicated than a square, circle, diamond, etc.
- For imagery, never hand-draw SVGs; use subtly-striped SVG placeholders instead with monospace explainers for what should be dropped there (e.g. “product shot”)

CRITICAL: ignore default aesthetic entirely if given other aesthetic instructions like reference images, design systems or guidance, or if there are files in the project already.
</default aesthetic_system_instructions>

<pasted_text name="Pasted text (29 lines)">
Here's a design prompt you can drop straight into a logo/brand tool (Canva, Midjourney, DALL·E, or a freelance brief):

---

**Brand:** HoleWinOne

**What it is:** A self-serve, trailer-mounted hole-in-one golf jackpot challenge. Players pay for shots at a 100m target for a chance at a growing cash jackpot (up to $10,000). It deploys at wineries, resorts, golf courses, and holiday parks.

**Critical positioning note:** The audience is *not* golfers — it's entertainment-seekers and prize-chasers at leisure venues, often a bit tipsy, looking for a fun dare with friends. The brand should NOT look like a traditional country-club / golf-pro identity (no muted greens, no crests, no serif "established 1920" vibe). Think carnival jackpot energy meets premium leisure venue — closer to a lottery scratchie or a fairground prize wheel than a golf brand.

**Logo requirements:**
- Wordmark: "HoleWinOne" — ideally with clever visual emphasis splitting WIN out of the name (e.g., bold/contrast treatment on "WIN")
- Icon option: should work as a standalone mark for app icons and small signage — consider a golf ball mid-flight into a target, or a golf ball morphing into a coin/jackpot symbol
- Must read clearly and feel premium even when small (trailer decals, app icon, social avatar)
- Needs a single-color/reversed version for embroidery, signage, and low-cost print

**Tone:** Bold, exciting, a little cheeky, premium-leisure rather than budget-carnival. Should feel at home next to a winery's branding, not clash with it.

**Color direction:** High-energy but not garish — think jackpot gold/yellow as an accent against a confident base color (deep green, navy, or black), so it reads "prize" without reading "kids' party." Avoid traditional golf-green-on-white.

**Typography feel:** Bold, modern, slightly playful sans-serif — confident and easy to read at a distance (people will be deciding whether to play while walking past a trailer).

**Must avoid:** generic golf clipart (flags, tees, clubs as the hero element), country-club seriousness, cheap fairground clip-art look, anything that reads "golf skill" over "have a go and win."

**Use cases it needs to survive:** trailer wrap/signage, app icon, Stripe receipt header, Instagram/TikTok overlay sticker, investor one-pager.

---

Want me to actually generate some logo concepts now using Canva, or were you planning to take this prompt elsewhere?
</pasted_text>

<!-- The user explicitly selected the following skills for this project, as attachments to their message. These are not optional context — they define how you work. Use them. -->
<attached-skill name="Design Components">
This project uses Design Components: every design is a single streaming `Name.dc.html` file. The full authoring spec is in your system prompt under "Writing code — Design Components" — follow it. Author and edit `.dc.html` content with the `dc_write`, `dc_html_str_replace`, `dc_js_str_replace`, and `dc_set_props` tools (not `write_file`; `str_replace_edit` works but won't stream); template edits stream into the live preview as you type.
</attached-skill>


<system-reminder>Auto-injected reminder (ignore if not relevant): do not recreate copyrighted or branded UI unless the user's email domain matches that company. Create original designs instead.</system-reminder>

## Assistant

I can build logo/wordmark concepts for **HoleWinOne** as a Design Component. Before I start, a few quick questions so I don't waste a round generating the wrong direction.

_[tool: questions_v2]_

## User

Questions answered:
- deliverable: A full mini brand sheet (logo + colors + type + lockups)
- num_concepts: Decide for me
- base_color: Deep green (not country-club — rich emerald/forest)
- win_treatment: Strong — boxed/highlighted WIN that pops
- icon_dir: Decide for me
- type_feel: Decide for me
- energy: 7

## Assistant

Brand sheet it is — deep emerald base, jackpot gold, a boxed **WIN**. Setting up the project and building it as a single streaming Design Component.

_[tool: set_project_title]_

_[tool: update_todos]_

_[tool: dc_write]_

_[tool: update_todos]_

_[tool: show_html]_

The brand sheet is built. Letting the verifier check it.

_[tool: ready_for_verification]_

Done. **HoleWinOne** mini brand sheet — a single scrolling page covering:

- **Hero** with the primary lockup and the boxed-gold **WIN**
- **Logo system** — horizontal, stacked, wordmark-only, and a 1-ink reversed version (outlined WIN) for embroidery/signage
- **The mark** — a golf-ball-into-target that doubles as a jackpot coin, shown as app icon, reversed, and 1-colour
- **Colour** (jackpot gold + deep emerald + ink + cream, with hex/oklch), **type** (Archivo / Space Grotesk / Space Mono)
- **In the wild** — trailer wrap, Stripe receipt header, social sticker
- **Do & Don't** guardrails

Deep emerald base, jackpot gold accent, premium-leisure energy — no clubs, crests, or country-club greens.

Want me to push any direction further (e.g. a navy or black base variant for comparison), or apply the logo to a real trailer/app-icon mockup?

## User

/design-login

## Assistant

I don't recognize a `/design-login` command. Did you mean something specific — a login/sign-in screen for the HoleWinOne app, or something else? Let me know and I'll build it.

## User

<system-info comment="Only acknowledge these if relevant">
Project title is now "Brand Sheet Scope"
What `list_files` on the project root returns right now (dotfiles, if any, are not shown here):
📄 HoleWinOne Brand Sheet.dc.html
📄 support.js
User is viewing file: HoleWinOne Brand Sheet.dc.html
Current date is now June 21, 2026
</system-info>

<pasted_text name="Pasted text (29 lines)">
Here's a ready-to-paste prompt for Claude (design/website builder). I've scoped it to a single consumer landing page with a nav link out to a future "For Courses" page.

---

**Prompt — Hole-Win-One landing page**

&gt; Design and build a single, public-facing **landing page** for **Hole-Win-One**, a hole-in-one jackpot game played on real golf courses. Output a polished, responsive one-page site (mobile-first — most visitors arrive by scanning a QR code on the course).
&gt;
&gt; **Audience:** everyday golfers standing at a Par 3, plus casual visitors discovering the brand. Tone: fun, energetic, trustworthy, and a little bit "lottery-meets-golf." Not corporate. Build excitement about a real cash jackpot while making it feel fair and legit.
&gt;
&gt; **The one-sentence pitch:** Scan the QR code at the tee, pay $5, take your swing — if you ace the hole, you win the course's live jackpot.
&gt;
&gt; **Page sections, top to bottom:**
&gt; 1. **Hero** — big headline (e.g. "One swing. One shot. The whole jackpot."), a live-jackpot feel (show an animated odometer-style number around **$2,500–$5,000 AUD**), and a primary CTA "**See How It Works**". Background should evoke a golf course at a Par 3.
&gt; 2. **How it works** — 4 simple steps with icons: **Scan** the QR at the tee → **Pay $5** → **Record your swing** → **Win** the local jackpot if you ace it. Keep it dead simple.
&gt; 3. **Why it's legit** — 3 trust points: every Par 3 has permanent on-course sensors + camera that verify your shot; jackpots are real and grow $1 with every attempt (floor $2,500, cap $5,000); if the hardware ever faults, you're automatically refunded.
&gt; 4. **The jackpot** — explain one shared pool per course that climbs with play, with a visual of the number ticking up.
&gt; 5. **FAQ** — short answers: How much does it cost? ($5 per attempt, flat.) How do you know if I made it? (course sensors + camera verify automatically). What if something goes wrong? (auto-refund). Do I need an account? (no — just scan and play).
&gt; 6. **Footer** — brand mark, and a clear nav/CTA link to a **"For Golf Courses"** page (link to `/for-courses`, which doesn't exist yet — just make it a working anchor/button). Tagline like "Run a course? Earn from every swing →".
&gt;
&gt; **Navigation:** simple top nav with the logo, "How it works", "FAQ", and a "For Courses" link to `/for-courses`.
&gt;
&gt; **Brand &amp; visual style:** golf-inspired but modern and bold — deep fairway greens, clean whites, and a high-energy accent (gold/amber for the jackpot money moments). Big confident typography, generous spacing, rounded cards, subtle motion on the jackpot number. Currency shown in **AUD**. Fully responsive, fast, accessible.
&gt;
&gt; Keep all copy concise and punchy. No login, no signup — this page only informs and excites; the actual game lives behind the on-course QR code.

---

Want me to tailor it for a specific tool (e.g. claude.ai/code with React + Tailwind to match your existing stack, vs. a generic design generator)? I can also draft the matching **For Courses** prompt now so it's ready when you build that page.
</pasted_text>

## Assistant

Clear scope and I already have the brand system locked. Building the landing page as a Design Component using the same emerald/gold palette and Archivo/Space Grotesk type. I'll make the jackpot odometer animate via the logic class so it survives re-renders.

_[tool: update_todos]_

_[tool: dc_write]_

_[tool: show_html]_

_[tool: update_todos]_

_[tool: ready_for_verification]_

Built the **Hole-Win-One landing page** on the existing brand system — mobile-first, fully responsive.

- **Sticky nav** → logo, How it works, FAQ, and a gold "For Courses" button (→ `/for-courses`)
- **Hero** → "One swing. One shot. The whole jackpot." with a live-ticking jackpot odometer (animates $2,500→$3,460, then keeps climbing $1 at a time) + "See How It Works" CTA over a layered fairway
- **How it works** → Scan → Pay $5 → Take your swing → Win (the Win card flips to emerald/gold)
- **Why it's legit** → sensors+camera verify, real growing jackpot, auto-refund on fault
- **The jackpot** → floor/+$1/cap stats + a live card with a progress bar filling from $2,500 to $5,000
- **FAQ** → 4 accordion items
- **For Courses** gold CTA band + footer, both linking `/for-courses`. AUD throughout, 18+ note.

Want me to draft the matching **For Courses** page next so that link lands somewhere real?

