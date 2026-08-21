# Session Log — 2026-08-21

Work done today on the `sivasoundhar/sivasoundhar` GitHub profile README.

## Built
- Created the profile README from scratch (header banner, badges, About Me,
  Featured Projects, Certifications, footer).
- Simplified structure to a minimal layout: header → badges → About Me table →
  Featured Projects → Certifications → footer.

## Content iterations
- Trimmed the original long-form draft: removed the "Seven years of
  simulating..." intro paragraph and the full "Engineering Background"
  section (Segula/Mercedes-Benz/Expleo bio + achievement bullets).
- Reworked the header tagline several times: "AI Engineer • CAE & Simulation
  Background" → "AI Engineer • Agentic Systems and Applied ML" →
  final: **"Design, CAE and AI Engineering"**.
- Updated the "Experienced on" row to: Design, CAE & Simulation Engineering,
  Healthcare.
- Replaced the GitHub stats/top-languages/streak cards with a "Featured
  Projects" section listing the three real projects (UniRAG, PatientShield-AI,
  Medical Imaging AI Copilot) with one-line descriptions, tech tags, and
  repo links.
- Added a **Certifications** section with the CITI Program "Human Research
  (Data or Specimens Only Research)" credential (MIT Affiliates). Linked the
  title to the actual certificate PDF now stored in `certs/` in this repo,
  plus a secondary link to the public CITI verification page.

## Bugs found and fixed
- **Broken stats cards**: the public `github-readme-stats.vercel.app`
  instance was returning `503` (overloaded/rate-limited). Switched to the
  `github-readme-stats-six-seven.vercel.app` mirror (later removed entirely
  when stats were replaced by Featured Projects).
- **Header text invisible**: the header's CSS fade-in animation
  (`opacity: 0 → 1`) appears to get suppressed by GitHub's camo image proxy,
  leaving the "Siva S" title and tagline permanently stuck at `opacity: 0`
  (invisible), even though the banner shape rendered fine. Fixed by adding
  `&animation=false` to the capsule-render URL so text renders statically
  visible with no animation dependency.
- **Broken header SVG (XML parse error)**: while testing `type=venom` for a
  "real" continuous animation, an unescaped `&` in the description text
  broke XML parsing (`xmlParseEntityRef: no name`), producing a fully broken
  image. Fixed by removing the literal `&` from the text. Also found `venom`
  renders as an oversized blob unsuited to a text banner layout, so reverted
  to `type=waving`.
- Verified every fix by actually loading the live GitHub page in a browser
  (not just checking HTTP status codes) after being burned by an
  animation-suppression issue that curl/HTTP checks couldn't reveal.

## Investigated (not changed)
- Audited three local projects against the README's "Featured Work" links:
  - `D:\projects\UniRag` → pushed to `github.com/sivasoundhar/UniRAG`,
    **private**, clean (no secrets tracked).
  - `D:\projects\medical\PatientShield-AI` (contains `medintel-ui/`, the
    actual "MedIntel" project referenced in the earlier draft) → pushed to
    `github.com/sivasoundhar/PatientShield-AI`, **private**, clean.
  - `D:\projects\medical\MedicalImaging_public` → discovered this already
    exists as `github.com/sivasoundhar/medical-imaging-ai-copilot` with a
    full commit history, professional README, and a `v1.0.0` release —
    **private**, nothing needed pushing.
  - All three repos are complete and just need to be flipped to public.

## Outstanding / not done yet
- LinkedIn badge still has the `YOUR-HANDLE` placeholder.
- UniRAG, PatientShield-AI, and medical-imaging-ai-copilot are still
  **private** — the Featured Projects links in the README will 404 for
  visitors until these go public (user wants to review first).
- Once public: pin the repos on the profile (GitHub's actual pinned-repos
  feature, separate from the README) and add short descriptions/topics to
  each repo.
- GitHub account bio + location fields (Settings → Profile) are still empty
  — separate from the README content.
