Build a flagship product showcase landing page in React and Tailwind CSS modeled directly after Apple Thailand (apple.com/th).

STRICT DESIGN SYSTEM (Avoid generic AI templates):
1. Color & Surface Alternation:
   - Alternate full-bleed edge-to-edge sections between crisp light gray (`#F5F5F7`) with near-black ink (`#1D1D1F`) and pure pitch black (`#000000`) with pure white text (`#F5F5F7`).
   - NO drop shadows, NO card borders, NO glassmorphism on product sections, and NO purple/indigo gradients.
   - Primary CTA Accent: Classic Apple Blue (`#0071E3` background, `#0077ED` hover).

2. Navigation & Promo Ribbon:
   - Sticky top global navbar (`h-11`, `bg-[#161617]/80 backdrop-blur-md`) with centered micro-links (`text-xs text-white/80 hover:text-white tracking-normal`).
   - Immediately below navbar: A clean white or `#F5F5F7` single-line promo ribbon (`text-xs py-3 text-center`) with an inline blue link (`text-[#0066CC] hover:underline`).

3. Hero & Bento Grid Architecture:
   - Top 3 stacked full-width heกro sections (`min-h-[580px]`), centered top-aligned typography, large product imagery anchored cleanly at the bottom.
   - Followed by a 2-column split grid (`grid-cols-1 md:grid-cols-2 gap-3 p-3 bg-white`) where each tile is a self-contained `#F5F5F7` or `#000000` showcase with zero border-radius (`rounded-none`).
   - Dual-CTA Pattern: Every product block must feature two side-by-side pill buttons (`rounded-full px-5 py-2 text-sm`):
     * Primary: Solid `#0071E3` text-white ("ดูเพิ่มเติม").
     * Secondary: Outlined `border border-[#0071E3] text-[#0071E3] hover:bg-[#0071E3] hover:text-white` ("ซื้อ").

4. Formal Thai Typography Rules:
   - Import Google Fonts: 'IBM Plex Sans Thai' (weights: 300, 400, 500, 600, 700) and 'Inter' (for English product names/numbers).
   - Font Stack: `'Inter', 'IBM Plex Sans Thai', sans-serif`.
   - Thai Spacing Fixes: Keep `tracking-normal` on all Thai headlines (never use negative tracking on Thai script). Use `leading-[1.3]` on large headings (`text-4xl md:text-5xl font-semibold`) and `leading-relaxed` on subheadings (`text-lg md:text-xl font-normal text-[#6E6E73]`) so Thai tone marks never collide.
   - Copywriting: Use concise, refined, official Thai product marketing copy.

5. Multi-Column Legal Footer:
   - Light gray footer (`#F5F5F7`) with `text-[11px] text-[#6E6E73] leading-relaxed` legal footnotes separated by a `1px` `#D2D2D7` divider, followed by a clean 5-column directory grid.
