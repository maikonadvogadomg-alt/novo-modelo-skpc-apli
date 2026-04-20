# PLANO DO PROJETO: SK-Code-Editor-APK (5)

> Gerado automaticamente pelo SK Code Editor em 20/04/2026, 03:11:22
> **697 arquivo(s)** | **~394.870 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Full-Stack (React + Express)
- **Frontend / Stack principal:** React + Vite, TypeScript, Tailwind CSS, Python
- **Backend / Dados:** Node.js + Express, PostgreSQL, Drizzle ORM
- **Versao:** 1.0.0

**Para rodar o projeto:**
```bash
npm install && npm run dev
```

---

## ESTRUTURA DE ARQUIVOS

```
SK-Code-Editor-APK (5)/
├── .config/
│   └── replit/
│       └── .semgrep/
│           └── semgrep_rules.json
├── .git/
│   ├── hooks/
│   │   ├── applypatch-msg.sample
│   │   ├── commit-msg.sample
│   │   ├── fsmonitor-watchman.sample
│   │   ├── post-update.sample
│   │   ├── pre-applypatch.sample
│   │   ├── pre-commit.sample
│   │   ├── pre-merge-commit.sample
│   │   ├── pre-push.sample
│   │   ├── pre-rebase.sample
│   │   ├── pre-receive.sample
│   │   ├── prepare-commit-msg.sample
│   │   ├── push-to-checkout.sample
│   │   ├── sendemail-validate.sample
│   │   └── update.sample
│   ├── info/
│   │   └── exclude
│   ├── logs/
│   │   ├── refs/
│   │   │   ├── heads/
│   │   │   │   ├── main
│   │   │   │   └── replit-agent
│   │   │   ├── notes/
│   │   │   │   └── commits
│   │   │   └── remotes/
│   │   │       ├── gitsafe-backup/
│   │   │       │   └── main
│   │   │       └── origin/
│   │   │           └── main
│   │   └── HEAD
│   ├── objects/
│   │   ├── 01/
│   │   │   └── 0f933fef4d29556d65cbbc93f332e897a7d836
│   │   ├── 02/
│   │   │   └── 098a71716e3d7afdc932143063317ab98e625c
│   │   ├── 0e/
│   │   │   └── 21917b77641ea6f26d8a74dfef140c9bf43f05
│   │   ├── 14/
│   │   │   └── 515c06f8093d46c9dadba5a5e38342eebb3a41
│   │   ├── 1d/
│   │   │   └── 285d20d62239428f1515f5f44955a64da83633
│   │   ├── 22/
│   │   │   └── 8c7a87b2158cc858eae600280602ea02e6f90b
│   │   ├── 24/
│   │   │   └── 7631141629198a79def36d2294042f06cf0b4e
│   │   ├── 26/
│   │   │   └── fca19e2eff238ffc2e12be5dc2a204bae8e0a2
│   │   ├── 2e/
│   │   │   └── 01f7292b88fcc769024d694fc1dd8e495f596c
│   │   ├── 32/
│   │   │   ├── 732dabf07f528bc24e32fb4b7f0b015f20157d
│   │   │   └── a5e26d270d46b95e93f63a0ec7136b5560f8e2
│   │   ├── 35/
│   │   │   ├── 084c8476ac94669e1f80a8534ed18de568ff68
│   │   │   └── 631eaec75c63d864314099505ee79c2576ff11
│   │   ├── 39/
│   │   │   └── c5f0269ec451e3183151055ed16dd1f9aa9833
│   │   ├── 41/
│   │   │   └── e24d34bf37f6f5ecbdfaf5dcb122605656fef1
│   │   ├── 42/
│   │   │   └── 3ef46bb5f85a04ffbbd5840217881b319d379f
│   │   ├── 43/
│   │   │   └── 2f32b1ed5f25004303af7a53d67cb073489545
│   │   ├── 47/
│   │   │   └── 61cd5f8d26b87a06fc2e709ef15c4269afddfd
│   │   ├── 49/
│   │   │   └── bab97114fbc2a34742c3b7c6258688f0c319ba
│   │   ├── 4b/
│   │   │   └── 94b99fbe4c162976d6742e69c94dd63192fbc8
│   │   ├── 51/
│   │   │   └── 7e9985a4234f707e20ff6aec2ce196991954fc
│   │   ├── 56/
│   │   │   └── ec5bf50fc10cc5dd65957655e07300db785f2c
│   │   ├── 57/
│   │   │   └── 198b63dd5f1d8884ac4bad7c4ed41eea15bb56
│   │   ├── 59/
│   │   │   └── 9920427066c4d18e30ab6d48579baaa730b730
│   │   ├── 5a/
│   │   │   ├── a1184c12db15ed4de1161ada9baa581f3ea952
│   │   │   └── de295b22ce532a150cede219d04c1c5b87c0c5
│   │   ├── 5b/
│   │   │   └── 85f37b666820fc6789e36500a8a25264d284fa
│   │   ├── 5e/
│   │   │   └── 5d7f8c6017bf41f8aab2d4b6dddc436450ef81
│   │   ├── 5f/
│   │   │   └── 8c4511a44324a3bb2e0b68d52381ab682166fe
│   │   ├── 60/
│   │   │   └── 00c948ca3852c784b63580855ddfd24a2fba8e
│   │   ├── 69/
│   │   │   └── 6e0d2b94fbc09e5bf2378678cfe86625c2f15c
│   │   ├── 79/
│   │   │   └── 8dce67e8d5175e2abad3b31cf007b0737f7403
│   │   ├── 7a/
│   │   │   └── 06badc3d5a93db6dbdc1ac0786e9f36027dcd4
│   │   ├── 7e/
│   │   │   └── b8aaa7dcf576558014a1dc8d500a9e6d21c870
│   │   ├── 86/
│   │   │   └── 0358fa1fd66ac26404ada1e9268423984981dc
│   │   ├── 89/
│   │   │   └── 7183c53372503a17fb0321783ec78dcc5b52bd
│   │   ├── 8f/
│   │   │   └── 171f68dc233525d7c8304b4eeaf96283915ead
│   │   ├── 91/
│   │   │   └── 84ee2c2a44a71b7805c33fec085636582e7ad6
│   │   ├── 94/
│   │   │   └── 0375e8218a6553f013e2b76e04cace9eea8d8a
│   │   ├── 98/
│   │   │   └── 0bf1f4dc5aac2ba96d1039b6860b5f114f2a1e
│   │   ├── 9e/
│   │   │   └── 48cdbea6ca8e1e6ab2c6f9d3b3d504519ba8f1
│   │   ├── a3/
│   │   │   └── 23e8b8daf5cdfd7f719c6d77d3a1a60d175408
│   │   ├── a8/
│   │   │   ├── 36626f7be22e6636f493f6f37bfd567fdc871d
│   │   │   └── 49d26fa5350a0447d55a4f8a9a54bcc2f45d40
│   │   ├── ab/
│   │   │   └── 3d5fa8fd7d22f2c900ad376e6cae0c090cc44f
│   │   ├── ad/
│   │   │   └── 48952423c08b6975cc563c69baac60b1024e62
│   │   ├── ae/
│   │   │   └── 5c07564541a2f6f84f1fec8fd5fd205dae3953
│   │   ├── b0/
│   │   │   └── 3e72732c7c1d8a2998df671c552788b7c6d3ec
│   │   ├── b6/
│   │   │   └── af4ac5b2b1e5f54d720e789263f8d2dd5a829f
│   │   ├── bc/
│   │   │   └── 6cce105c59e7cb61a4b46d3cbbfc42939de319
│   │   ├── c7/
│   │   │   └── a0147554e624be84c0ec415bea358965f1f550
│   │   ├── c9/
│   │   │   └── 17b0279e3a7990eaa95c9540d9a0b0cb8dfd08
│   │   ├── ca/
│   │   │   └── b18d2e5d58e5996b29efbb8a7df3730f753cd1
│   │   ├── cc/
│   │   │   └── 6307131a5395c2ba191ae542e984645b9a870e
│   │   ├── d6/
│   │   │   └── 40423b8635f174075473ce6c0fe7ddf3e63b45
│   │   ├── d8/
│   │   │   └── 3468ba8001865edc053aaae09e3067893f77a2
│   │   ├── df/
│   │   │   └── 2e36040de34bd6f71d78ad41119920dd7fd554
│   │   ├── e6/
│   │   │   └── 2b24e41b4988b9f5a88f75b067cadd547c7c86
│   │   ├── eb/
│   │   │   └── 44dc6928d1b538a84a0b5fff6663588c20fcde
│   │   ├── ec/
│   │   │   └── c21a22441bd8496c15b725f5c0692a007076d6
│   │   ├── ee/
│   │   │   └── 154b37543bda3bb146ce702bc78be977629536
│   │   ├── f5/
│   │   │   └── a7f0a80a7d04b7e41a83c7516711775bb31af3
│   │   ├── fe/
│   │   │   └── 11f3e11f23be794a79f703617530784e33940f
│   │   └── pack/
│   │       ├── pack-b039e4dd2d5151432844012a311727745540bc68.idx
│   │       ├── pack-b039e4dd2d5151432844012a311727745540bc68.pack
│   │       └── pack-b039e4dd2d5151432844012a311727745540bc68.rev
│   ├── refs/
│   │   ├── heads/
│   │   │   ├── main
│   │   │   └── replit-agent
│   │   ├── notes/
│   │   │   └── commits
│   │   ├── remotes/
│   │   │   ├── gitsafe-backup/
│   │   │   │   └── main
│   │   │   └── origin/
│   │   │       └── main
│   │   └── replit/
│   │       └── agent-ledger
│   ├── COMMIT_EDITMSG
│   ├── config
│   ├── description
│   ├── FETCH_HEAD
│   ├── HEAD
│   ├── index
│   ├── ORIG_HEAD
│   └── shallow
├── .local/
│   ├── secondary_skills/
│   │   ├── ad-creative/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── ai-recruiter/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── ai-sdr/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── ai-secretary/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── branding-generator/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── competitive-analysis/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── content-machine/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── deep-research/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── design-thinker/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── excel-generator/
│   │   │   ├── .fingerprint
│   │   │   ├── financial-models.md
│   │   │   └── SKILL.md
│   │   ├── file-converter/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── flashcard-generator/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── geo/
│   │   │   ├── references/
│   │   │   │   ├── content-patterns.md
│   │   │   │   ├── platform-notes.md
│   │   │   │   ├── scorecard.md
│   │   │   │   └── technical-checklist.md
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── github-solution-finder/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── infographic-builder/
│   │   │   ├── .fingerprint
│   │   │   ├── antv-syntax.md
│   │   │   ├── react-fallback.md
│   │   │   └── SKILL.md
│   │   ├── insurance-optimizer/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── interview-prep/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── invoice-generator/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── legal-contract/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── meal-planner/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── personal-shopper/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── photo-editor/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── podcast-generator/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── podcast-marketing/
│   │   │   ├── .fingerprint
│   │   │   ├── audio-processing.md
│   │   │   ├── content-atoms.md
│   │   │   ├── content-calendar.md
│   │   │   ├── content-templates.md
│   │   │   ├── quote-cards.md
│   │   │   ├── rss-and-batch.md
│   │   │   ├── SKILL.md
│   │   │   ├── video-clips.md
│   │   │   └── youtube-processing.md
│   │   ├── product-manager/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── programmatic-seo/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── real-estate-analyzer/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── recipe-creator/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── recreate-screenshot/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── resume-maker/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── seo-auditor/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── skill-creator/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── skill-finder/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── stock-analyzer/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── storyboard/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── supplier-research/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── tax-reviewer/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── travel-assistant/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── video-editing/
│   │   │   ├── .fingerprint
│   │   │   ├── dead-space-and-chunking.md
│   │   │   ├── operations.md
│   │   │   ├── SKILL.md
│   │   │   ├── virality-scoring.md
│   │   │   └── voiceover.md
│   │   ├── website-cloning/
│   │   │   ├── .fingerprint
│   │   │   ├── extraction.md
│   │   │   ├── pitfalls.md
│   │   │   └── SKILL.md
│   │   └── LICENSE.txt
│   ├── skills/
│   │   ├── agent-inbox/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── artifacts/
│   │   │   ├── artifacts/
│   │   │   │   ├── automation/
│   │   │   │   │   ├── files/
│   │   │   │   │   │   ├── scripts/
│   │   │   │   │   │   │   ├── build.sh
│   │   │   │   │   │   │   └── inngest.sh
│   │   │   │   │   │   ├── src/
│   │   │   │   │   │   │   ├── mastra/
│   │   │   │   │   │   │   │   ├── agents/
│   │   │   │   │   │   │   │   │   └── agent.ts
│   │   │   │   │   │   │   │   ├── inngest/
│   │   │   │   │   │   │   │   │   ├── client.ts
│   │   │   │   │   │   │   │   │   └── index.ts
│   │   │   │   │   │   │   │   ├── storage/
│   │   │   │   │   │   │   │   │   └── index.ts
│   │   │   │   │   │   │   │   ├── tools/
│   │   │   │   │   │   │   │   │   └── exampleTool.ts
│   │   │   │   │   │   │   │   ├── workflows/
│   │   │   │   │   │   │   │   │   └── workflow.ts
│   │   │   │   │   │   │   │   └── index.ts
│   │   │   │   │   │   │   ├── triggers/
│   │   │   │   │   │   │   │   ├── cronTriggers.ts
│   │   │   │   │   │   │   │   ├── exampleConnectorTrigger.ts
│   │   │   │   │   │   │   │   ├── slackTriggers.ts
│   │   │   │   │   │   │   │   └── telegramTriggers.ts
│   │   │   │   │   │   │   └── global.d.ts
│   │   │   │   │   │   ├── tests/
│   │   │   │   │   │   │   ├── testCronAutomation.ts
│   │   │   │   │   │   │   └── testWebhookAutomation.ts
│   │   │   │   │   │   ├── .gitignore
│   │   │   │   │   │   ├── package.json.template
│   │   │   │   │   │   └── tsconfig.json
│   │   │   │   │   └── artifact.yaml
│   │   │   │   ├── data-visualization/
│   │   │   │   │   └── artifact.yaml
│   │   │   │   ├── expo/
│   │   │   │   │   ├── files/
│   │   │   │   │   │   ├── app/
│   │   │   │   │   │   │   ├── (tabs)/
│   │   │   │   │   │   │   │   ├── _layout.tsx
│   │   │   │   │   │   │   │   └── index.tsx
│   │   │   │   │   │   │   ├── _layout.tsx
│   │   │   │   │   │   │   └── +not-found.tsx
│   │   │   │   │   │   ├── assets/
│   │   │   │   │   │   │   └── images/
│   │   │   │   │   │   │       └── icon.png
│   │   │   │   │   │   ├── components/
│   │   │   │   │   │   │   ├── ErrorBoundary.tsx
│   │   │   │   │   │   │   ├── ErrorFallback.tsx
│   │   │   │   │   │   │   └── KeyboardAwareScrollViewCompat.tsx
│   │   │   │   │   │   ├── constants/
│   │   │   │   │   │   │   └── colors.ts
│   │   │   │   │   │   ├── hooks/
│   │   │   │   │   │   │   └── useColors.ts
│   │   │   │   │   │   ├── scripts/
│   │   │   │   │   │   │   └── build.js
│   │   │   │   │   │   ├── server/
│   │   │   │   │   │   │   ├── templates/
│   │   │   │   │   │   │   │   └── landing-page.html
│   │   │   │   │   │   │   └── serve.js
│   │   │   │   │   │   ├── .gitignore
│   │   │   │   │   │   ├── app.json.template
│   │   │   │   │   │   ├── babel.config.js
│   │   │   │   │   │   ├── metro.config.js
│   │   │   │   │   │   ├── package.json.template
│   │   │   │   │   │   └── tsconfig.json
│   │   │   │   │   ├── artifact.yaml
│   │   │   │   │   └── OWNERS
│   │   │   │   ├── mockup-sandbox/
│   │   │   │   │   ├── files/
│   │   │   │   │   │   ├── public/
│   │   │   │   │   │   │   └── favicon.svg
│   │   │   │   │   │   ├── src/
│   │   │   │   │   │   │   ├── .generated/
│   │   │   │   │   │   │   │   └── mockup-components.ts
│   │   │   │   │   │   │   ├── components/
│   │   │   │   │   │   │   │   └── ui/
│   │   │   │   │   │   │   │       ├── accordion.tsx
│   │   │   │   │   │   │   │       ├── alert-dialog.tsx
│   │   │   │   │   │   │   │       ├── alert.tsx
│   │   │   │   │   │   │   │       ├── aspect-ratio.tsx
│   │   │   │   │   │   │   │       ├── avatar.tsx
│   │   │   │   │   │   │   │       ├── badge.tsx
│   │   │   │   │   │   │   │       ├── breadcrumb.tsx
│   │   │   │   │   │   │   │       ├── button-group.tsx
│   │   │   │   │   │   │   │       ├── button.tsx
│   │   │   │   │   │   │   │       ├── calendar.tsx
│   │   │   │   │   │   │   │       ├── card.tsx
│   │   │   │   │   │   │   │       ├── carousel.tsx
│   │   │   │   │   │   │   │       ├── chart.tsx
│   │   │   │   │   │   │   │       ├── checkbox.tsx
│   │   │   │   │   │   │   │       ├── collapsible.tsx
│   │   │   │   │   │   │   │       ├── command.tsx
│   │   │   │   │   │   │   │       ├── context-menu.tsx
│   │   │   │   │   │   │   │       ├── dialog.tsx
│   │   │   │   │   │   │   │       ├── drawer.tsx
│   │   │   │   │   │   │   │       ├── dropdown-menu.tsx
│   │   │   │   │   │   │   │       ├── empty.tsx
│   │   │   │   │   │   │   │       ├── field.tsx
│   │   │   │   │   │   │   │       ├── form.tsx
│   │   │   │   │   │   │   │       ├── hover-card.tsx
│   │   │   │   │   │   │   │       ├── input-group.tsx
│   │   │   │   │   │   │   │       ├── input-otp.tsx
│   │   │   │   │   │   │   │       ├── input.tsx
│   │   │   │   │   │   │   │       ├── item.tsx
│   │   │   │   │   │   │   │       ├── kbd.tsx
│   │   │   │   │   │   │   │       ├── label.tsx
│   │   │   │   │   │   │   │       ├── menubar.tsx
│   │   │   │   │   │   │   │       ├── navigation-menu.tsx
│   │   │   │   │   │   │   │       ├── pagination.tsx
│   │   │   │   │   │   │   │       ├── popover.tsx
│   │   │   │   │   │   │   │       ├── progress.tsx
│   │   │   │   │   │   │   │       ├── radio-group.tsx
│   │   │   │   │   │   │   │       ├── resizable.tsx
│   │   │   │   │   │   │   │       ├── scroll-area.tsx
│   │   │   │   │   │   │   │       ├── select.tsx
│   │   │   │   │   │   │   │       ├── separator.tsx
│   │   │   │   │   │   │   │       ├── sheet.tsx
│   │   │   │   │   │   │   │       ├── sidebar.tsx
│   │   │   │   │   │   │   │       ├── skeleton.tsx
│   │   │   │   │   │   │   │       ├── slider.tsx
│   │   │   │   │   │   │   │       ├── sonner.tsx
│   │   │   │   │   │   │   │       ├── spinner.tsx
│   │   │   │   │   │   │   │       ├── switch.tsx
│   │   │   │   │   │   │   │       ├── table.tsx
│   │   │   │   │   │   │   │       ├── tabs.tsx
│   │   │   │   │   │   │   │       ├── textarea.tsx
│   │   │   │   │   │   │   │       ├── toast.tsx
│   │   │   │   │   │   │   │       ├── toaster.tsx
│   │   │   │   │   │   │   │       ├── toggle-group.tsx
│   │   │   │   │   │   │   │       ├── toggle.tsx
│   │   │   │   │   │   │   │       └── tooltip.tsx
│   │   │   │   │   │   │   ├── hooks/
│   │   │   │   │   │   │   │   ├── use-mobile.tsx
│   │   │   │   │   │   │   │   └── use-toast.ts
│   │   │   │   │   │   │   ├── lib/
│   │   │   │   │   │   │   │   └── utils.ts
│   │   │   │   │   │   │   ├── App.tsx
│   │   │   │   │   │   │   ├── index.css
│   │   │   │   │   │   │   └── main.tsx
│   │   │   │   │   │   ├── components.json
│   │   │   │   │   │   ├── index.html
│   │   │   │   │   │   ├── mockupPreviewPlugin.ts
│   │   │   │   │   │   ├── package.json.template
│   │   │   │   │   │   ├── tsconfig.json
│   │   │   │   │   │   └── vite.config.ts
│   │   │   │   │   └── artifact.yaml
│   │   │   │   ├── react-vite/
│   │   │   │   │   ├── files/
│   │   │   │   │   │   ├── public/
│   │   │   │   │   │   │   └── favicon.svg
│   │   │   │   │   │   ├── src/
│   │   │   │   │   │   │   ├── components/
│   │   │   │   │   │   │   │   └── ui/
│   │   │   │   │   │   │   │       ├── accordion.tsx
│   │   │   │   │   │   │   │       ├── alert-dialog.tsx
│   │   │   │   │   │   │   │       ├── alert.tsx
│   │   │   │   │   │   │   │       ├── aspect-ratio.tsx
│   │   │   │   │   │   │   │       ├── avatar.tsx
│   │   │   │   │   │   │   │       ├── badge.tsx
│   │   │   │   │   │   │   │       ├── breadcrumb.tsx
│   │   │   │   │   │   │   │       ├── button-group.tsx
│   │   │   │   │   │   │   │       ├── button.tsx
│   │   │   │   │   │   │   │       ├── calendar.tsx
│   │   │   │   │   │   │   │       ├── card.tsx
│   │   │   │   │   │   │   │       ├── carousel.tsx
│   │   │   │   │   │   │   │       ├── chart.tsx
│   │   │   │   │   │   │   │       ├── checkbox.tsx
│   │   │   │   │   │   │   │       ├── collapsible.tsx
│   │   │   │   │   │   │   │       ├── command.tsx
│   │   │   │   │   │   │   │       ├── context-menu.tsx
│   │   │   │   │   │   │   │       ├── dialog.tsx
│   │   │   │   │   │   │   │       ├── drawer.tsx
│   │   │   │   │   │   │   │       ├── dropdown-menu.tsx
│   │   │   │   │   │   │   │       ├── empty.tsx
│   │   │   │   │   │   │   │       ├── field.tsx
│   │   │   │   │   │   │   │       ├── form.tsx
│   │   │   │   │   │   │   │       ├── hover-card.tsx
│   │   │   │   │   │   │   │       ├── input-group.tsx
│   │   │   │   │   │   │   │       ├── input-otp.tsx
│   │   │   │   │   │   │   │       ├── input.tsx
│   │   │   │   │   │   │   │       ├── item.tsx
│   │   │   │   │   │   │   │       ├── kbd.tsx
│   │   │   │   │   │   │   │       ├── label.tsx
│   │   │   │   │   │   │   │       ├── menubar.tsx
│   │   │   │   │   │   │   │       ├── navigation-menu.tsx
│   │   │   │   │   │   │   │       ├── pagination.tsx
│   │   │   │   │   │   │   │       ├── popover.tsx
│   │   │   │   │   │   │   │       ├── progress.tsx
│   │   │   │   │   │   │   │       ├── radio-group.tsx
│   │   │   │   │   │   │   │       ├── resizable.tsx
│   │   │   │   │   │   │   │       ├── scroll-area.tsx
│   │   │   │   │   │   │   │       ├── select.tsx
│   │   │   │   │   │   │   │       ├── separator.tsx
│   │   │   │   │   │   │   │       ├── sheet.tsx
│   │   │   │   │   │   │   │       ├── sidebar.tsx
│   │   │   │   │   │   │   │       ├── skeleton.tsx
│   │   │   │   │   │   │   │       ├── slider.tsx
│   │   │   │   │   │   │   │       ├── sonner.tsx
│   │   │   │   │   │   │   │       ├── spinner.tsx
│   │   │   │   │   │   │   │       ├── switch.tsx
│   │   │   │   │   │   │   │       ├── table.tsx
│   │   │   │   │   │   │   │       ├── tabs.tsx
│   │   │   │   │   │   │   │       ├── textarea.tsx
│   │   │   │   │   │   │   │       ├── toast.tsx
│   │   │   │   │   │   │   │       ├── toaster.tsx
│   │   │   │   │   │   │   │       ├── toggle-group.tsx
│   │   │   │   │   │   │   │       ├── toggle.tsx
│   │   │   │   │   │   │   │       └── tooltip.tsx
│   │   │   │   │   │   │   ├── hooks/
│   │   │   │   │   │   │   │   ├── use-mobile.tsx
│   │   │   │   │   │   │   │   └── use-toast.ts
│   │   │   │   │   │   │   ├── lib/
│   │   │   │   │   │   │   │   └── utils.ts
│   │   │   │   │   │   │   ├── pages/
│   │   │   │   │   │   │   │   └── not-found.tsx
│   │   │   │   │   │   │   ├── App.tsx
│   │   │   │   │   │   │   ├── index.css
│   │   │   │   │   │   │   └── main.tsx
│   │   │   │   │   │   ├── components.json
│   │   │   │   │   │   ├── index.html.template
│   │   │   │   │   │   ├── package.json.template
│   │   │   │   │   │   ├── tsconfig.json
│   │   │   │   │   │   └── vite.config.ts
│   │   │   │   │   └── artifact.yaml
│   │   │   │   ├── slides/
│   │   │   │   │   ├── files/
│   │   │   │   │   │   ├── public/
│   │   │   │   │   │   │   └── favicon.svg
│   │   │   │   │   │   ├── scripts/
│   │   │   │   │   │   │   └── validate-slides.ts
│   │   │   │   │   │   ├── src/
│   │   │   │   │   │   │   ├── data/
│   │   │   │   │   │   │   │   ├── slides-manifest.json
│   │   │   │   │   │   │   │   └── slidesManifestSchema.ts
│   │   │   │   │   │   │   ├── App.tsx
│   │   │   │   │   │   │   ├── index.css
│   │   │   │   │   │   │   ├── main.tsx
│   │   │   │   │   │   │   └── slideLoader.ts
│   │   │   │   │   │   ├── index.html.template
│   │   │   │   │   │   ├── package.json.template
│   │   │   │   │   │   ├── tsconfig.json
│   │   │   │   │   │   └── vite.config.ts
│   │   │   │   │   └── artifact.yaml
│   │   │   │   └── video-js/
│   │   │   │       ├── files/
│   │   │   │       │   ├── public/
│   │   │   │       │   │   └── favicon.svg
│   │   │   │       │   ├── scripts/
│   │   │   │       │   │   └── validate-recording.sh
│   │   │   │       │   ├── src/
│   │   │   │       │   │   ├── components/
│   │   │   │       │   │   │   └── video/
│   │   │   │       │   │   │       ├── index.ts
│   │   │   │       │   │   │       ├── ReplitLoadingScene.tsx
│   │   │   │       │   │   │       └── VideoTemplate.tsx
│   │   │   │       │   │   ├── hooks/
│   │   │   │       │   │   │   └── use-mobile.tsx
│   │   │   │       │   │   ├── lib/
│   │   │   │       │   │   │   ├── video/
│   │   │   │       │   │   │   │   ├── animations.ts
│   │   │   │       │   │   │   │   ├── hooks.ts
│   │   │   │       │   │   │   │   └── index.ts
│   │   │   │       │   │   │   └── utils.ts
│   │   │   │       │   │   ├── App.tsx
│   │   │   │       │   │   ├── index.css
│   │   │   │       │   │   └── main.tsx
│   │   │   │       │   ├── index.html.template
│   │   │   │       │   ├── package.json.template
│   │   │   │       │   ├── tsconfig.json
│   │   │   │       │   └── vite.config.ts
│   │   │   │       └── artifact.yaml
│   │   │   ├── references/
│   │   │   │   └── multi-artifact-creation.md
│   │   │   ├── .fingerprint
│   │   │   ├── bootstrap-legacy.js
│   │   │   ├── bootstrap.js
│   │   │   └── SKILL.md
│   │   ├── canvas/
│   │   │   ├── __init__.py
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── code_review/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── database/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── delegation/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── deployment/
│   │   │   ├── references/
│   │   │   │   └── deployment-logs.md
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── design/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── design-exploration/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── diagnostics/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── environment-secrets/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── external_apis/
│   │   │   ├── references/
│   │   │   │   └── brave.md
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── follow-up-tasks/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── fullstack-js/
│   │   │   ├── references/
│   │   │   │   ├── hover_and_elevation.md
│   │   │   │   ├── layout_and_spacing.md
│   │   │   │   ├── shadcn_component_rules.md
│   │   │   │   ├── sidebar_rules.md
│   │   │   │   └── visual_style_and_contrast.md
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── integrations/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── media-generation/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── mockup-extract/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── mockup-graduate/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── mockup-sandbox/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── package-management/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── post_merge_setup/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── project_tasks/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── query-integration-data/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── remove-image-background/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── repl_setup/
│   │   │   ├── references/
│   │   │   │   ├── angular.md
│   │   │   │   ├── react_vite.md
│   │   │   │   └── vue.md
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── replit-docs/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── revenuecat/
│   │   │   ├── references/
│   │   │   │   ├── initial-setup.md
│   │   │   │   ├── replit-revenuecat-sdk-docs.md
│   │   │   │   └── subsequent-management.md
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── security_scan/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── skill-authoring/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── stripe/
│   │   │   ├── references/
│   │   │   │   └── code-templates.md
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── suggest-new-project/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── threat_modeling/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── validation/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── web-search/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   ├── workflows/
│   │   │   ├── .fingerprint
│   │   │   └── SKILL.md
│   │   └── LICENSE.txt
│   └── state/
│       ├── replit/
│       │   ├── agent/
│       │   │   ├── .agent_state_010f933fef4d29556d65cbbc93f332e897a7d836.bin
│       │   │   ├── .agent_state_14515c06f8093d46c9dadba5a5e38342eebb3a41.bin
│       │   │   ├── .agent_state_228c7a87b2158cc858eae600280602ea02e6f90b.bin
│       │   │   ├── .agent_state_432f32b1ed5f25004303af7a53d67cb073489545.bin
│       │   │   ├── .agent_state_5b85f37b666820fc6789e36500a8a25264d284fa.bin
│       │   │   ├── .agent_state_6000c948ca3852c784b63580855ddfd24a2fba8e.bin
│       │   │   ├── .agent_state_980bf1f4dc5aac2ba96d1039b6860b5f114f2a1e.bin
│       │   │   ├── .agent_state_ae5c07564541a2f6f84f1fec8fd5fd205dae3953.bin
│       │   │   ├── .agent_state_b03e72732c7c1d8a2998df671c552788b7c6d3ec.bin
│       │   │   ├── .agent_state_cc6307131a5395c2ba191ae542e984645b9a870e.bin
│       │   │   ├── .agent_state_f5a7f0a80a7d04b7e41a83c7516711775bb31af3.bin
│       │   │   ├── .agent_state_main.bin
│       │   │   ├── .latest.json
│       │   │   ├── progress_tracker.md
│       │   │   └── repl_state.bin
│       │   ├── log-query.db
│       │   ├── log-query.db-shm
│       │   └── log-query.db-wal
│       ├── scribe/
│       │   ├── scribe.db
│       │   ├── scribe.db-shm
│       │   └── scribe.db-wal
│       └── workflow-logs/
│           ├── 55Gr7v8DXu5ewWUWfs4Lq/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── 5cDC29B7tJw5XXbBOrhWh/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── E1ZL-IAPLGApOqirZ4sJY/
│           │   └── metadata.json
│           ├── GtNudELQEcgARdYMZXL2U/
│           │   └── metadata.json
│           ├── HPbCVcItFOa3mfeJFK8kf/
│           │   └── metadata.json
│           ├── hWQEAm0pGU0QvTGg2KeoI/
│           │   └── metadata.json
│           ├── Ij6htOPNrryT22iN66-TE/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── Jg0_YczQpCvNyu5SPmfpI/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── Kr4Rl61IQpvtOMDRHcc0d/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── LbZi5kZQB7Ym_CrpUVI_H/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── LN8Ypo2mUdcuyqFhIh6Fl/
│           │   └── metadata.json
│           ├── naLrCNUov5fD0PtVxdPdU/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── pITQDUoOlG2F1v9qoRwHb/
│           │   └── metadata.json
│           ├── Pw0Qq6gHq3cQ4SWSW6oQB/
│           │   └── metadata.json
│           ├── SQjKh0Fh_-kO7G-0Vi5bG/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── tljoQIkZd--W9BtSbS0aX/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── Ujr1I1TrA5ofTdJDo9VZP/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           ├── x7K8OcA4UDDBilTnmKtwZ/
│           │   └── metadata.json
│           ├── X8A4VPXQihbRxTi8hznz4/
│           │   ├── metadata.json
│           │   └── start_application.shell.exec.0
│           └── zMCgmyyArMsumYNVrbt1S/
│               └── metadata.json
├── api/
│   └── index.ts
├── client/
│   ├── public/
│   │   ├── auditoria.html
│   │   ├── codigo-formatacao.txt
│   │   ├── comparador.html
│   │   ├── favicon.png
│   │   ├── icon-192.png
│   │   ├── icon-512.png
│   │   ├── manifest.json
│   │   └── sw.js
│   ├── replit_integrations/
│   │   └── audio/
│   │       ├── audio-playback-worklet.js
│   │       ├── audio-utils.ts
│   │       ├── index.ts
│   │       ├── useAudioPlayback.ts
│   │       ├── useVoiceRecorder.ts
│   │       └── useVoiceStream.ts
│   ├── src/
│   │   ├── components/
│   │   │   ├── ui/
│   │   │   │   ├── accordion.tsx
│   │   │   │   ├── alert-dialog.tsx
│   │   │   │   ├── alert.tsx
│   │   │   │   ├── aspect-ratio.tsx
│   │   │   │   ├── avatar.tsx
│   │   │   │   ├── badge.tsx
│   │   │   │   ├── breadcrumb.tsx
│   │   │   │   ├── button.tsx
│   │   │   │   ├── calendar.tsx
│   │   │   │   ├── card.tsx
│   │   │   │   ├── carousel.tsx
│   │   │   │   ├── chart.tsx
│   │   │   │   ├── checkbox.tsx
│   │   │   │   ├── collapsible.tsx
│   │   │   │   ├── command.tsx
│   │   │   │   ├── context-menu.tsx
│   │   │   │   ├── dialog.tsx
│   │   │   │   ├── drawer.tsx
│   │   │   │   ├── dropdown-menu.tsx
│   │   │   │   ├── form.tsx
│   │   │   │   ├── hover-card.tsx
│   │   │   │   ├── input-otp.tsx
│   │   │   │   ├── input.tsx
│   │   │   │   ├── label.tsx
│   │   │   │   ├── menubar.tsx
│   │   │   │   ├── navigation-menu.tsx
│   │   │   │   ├── pagination.tsx
│   │   │   │   ├── popover.tsx
│   │   │   │   ├── progress.tsx
│   │   │   │   ├── radio-group.tsx
│   │   │   │   ├── resizable.tsx
│   │   │   │   ├── scroll-area.tsx
│   │   │   │   ├── select.tsx
│   │   │   │   ├── separator.tsx
│   │   │   │   ├── sheet.tsx
│   │   │   │   ├── sidebar.tsx
│   │   │   │   ├── skeleton.tsx
│   │   │   │   ├── slider.tsx
│   │   │   │   ├── switch.tsx
│   │   │   │   ├── table.tsx
│   │   │   │   ├── tabs.tsx
│   │   │   │   ├── textarea.tsx
│   │   │   │   ├── toast.tsx
│   │   │   │   ├── toaster.tsx
│   │   │   │   ├── toggle-group.tsx
│   │   │   │   ├── toggle.tsx
│   │   │   │   └── tooltip.tsx
│   │   │   ├── pwa-install.tsx
│   │   │   ├── theme-provider.tsx
│   │   │   ├── theme-toggle.tsx
│   │   │   └── tiptap-editor.tsx
│   │   ├── hooks/
│   │   │   ├── use-mobile.tsx
│   │   │   └── use-toast.ts
│   │   ├── lib/
│   │   │   ├── queryClient.ts
│   │   │   └── utils.ts
│   │   ├── pages/
│   │   │   ├── auditoria-financeira.tsx
│   │   │   ├── code-assistant.tsx
│   │   │   ├── comparador-juridico.tsx
│   │   │   ├── comunicacoes-cnj.tsx
│   │   │   ├── consulta-corporativo.tsx
│   │   │   ├── consulta-pdpj.tsx
│   │   │   ├── consulta-processual.tsx
│   │   │   ├── filtrador.tsx
│   │   │   ├── jurisprudencia.tsx
│   │   │   ├── legal-assistant.tsx
│   │   │   ├── legal-assistant.tsx.recovered
│   │   │   ├── login.tsx
│   │   │   ├── not-found.tsx
│   │   │   ├── painel-processos.tsx
│   │   │   ├── playground.tsx
│   │   │   ├── previdenciario.tsx
│   │   │   ├── robo-djen.tsx
│   │   │   ├── token-generator.tsx
│   │   │   └── tramitacao.tsx
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   └── index.html
├── migrations/
│   ├── meta/
│   │   ├── _journal.json
│   │   └── 0000_snapshot.json
│   └── 0000_init.sql
├── public/
│   └── auditoria.html
├── script/
│   └── build.ts
├── server/
│   ├── replit_integrations/
│   │   ├── audio/
│   │   │   ├── client.ts
│   │   │   ├── index.ts
│   │   │   └── routes.ts
│   │   ├── batch/
│   │   │   ├── index.ts
│   │   │   └── utils.ts
│   │   ├── chat/
│   │   │   ├── index.ts
│   │   │   ├── routes.ts
│   │   │   └── storage.ts
│   │   └── image/
│   │       ├── client.ts
│   │       ├── index.ts
│   │       └── routes.ts
│   ├── db.ts
│   ├── djen.ts
│   ├── index.ts
│   ├── routes.ts
│   ├── static.ts
│   ├── storage.ts
│   └── vite.ts
├── shared/
│   ├── models/
│   │   └── chat.ts
│   └── schema.ts
├── .gitignore
├── .replit
├── components.json
├── drizzle.config.ts
├── fix_buttons.txt
├── main.py
├── MANUAL_APK_ANDROID.md
├── MANUAL_APK_ORIENTADO.md
├── novo 1.zip
├── package-lock.json
├── package.json
├── PLANO.md
├── postcss.config.js
├── pyproject.toml
├── README.md
├── RELATORIO_CORRECOES.md
├── replit.md
├── SECURITY.md
├── tailwind.config.ts
├── tsconfig.json
├── uv.lock
└── vite.config.ts
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React + Vite, TypeScript, Tailwind CSS, Python
- **Backend:** Node.js + Express, PostgreSQL, Drizzle ORM
- **Todos os pacotes (116):** @google/genai, @hookform/resolvers, @jridgewell/trace-mapping, @radix-ui/react-accordion, @radix-ui/react-alert-dialog, @radix-ui/react-aspect-ratio, @radix-ui/react-avatar, @radix-ui/react-checkbox, @radix-ui/react-collapsible, @radix-ui/react-context-menu, @radix-ui/react-dialog, @radix-ui/react-dropdown-menu, @radix-ui/react-hover-card, @radix-ui/react-label, @radix-ui/react-menubar, @radix-ui/react-navigation-menu, @radix-ui/react-popover, @radix-ui/react-progress, @radix-ui/react-radio-group, @radix-ui/react-scroll-area, @radix-ui/react-select, @radix-ui/react-separator, @radix-ui/react-slider, @radix-ui/react-slot, @radix-ui/react-switch, @radix-ui/react-tabs, @radix-ui/react-toast, @radix-ui/react-toggle, @radix-ui/react-toggle-group, @radix-ui/react-tooltip, @tanstack/react-query, @tiptap/extension-color, @tiptap/extension-font-family, @tiptap/extension-highlight, @tiptap/extension-link, @tiptap/extension-table, @tiptap/extension-table-cell, @tiptap/extension-table-header, @tiptap/extension-table-row, @tiptap/extension-text-align, @tiptap/extension-text-style, @tiptap/extension-underline, @tiptap/pm, @tiptap/react, @tiptap/starter-kit, @types/jsonwebtoken, @types/multer, adm-zip, axios, class-variance-authority, clsx, cmdk, connect-pg-simple, date-fns, docx, drizzle-orm, drizzle-zod, embla-carousel-react, express, express-session, framer-motion, html-entities, input-otp, jsonwebtoken, lucide-react, mammoth, memorystore, multer, next-themes, openai, p-limit, p-retry, passport, passport-local, pdf-parse, pdfjs-dist, pg, postcss-selector-parser, react, react-day-picker, react-dom, react-hook-form, react-icons, react-resizable-panels, recharts, tailwind-merge, tailwindcss-animate, tw-animate-css, vaul, wouter, ws, zod, zod-validation-error, @replit/vite-plugin-cartographer, @replit/vite-plugin-dev-banner, @replit/vite-plugin-runtime-error-modal, @tailwindcss/typography, @tailwindcss/vite, @types/connect-pg-simple, @types/express, @types/express-session, @types/node, @types/passport, @types/passport-local, @types/react, @types/react-dom, @types/ws, @vitejs/plugin-react, autoprefixer, drizzle-kit, esbuild, postcss, tailwindcss, tsx, typescript, vite

---

## ROTAS DA API (endpoints detectados automaticamente)

```
GET    /api/conversations  (em server/replit_integrations/audio/routes.ts)
GET    /api/conversations/:id  (em server/replit_integrations/audio/routes.ts)
POST   /api/conversations  (em server/replit_integrations/audio/routes.ts)
DELETE /api/conversations/:id  (em server/replit_integrations/audio/routes.ts)
POST   /api/conversations/:id/messages  (em server/replit_integrations/audio/routes.ts)
GET    /api/conversations  (em server/replit_integrations/chat/routes.ts)
GET    /api/conversations/:id  (em server/replit_integrations/chat/routes.ts)
POST   /api/conversations  (em server/replit_integrations/chat/routes.ts)
DELETE /api/conversations/:id  (em server/replit_integrations/chat/routes.ts)
POST   /api/conversations/:id/messages  (em server/replit_integrations/chat/routes.ts)
POST   /api/generate-image  (em server/replit_integrations/image/routes.ts)
GET    /sw.js  (em server/routes.ts)
GET    /api/auth/check  (em server/routes.ts)
POST   /api/auth/login  (em server/routes.ts)
POST   /api/auth/logout  (em server/routes.ts)
GET    /parecer/:id  (em server/routes.ts)
GET    /api/tjmg/fatores  (em server/routes.ts)
POST   /api/pdpj/test-connection  (em server/routes.ts)
GET    /api/pdpj/status  (em server/routes.ts)
POST   /api/pdpj/comunicacoes  (em server/routes.ts)
POST   /api/pdpj/representados  (em server/routes.ts)
POST   /api/pdpj/habilitacao  (em server/routes.ts)
POST   /api/pdpj/pessoa  (em server/routes.ts)
POST   /api/webhooks/tramitacao  (em server/routes.ts)
GET    /api/demo-key-status  (em server/routes.ts)
GET    /api/demo-key-config  (em server/routes.ts)
POST   /api/demo-key-config  (em server/routes.ts)
GET    /api/perplexity-key-status  (em server/routes.ts)
POST   /api/demo-key-test  (em server/routes.ts)
POST   /api/tts  (em server/routes.ts)
POST   /api/voice-chat  (em server/routes.ts)
USE    /api  (em server/routes.ts)
POST   /api/share/parecer  (em server/routes.ts)
GET    /api/snippets  (em server/routes.ts)
GET    /api/snippets/:id  (em server/routes.ts)
POST   /api/snippets  (em server/routes.ts)
PATCH  /api/snippets/:id  (em server/routes.ts)
DELETE /api/snippets/:id  (em server/routes.ts)
GET    /api/custom-actions  (em server/routes.ts)
POST   /api/custom-actions  (em server/routes.ts)
PATCH  /api/custom-actions/:id  (em server/routes.ts)
DELETE /api/custom-actions/:id  (em server/routes.ts)
GET    /api/ementas  (em server/routes.ts)
POST   /api/ementas  (em server/routes.ts)
PATCH  /api/ementas/:id  (em server/routes.ts)
DELETE /api/ementas/:id  (em server/routes.ts)
POST   /api/jurisprudencia/buscar  (em server/routes.ts)
GET    /api/ai-history  (em server/routes.ts)
POST   /api/ai-history  (em server/routes.ts)
DELETE /api/ai-history/:id  (em server/routes.ts)
DELETE /api/ai-history  (em server/routes.ts)
GET    /api/ai-usage-summary  (em server/routes.ts)
POST   /api/ai-usage-credit  (em server/routes.ts)
GET    /api/prompt-templates  (em server/routes.ts)
POST   /api/prompt-templates  (em server/routes.ts)
PATCH  /api/prompt-templates/:id  (em server/routes.ts)
DELETE /api/prompt-templates/:id  (em server/routes.ts)
GET    /api/doc-templates  (em server/routes.ts)
POST   /api/doc-templates  (em server/routes.ts)
PATCH  /api/doc-templates/:id  (em server/routes.ts)
DELETE /api/doc-templates/:id  (em server/routes.ts)
POST   /api/doc-templates/upload-docx  (em server/routes.ts)
POST   /api/export/word-with-template  (em server/routes.ts)
POST   /api/import/url  (em server/routes.ts)
POST   /api/upload/extract-text  (em server/routes.ts)
POST   /api/upload/transcribe  (em server/routes.ts)
POST   /api/ai/process  (em server/routes.ts)
POST   /api/ai/refine  (em server/routes.ts)
POST   /api/export/word  (em server/routes.ts)
POST   /api/jwt/generate  (em server/routes.ts)
GET    /api/jwt/status  (em server/routes.ts)
GET    /api/processos  (em server/routes.ts)
GET    /api/processos/:id  (em server/routes.ts)
POST   /api/processos  (em server/routes.ts)
PATCH  /api/processos/:id  (em server/routes.ts)
DELETE /api/processos/:id  (em server/routes.ts)
POST   /api/datajud/consulta  (em server/routes.ts)
POST   /api/datajud/consulta-oab  (em server/routes.ts)
GET    /api/corporativo/advogado/cpf/:cpf  (em server/routes.ts)
GET    /api/corporativo/advogado/oab/:uf/:inscricao  (em server/routes.ts)
GET    /api/corporativo/magistrados/:tribunal  (em server/routes.ts)
GET    /api/pdpj/status  (em server/routes.ts)
POST   /api/pdpj/test-connection  (em server/routes.ts)
POST   /api/pdpj/comunicacoes  (em server/routes.ts)
POST   /api/pdpj/representados  (em server/routes.ts)
POST   /api/pdpj/habilitacao  (em server/routes.ts)
POST   /api/pdpj/pessoa  (em server/routes.ts)
GET    /api/datajud/tribunais  (em server/routes.ts)
POST   /api/cnj/comunicacoes  (em server/routes.ts)
GET    /api/cnj/comunicacoes/certidao/:hash  (em server/routes.ts)
GET    /api/settings/:key  (em server/routes.ts)
PUT    /api/settings/:key  (em server/routes.ts)
GET    /api/tramitacao/clientes  (em server/routes.ts)
POST   /api/tramitacao/clientes  (em server/routes.ts)
GET    /api/tramitacao/clientes/:id  (em server/routes.ts)
PATCH  /api/tramitacao/clientes/:id  (em server/routes.ts)
GET    /api/tramitacao/notas  (em server/routes.ts)
POST   /api/tramitacao/notas  (em server/routes.ts)
DELETE /api/tramitacao/notas/:id  (em server/routes.ts)
GET    /api/tramitacao/usuarios  (em server/routes.ts)
GET    /api/tramitacao/test  (em server/routes.ts)
GET    /api/tramitacao/publicacoes  (em server/routes.ts)
POST   /api/tramitacao/sync-publicacoes  (em server/routes.ts)
PATCH  /api/tramitacao/publicacoes/:id/lida  (em server/routes.ts)
POST   /api/code/run  (em server/routes.ts)
POST   /api/previdenciario/extrair  (em server/routes.ts)
GET    /api/pesquisa/oab  (em server/routes.ts)
GET    /api/pesquisa/processo  (em server/routes.ts)
GET    /api/djen/config  (em server/routes.ts)
PUT    /api/djen/config  (em server/routes.ts)
GET    /api/djen/clientes  (em server/routes.ts)
POST   /api/djen/clientes  (em server/routes.ts)
DELETE /api/djen/clientes/:id  (em server/routes.ts)
GET    /api/djen/publicacoes  (em server/routes.ts)
GET    /api/djen/execucoes  (em server/routes.ts)
POST   /api/djen/executar  (em server/routes.ts)
POST   /api/djen/gerar-token  (em server/routes.ts)
POST   /api/code-assistant  (em server/routes.ts)
POST   /api/git-push  (em server/routes.ts)
USE    /sw.js  (em server/static.ts)
USE    /manifest.json  (em server/static.ts)
USE    /{*path}  (em server/static.ts)
USE    /{*path}  (em server/vite.ts)
```

---

## SCRIPTS DISPONIVEIS (package.json)

```bash
npm run dev           # NODE_ENV=development tsx server/index.ts
npm run build         # tsx script/build.ts
npm run start         # NODE_ENV=production node dist/index.cjs
npm run check         # tsc
npm run db:push       # drizzle-kit push
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
AI_INTEGRATIONS_OPENAI_BASE_URL=seu_valor_aqui
AI_INTEGRATIONS_OPENAI_API_KEY=seu_valor_aqui
OPENAI_BASE_URL=seu_valor_aqui
OPENAI_API_KEY=seu_valor_aqui
PORT=seu_valor_aqui
INNGEST_PORT=seu_valor_aqui
BASE_PATH=seu_valor_aqui
REPLIT_DOMAINS=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
REPLIT_CONNECTORS_HOSTNAME=seu_valor_aqui
TELEGRAM_BOT_TOKEN=seu_valor_aqui
REPLIT_INTERNAL_APP_DOMAIN=seu_valor_aqui
REPLIT_DEV_DOMAIN=seu_valor_aqui
EXPO_PUBLIC_DOMAIN=seu_valor_aqui
REPL_ID=seu_valor_aqui
EXPO_PUBLIC_REPL_ID=seu_valor_aqui
SESSION_SECRET=seu_valor_aqui
PUBLIC_API_KEY=seu_valor_aqui
APP_PASSWORD=seu_valor_aqui
AI_INTEGRATIONS_GEMINI_API_KEY=seu_valor_aqui
AI_INTEGRATIONS_GEMINI_BASE_URL=seu_valor_aqui
PDPJ_PEM_PRIVATE_KEY=seu_valor_aqui
PUBLIC_API_MODEL=seu_valor_aqui
PUBLIC_API_URL=seu_valor_aqui
DATAJUD_API_KEY=seu_valor_aqui
PERPLEXITY_API_KEY=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `.local/skills/artifacts/artifacts/automation/files/src/mastra/index.ts` — Arquivo principal
- `.local/skills/artifacts/artifacts/automation/files/src/mastra/inngest/index.ts` — Arquivo principal
- `.local/skills/artifacts/artifacts/automation/files/src/mastra/storage/index.ts` — Arquivo principal
- `.local/skills/artifacts/artifacts/expo/files/app/(tabs)/index.tsx` — Arquivo principal
- `.local/skills/artifacts/artifacts/mockup-sandbox/files/index.html` — Arquivo principal
- `.local/skills/artifacts/artifacts/mockup-sandbox/files/src/App.tsx` — Componente raiz do frontend
- `.local/skills/artifacts/artifacts/mockup-sandbox/files/src/main.tsx` — Arquivo principal
- `.local/skills/artifacts/artifacts/react-vite/files/src/App.tsx` — Componente raiz do frontend
- `.local/skills/artifacts/artifacts/react-vite/files/src/main.tsx` — Arquivo principal
- `.local/skills/artifacts/artifacts/slides/files/src/App.tsx` — Componente raiz do frontend

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`.gitignore`** _(6 linhas)_
Lista de arquivos/pastas que o Git deve IGNORAR (nao versionar). Ex: node_modules, .env

**`.replit`** _(59 linhas)_
Arquivo REPLIT — parte do projeto.

**`MANUAL_APK_ANDROID.md`** _(391 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`MANUAL_APK_ORIENTADO.md`** _(774 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`PLANO.md`** _(5301 linhas)_
Este documento! Gerado automaticamente pelo SK Code Editor com toda a estrutura do projeto.

**`README.md`** _(3 linhas)_
Documentacao principal do projeto. Explica o que o projeto faz e como rodar.

**`RELATORIO_CORRECOES.md`** _(142 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`SECURITY.md`** _(22 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`components.json`** _(20 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`drizzle.config.ts`** _(15 linhas)_
Configuracao do Drizzle ORM — gerencia a conexao e migracao do banco de dados.

**`fix_buttons.txt`** _(64 linhas)_
Arquivo TXT — parte do projeto.

**`main.py`** _(7 linhas)_
Arquivo Python — codigo de logica ou script de automacao.

**`novo 1.zip`** _(9561 linhas)_
Arquivo ZIP — parte do projeto.

**`package-lock.json`** _(11813 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`package.json`** _(142 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`postcss.config.js`** _(7 linhas)_
Configuracao do PostCSS, necessaria para o Tailwind processar os estilos.

**`pyproject.toml`** _(9 linhas)_
Arquivo TOML — parte do projeto.

**`replit.md`** _(141 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`tailwind.config.ts`** _(108 linhas)_
Configuracao do Tailwind CSS — a biblioteca de estilos visuais usada no projeto.

**`tsconfig.json`** _(24 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`uv.lock`** _(630 linhas)_
Arquivo LOCK — parte do projeto.

**`vite.config.ts`** _(39 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `.git/`
> Pasta '.git' — agrupamento de arquivos relacionados.

**`COMMIT_EDITMSG`** _(10 linhas)_
Arquivo COMMIT_EDITMSG — parte do projeto.

**`FETCH_HEAD`** _(2 linhas)_
Arquivo FETCH_HEAD — parte do projeto.

**`HEAD`** _(2 linhas)_
Arquivo HEAD — parte do projeto.

**`ORIG_HEAD`** _(2 linhas)_
Arquivo ORIG_HEAD — parte do projeto.

**`config`** _(19 linhas)_
Arquivo CONFIG — parte do projeto.

**`description`** _(2 linhas)_
Arquivo DESCRIPTION — parte do projeto.

**`index`** _(46 linhas)_
Arquivo INDEX — parte do projeto.

**`shallow`** _(2 linhas)_
Arquivo SHALLOW — parte do projeto.

---

### 📁 `api/`
> Comunicacao com servidor, banco de dados ou APIs externas.

**`index.ts`** _(47 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `client/`
> Pasta 'client' — agrupamento de arquivos relacionados.

**`index.html`** _(18 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

---

### 📁 `migrations/`
> Historico de alteracoes do banco de dados.

**`0000_init.sql`** _(141 linhas)_
Script SQL — contem comandos para criar tabelas, inserir ou consultar dados no banco.

---

### 📁 `public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`auditoria.html`** _(35 linhas)_
Arquivo HTML — parte do projeto.

---

### 📁 `script/`
> Pasta 'script' — agrupamento de arquivos relacionados.

**`build.ts`** _(71 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `server/`
> Pasta 'server' — agrupamento de arquivos relacionados.

**`db.ts`** _(2 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`djen.ts`** _(384 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(179 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`routes.ts`** _(5789 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

**`static.ts`** _(30 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`storage.ts`** _(280 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`vite.ts`** _(56 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `shared/`
> Pasta 'shared' — agrupamento de arquivos relacionados.

**`schema.ts`** _(267 linhas)_
Arquivo de MODELO — define a estrutura dos dados (tabelas, campos, tipos).

---

### 📁 `.git/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`applypatch-msg.sample`** _(16 linhas)_
Arquivo SAMPLE — parte do projeto.

**`commit-msg.sample`** _(25 linhas)_
Arquivo SAMPLE — parte do projeto.

**`fsmonitor-watchman.sample`** _(175 linhas)_
Arquivo SAMPLE — parte do projeto.

**`post-update.sample`** _(9 linhas)_
Arquivo SAMPLE — parte do projeto.

**`pre-applypatch.sample`** _(15 linhas)_
Arquivo SAMPLE — parte do projeto.

**`pre-commit.sample`** _(50 linhas)_
Arquivo SAMPLE — parte do projeto.

**`pre-merge-commit.sample`** _(14 linhas)_
Arquivo SAMPLE — parte do projeto.

**`pre-push.sample`** _(54 linhas)_
Arquivo SAMPLE — parte do projeto.

**`pre-rebase.sample`** _(170 linhas)_
Arquivo SAMPLE — parte do projeto.

**`pre-receive.sample`** _(25 linhas)_
Arquivo SAMPLE — parte do projeto.

**`prepare-commit-msg.sample`** _(43 linhas)_
Arquivo SAMPLE — parte do projeto.

**`push-to-checkout.sample`** _(79 linhas)_
Arquivo SAMPLE — parte do projeto.

**`sendemail-validate.sample`** _(78 linhas)_
Arquivo SAMPLE — parte do projeto.

**`update.sample`** _(129 linhas)_
Arquivo SAMPLE — parte do projeto.

---

### 📁 `.git/info/`
> Pasta 'info' — agrupamento de arquivos relacionados.

**`exclude`** _(7 linhas)_
Arquivo EXCLUDE — parte do projeto.

---

### 📁 `.git/logs/`
> Pasta 'logs' — agrupamento de arquivos relacionados.

**`HEAD`** _(15 linhas)_
Arquivo HEAD — parte do projeto.

---

### 📁 `.local/secondary_skills/`
> Pasta 'secondary_skills' — agrupamento de arquivos relacionados.

**`LICENSE.txt`** _(22 linhas)_
Arquivo TXT — parte do projeto.

---

### 📁 `.local/skills/`
> Pasta 'skills' — agrupamento de arquivos relacionados.

**`LICENSE.txt`** _(22 linhas)_
Arquivo TXT — parte do projeto.

---

### 📁 `client/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`auditoria.html`** _(259 linhas)_
Arquivo HTML — parte do projeto.

**`codigo-formatacao.txt`** _(123 linhas)_
Arquivo TXT — parte do projeto.

**`comparador.html`** _(494 linhas)_
Arquivo HTML — parte do projeto.

**`favicon.png`** _(7 linhas)_
Arquivo de imagem.

**`icon-192.png`** _(2304 linhas)_
Arquivo de imagem.

**`icon-512.png`** _(2216 linhas)_
Arquivo de imagem.

**`manifest.json`** _(25 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`sw.js`** _(19 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `client/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(169 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(351 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `migrations/meta/`
> Pasta 'meta' — agrupamento de arquivos relacionados.

**`0000_snapshot.json`** _(871 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`_journal.json`** _(13 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `shared/models/`
> Modelos de dados — representacao das tabelas do banco de dados.

**`chat.ts`** _(35 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.config/replit/.semgrep/`
> Pasta '.semgrep' — agrupamento de arquivos relacionados.

**`semgrep_rules.json`** _(51908 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.git/objects/01/`
> Pasta '01' — agrupamento de arquivos relacionados.

**`0f933fef4d29556d65cbbc93f332e897a7d836`** _(1 linha)_
Arquivo 0F933FEF4D29556D65CBBC93F332E897A7D836 — parte do projeto.

---

### 📁 `.git/objects/02/`
> Pasta '02' — agrupamento de arquivos relacionados.

**`098a71716e3d7afdc932143063317ab98e625c`** _(2 linhas)_
Arquivo 098A71716E3D7AFDC932143063317AB98E625C — parte do projeto.

---

### 📁 `.git/objects/0e/`
> Pasta '0e' — agrupamento de arquivos relacionados.

**`21917b77641ea6f26d8a74dfef140c9bf43f05`** _(1 linha)_
Arquivo 21917B77641EA6F26D8A74DFEF140C9BF43F05 — parte do projeto.

---

### 📁 `.git/objects/14/`
> Pasta '14' — agrupamento de arquivos relacionados.

**`515c06f8093d46c9dadba5a5e38342eebb3a41`** _(1 linha)_
Arquivo 515C06F8093D46C9DADBA5A5E38342EEBB3A41 — parte do projeto.

---

### 📁 `.git/objects/1d/`
> Pasta '1d' — agrupamento de arquivos relacionados.

**`285d20d62239428f1515f5f44955a64da83633`** _(1 linha)_
Arquivo 285D20D62239428F1515F5F44955A64DA83633 — parte do projeto.

---

### 📁 `.git/objects/22/`
> Pasta '22' — agrupamento de arquivos relacionados.

**`8c7a87b2158cc858eae600280602ea02e6f90b`** _(3 linhas)_
Arquivo 8C7A87B2158CC858EAE600280602EA02E6F90B — parte do projeto.

---

### 📁 `.git/objects/24/`
> Pasta '24' — agrupamento de arquivos relacionados.

**`7631141629198a79def36d2294042f06cf0b4e`** _(2 linhas)_
Arquivo 7631141629198A79DEF36D2294042F06CF0B4E — parte do projeto.

---

### 📁 `.git/objects/26/`
> Pasta '26' — agrupamento de arquivos relacionados.

**`fca19e2eff238ffc2e12be5dc2a204bae8e0a2`** _(1 linha)_
Arquivo FCA19E2EFF238FFC2E12BE5DC2A204BAE8E0A2 — parte do projeto.

---

### 📁 `.git/objects/2e/`
> Pasta '2e' — agrupamento de arquivos relacionados.

**`01f7292b88fcc769024d694fc1dd8e495f596c`** _(6 linhas)_
Arquivo 01F7292B88FCC769024D694FC1DD8E495F596C — parte do projeto.

---

### 📁 `.git/objects/32/`
> Pasta '32' — agrupamento de arquivos relacionados.

**`732dabf07f528bc24e32fb4b7f0b015f20157d`** _(1 linha)_
Arquivo 732DABF07F528BC24E32FB4B7F0B015F20157D — parte do projeto.

**`a5e26d270d46b95e93f63a0ec7136b5560f8e2`** _(15 linhas)_
Arquivo A5E26D270D46B95E93F63A0EC7136B5560F8E2 — parte do projeto.

---

### 📁 `.git/objects/35/`
> Pasta '35' — agrupamento de arquivos relacionados.

**`084c8476ac94669e1f80a8534ed18de568ff68`** _(486 linhas)_
Arquivo 084C8476AC94669E1F80A8534ED18DE568FF68 — parte do projeto.

**`631eaec75c63d864314099505ee79c2576ff11`** _(1 linha)_
Arquivo 631EAEC75C63D864314099505EE79C2576FF11 — parte do projeto.

---

### 📁 `.git/objects/39/`
> Pasta '39' — agrupamento de arquivos relacionados.

**`c5f0269ec451e3183151055ed16dd1f9aa9833`** _(1 linha)_
Arquivo C5F0269EC451E3183151055ED16DD1F9AA9833 — parte do projeto.

---

### 📁 `.git/objects/41/`
> Pasta '41' — agrupamento de arquivos relacionados.

**`e24d34bf37f6f5ecbdfaf5dcb122605656fef1`** _(3 linhas)_
Arquivo E24D34BF37F6F5ECBDFAF5DCB122605656FEF1 — parte do projeto.

---

### 📁 `.git/objects/42/`
> Pasta '42' — agrupamento de arquivos relacionados.

**`3ef46bb5f85a04ffbbd5840217881b319d379f`** _(1 linha)_
Arquivo 3EF46BB5F85A04FFBBD5840217881B319D379F — parte do projeto.

---

### 📁 `.git/objects/43/`
> Pasta '43' — agrupamento de arquivos relacionados.

**`2f32b1ed5f25004303af7a53d67cb073489545`** _(8 linhas)_
Arquivo 2F32B1ED5F25004303AF7A53D67CB073489545 — parte do projeto.

---

### 📁 `.git/objects/47/`
> Pasta '47' — agrupamento de arquivos relacionados.

**`61cd5f8d26b87a06fc2e709ef15c4269afddfd`** _(3 linhas)_
Arquivo 61CD5F8D26B87A06FC2E709EF15C4269AFDDFD — parte do projeto.

---

### 📁 `.git/objects/49/`
> Pasta '49' — agrupamento de arquivos relacionados.

**`bab97114fbc2a34742c3b7c6258688f0c319ba`** _(6 linhas)_
Arquivo BAB97114FBC2A34742C3B7C6258688F0C319BA — parte do projeto.

---

### 📁 `.git/objects/4b/`
> Pasta '4b' — agrupamento de arquivos relacionados.

**`94b99fbe4c162976d6742e69c94dd63192fbc8`** _(548 linhas)_
Arquivo 94B99FBE4C162976D6742E69C94DD63192FBC8 — parte do projeto.

---

### 📁 `.git/objects/51/`
> Pasta '51' — agrupamento de arquivos relacionados.

**`7e9985a4234f707e20ff6aec2ce196991954fc`** _(2 linhas)_
Arquivo 7E9985A4234F707E20FF6AEC2CE196991954FC — parte do projeto.

---

### 📁 `.git/objects/56/`
> Pasta '56' — agrupamento de arquivos relacionados.

**`ec5bf50fc10cc5dd65957655e07300db785f2c`** _(5 linhas)_
Arquivo EC5BF50FC10CC5DD65957655E07300DB785F2C — parte do projeto.

---

### 📁 `.git/objects/57/`
> Pasta '57' — agrupamento de arquivos relacionados.

**`198b63dd5f1d8884ac4bad7c4ed41eea15bb56`** _(1 linha)_
Arquivo 198B63DD5F1D8884AC4BAD7C4ED41EEA15BB56 — parte do projeto.

---

### 📁 `.git/objects/59/`
> Pasta '59' — agrupamento de arquivos relacionados.

**`9920427066c4d18e30ab6d48579baaa730b730`** _(2 linhas)_
Arquivo 9920427066C4D18E30AB6D48579BAAA730B730 — parte do projeto.

---

### 📁 `.git/objects/5a/`
> Pasta '5a' — agrupamento de arquivos relacionados.

**`a1184c12db15ed4de1161ada9baa581f3ea952`** _(1 linha)_
Arquivo A1184C12DB15ED4DE1161ADA9BAA581F3EA952 — parte do projeto.

**`de295b22ce532a150cede219d04c1c5b87c0c5`** _(1 linha)_
Arquivo DE295B22CE532A150CEDE219D04C1C5B87C0C5 — parte do projeto.

---

### 📁 `.git/objects/5b/`
> Pasta '5b' — agrupamento de arquivos relacionados.

**`85f37b666820fc6789e36500a8a25264d284fa`** _(1 linha)_
Arquivo 85F37B666820FC6789E36500A8A25264D284FA — parte do projeto.

---

### 📁 `.git/objects/5e/`
> Pasta '5e' — agrupamento de arquivos relacionados.

**`5d7f8c6017bf41f8aab2d4b6dddc436450ef81`** _(1 linha)_
Arquivo 5D7F8C6017BF41F8AAB2D4B6DDDC436450EF81 — parte do projeto.

---

### 📁 `.git/objects/5f/`
> Pasta '5f' — agrupamento de arquivos relacionados.

**`8c4511a44324a3bb2e0b68d52381ab682166fe`** _(2 linhas)_
Arquivo 8C4511A44324A3BB2E0B68D52381AB682166FE — parte do projeto.

---

### 📁 `.git/objects/60/`
> Pasta '60' — agrupamento de arquivos relacionados.

**`00c948ca3852c784b63580855ddfd24a2fba8e`** _(1 linha)_
Arquivo 00C948CA3852C784B63580855DDFD24A2FBA8E — parte do projeto.

---

### 📁 `.git/objects/69/`
> Pasta '69' — agrupamento de arquivos relacionados.

**`6e0d2b94fbc09e5bf2378678cfe86625c2f15c`** _(1 linha)_
Arquivo 6E0D2B94FBC09E5BF2378678CFE86625C2F15C — parte do projeto.

---

### 📁 `.git/objects/79/`
> Pasta '79' — agrupamento de arquivos relacionados.

**`8dce67e8d5175e2abad3b31cf007b0737f7403`** _(1 linha)_
Arquivo 8DCE67E8D5175E2ABAD3B31CF007B0737F7403 — parte do projeto.

---

### 📁 `.git/objects/7a/`
> Pasta '7a' — agrupamento de arquivos relacionados.

**`06badc3d5a93db6dbdc1ac0786e9f36027dcd4`** _(1 linha)_
Arquivo 06BADC3D5A93DB6DBDC1AC0786E9F36027DCD4 — parte do projeto.

---

### 📁 `.git/objects/7e/`
> Pasta '7e' — agrupamento de arquivos relacionados.

**`b8aaa7dcf576558014a1dc8d500a9e6d21c870`** _(2 linhas)_
Arquivo B8AAA7DCF576558014A1DC8D500A9E6D21C870 — parte do projeto.

---

### 📁 `.git/objects/86/`
> Pasta '86' — agrupamento de arquivos relacionados.

**`0358fa1fd66ac26404ada1e9268423984981dc`** _(8 linhas)_
Arquivo 0358FA1FD66AC26404ADA1E9268423984981DC — parte do projeto.

---

### 📁 `.git/objects/89/`
> Pasta '89' — agrupamento de arquivos relacionados.

**`7183c53372503a17fb0321783ec78dcc5b52bd`** _(2 linhas)_
Arquivo 7183C53372503A17FB0321783EC78DCC5B52BD — parte do projeto.

---

### 📁 `.git/objects/8f/`
> Pasta '8f' — agrupamento de arquivos relacionados.

**`171f68dc233525d7c8304b4eeaf96283915ead`** _(1 linha)_
Arquivo 171F68DC233525D7C8304B4EEAF96283915EAD — parte do projeto.

---

### 📁 `.git/objects/91/`
> Pasta '91' — agrupamento de arquivos relacionados.

**`84ee2c2a44a71b7805c33fec085636582e7ad6`** _(1 linha)_
Arquivo 84EE2C2A44A71B7805C33FEC085636582E7AD6 — parte do projeto.

---

### 📁 `.git/objects/94/`
> Pasta '94' — agrupamento de arquivos relacionados.

**`0375e8218a6553f013e2b76e04cace9eea8d8a`** _(1 linha)_
Arquivo 0375E8218A6553F013E2B76E04CACE9EEA8D8A — parte do projeto.

---

### 📁 `.git/objects/98/`
> Pasta '98' — agrupamento de arquivos relacionados.

**`0bf1f4dc5aac2ba96d1039b6860b5f114f2a1e`** _(4 linhas)_
Arquivo 0BF1F4DC5AAC2BA96D1039B6860B5F114F2A1E — parte do projeto.

---

### 📁 `.git/objects/9e/`
> Pasta '9e' — agrupamento de arquivos relacionados.

**`48cdbea6ca8e1e6ab2c6f9d3b3d504519ba8f1`** _(2 linhas)_
Arquivo 48CDBEA6CA8E1E6AB2C6F9D3B3D504519BA8F1 — parte do projeto.

---

### 📁 `.git/objects/a3/`
> Pasta 'a3' — agrupamento de arquivos relacionados.

**`23e8b8daf5cdfd7f719c6d77d3a1a60d175408`** _(1 linha)_
Arquivo 23E8B8DAF5CDFD7F719C6D77D3A1A60D175408 — parte do projeto.

---

### 📁 `.git/objects/a8/`
> Pasta 'a8' — agrupamento de arquivos relacionados.

**`36626f7be22e6636f493f6f37bfd567fdc871d`** _(1 linha)_
Arquivo 36626F7BE22E6636F493F6F37BFD567FDC871D — parte do projeto.

**`49d26fa5350a0447d55a4f8a9a54bcc2f45d40`** _(51 linhas)_
Arquivo 49D26FA5350A0447D55A4F8A9A54BCC2F45D40 — parte do projeto.

---

### 📁 `.git/objects/ab/`
> Pasta 'ab' — agrupamento de arquivos relacionados.

**`3d5fa8fd7d22f2c900ad376e6cae0c090cc44f`** _(28 linhas)_
Arquivo 3D5FA8FD7D22F2C900AD376E6CAE0C090CC44F — parte do projeto.

---

### 📁 `.git/objects/ad/`
> Pasta 'ad' — agrupamento de arquivos relacionados.

**`48952423c08b6975cc563c69baac60b1024e62`** _(5 linhas)_
Arquivo 48952423C08B6975CC563C69BAAC60B1024E62 — parte do projeto.

---

### 📁 `.git/objects/ae/`
> Pasta 'ae' — agrupamento de arquivos relacionados.

**`5c07564541a2f6f84f1fec8fd5fd205dae3953`** _(6 linhas)_
Arquivo 5C07564541A2F6F84F1FEC8FD5FD205DAE3953 — parte do projeto.

---

### 📁 `.git/objects/b0/`
> Pasta 'b0' — agrupamento de arquivos relacionados.

**`3e72732c7c1d8a2998df671c552788b7c6d3ec`** _(2 linhas)_
Arquivo 3E72732C7C1D8A2998DF671C552788B7C6D3EC — parte do projeto.

---

### 📁 `.git/objects/b6/`
> Pasta 'b6' — agrupamento de arquivos relacionados.

**`af4ac5b2b1e5f54d720e789263f8d2dd5a829f`** _(3 linhas)_
Arquivo AF4AC5B2B1E5F54D720E789263F8D2DD5A829F — parte do projeto.

---

### 📁 `.git/objects/bc/`
> Pasta 'bc' — agrupamento de arquivos relacionados.

**`6cce105c59e7cb61a4b46d3cbbfc42939de319`** _(7 linhas)_
Arquivo 6CCE105C59E7CB61A4B46D3CBBFC42939DE319 — parte do projeto.

---

### 📁 `.git/objects/c7/`
> Pasta 'c7' — agrupamento de arquivos relacionados.

**`a0147554e624be84c0ec415bea358965f1f550`** _(2 linhas)_
Arquivo A0147554E624BE84C0EC415BEA358965F1F550 — parte do projeto.

---

### 📁 `.git/objects/c9/`
> Pasta 'c9' — agrupamento de arquivos relacionados.

**`17b0279e3a7990eaa95c9540d9a0b0cb8dfd08`** _(3 linhas)_
Arquivo 17B0279E3A7990EAA95C9540D9A0B0CB8DFD08 — parte do projeto.

---

### 📁 `.git/objects/ca/`
> Pasta 'ca' — agrupamento de arquivos relacionados.

**`b18d2e5d58e5996b29efbb8a7df3730f753cd1`** _(22 linhas)_
Arquivo B18D2E5D58E5996B29EFBB8A7DF3730F753CD1 — parte do projeto.

---

### 📁 `.git/objects/cc/`
> Pasta 'cc' — agrupamento de arquivos relacionados.

**`6307131a5395c2ba191ae542e984645b9a870e`** _(2 linhas)_
Arquivo 6307131A5395C2BA191AE542E984645B9A870E — parte do projeto.

---

### 📁 `.git/objects/d6/`
> Pasta 'd6' — agrupamento de arquivos relacionados.

**`40423b8635f174075473ce6c0fe7ddf3e63b45`** _(3 linhas)_
Arquivo 40423B8635F174075473CE6C0FE7DDF3E63B45 — parte do projeto.

---

### 📁 `.git/objects/d8/`
> Pasta 'd8' — agrupamento de arquivos relacionados.

**`3468ba8001865edc053aaae09e3067893f77a2`** _(1 linha)_
Arquivo 3468BA8001865EDC053AAAE09E3067893F77A2 — parte do projeto.

---

### 📁 `.git/objects/df/`
> Pasta 'df' — agrupamento de arquivos relacionados.

**`2e36040de34bd6f71d78ad41119920dd7fd554`** _(1 linha)_
Arquivo 2E36040DE34BD6F71D78AD41119920DD7FD554 — parte do projeto.

---

### 📁 `.git/objects/e6/`
> Pasta 'e6' — agrupamento de arquivos relacionados.

**`2b24e41b4988b9f5a88f75b067cadd547c7c86`** _(6 linhas)_
Arquivo 2B24E41B4988B9F5A88F75B067CADD547C7C86 — parte do projeto.

---

### 📁 `.git/objects/eb/`
> Pasta 'eb' — agrupamento de arquivos relacionados.

**`44dc6928d1b538a84a0b5fff6663588c20fcde`** _(56 linhas)_
Arquivo 44DC6928D1B538A84A0B5FFF6663588C20FCDE — parte do projeto.

---

### 📁 `.git/objects/ec/`
> Pasta 'ec' — agrupamento de arquivos relacionados.

**`c21a22441bd8496c15b725f5c0692a007076d6`** _(1 linha)_
Arquivo C21A22441BD8496C15B725F5C0692A007076D6 — parte do projeto.

---

### 📁 `.git/objects/ee/`
> Pasta 'ee' — agrupamento de arquivos relacionados.

**`154b37543bda3bb146ce702bc78be977629536`** _(28 linhas)_
Arquivo 154B37543BDA3BB146CE702BC78BE977629536 — parte do projeto.

---

### 📁 `.git/objects/f5/`
> Pasta 'f5' — agrupamento de arquivos relacionados.

**`a7f0a80a7d04b7e41a83c7516711775bb31af3`** _(2 linhas)_
Arquivo A7F0A80A7D04B7E41A83C7516711775BB31AF3 — parte do projeto.

---

### 📁 `.git/objects/fe/`
> Pasta 'fe' — agrupamento de arquivos relacionados.

**`11f3e11f23be794a79f703617530784e33940f`** _(1 linha)_
Arquivo 11F3E11F23BE794A79F703617530784E33940F — parte do projeto.

---

### 📁 `.git/objects/pack/`
> Pasta 'pack' — agrupamento de arquivos relacionados.

**`pack-b039e4dd2d5151432844012a311727745540bc68.idx`** _(24 linhas)_
Arquivo IDX — parte do projeto.

**`pack-b039e4dd2d5151432844012a311727745540bc68.pack`** _(182140 linhas)_
Arquivo PACK — parte do projeto.

**`pack-b039e4dd2d5151432844012a311727745540bc68.rev`** _(3 linhas)_
Arquivo REV — parte do projeto.

---

### 📁 `.git/refs/heads/`
> Pasta 'heads' — agrupamento de arquivos relacionados.

**`main`** _(2 linhas)_
Arquivo MAIN — parte do projeto.

**`replit-agent`** _(2 linhas)_
Arquivo REPLIT-AGENT — parte do projeto.

---

### 📁 `.git/refs/notes/`
> Pasta 'notes' — agrupamento de arquivos relacionados.

**`commits`** _(2 linhas)_
Arquivo COMMITS — parte do projeto.

---

### 📁 `.git/refs/replit/`
> Pasta 'replit' — agrupamento de arquivos relacionados.

**`agent-ledger`** _(2 linhas)_
Arquivo AGENT-LEDGER — parte do projeto.

---

### 📁 `.local/secondary_skills/ad-creative/`
> Pasta 'ad-creative' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(877 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/ai-recruiter/`
> Pasta 'ai-recruiter' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(1088 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/ai-sdr/`
> Pasta 'ai-sdr' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(205 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/ai-secretary/`
> Pasta 'ai-secretary' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(1133 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/branding-generator/`
> Pasta 'branding-generator' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(287 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/competitive-analysis/`
> Pasta 'competitive-analysis' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(430 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/content-machine/`
> Pasta 'content-machine' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(322 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/deep-research/`
> Pasta 'deep-research' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(522 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/design-thinker/`
> Pasta 'design-thinker' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(328 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/excel-generator/`
> Pasta 'excel-generator' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(955 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`financial-models.md`** _(290 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/file-converter/`
> Pasta 'file-converter' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(824 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/flashcard-generator/`
> Pasta 'flashcard-generator' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(234 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/geo/`
> Pasta 'geo' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(379 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/github-solution-finder/`
> Pasta 'github-solution-finder' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(175 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/infographic-builder/`
> Pasta 'infographic-builder' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(318 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`antv-syntax.md`** _(471 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`react-fallback.md`** _(211 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/insurance-optimizer/`
> Pasta 'insurance-optimizer' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(210 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/interview-prep/`
> Pasta 'interview-prep' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(350 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/invoice-generator/`
> Pasta 'invoice-generator' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(528 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/legal-contract/`
> Pasta 'legal-contract' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(978 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/meal-planner/`
> Pasta 'meal-planner' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(518 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/personal-shopper/`
> Pasta 'personal-shopper' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(362 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/photo-editor/`
> Pasta 'photo-editor' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(606 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/podcast-generator/`
> Pasta 'podcast-generator' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(561 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/podcast-marketing/`
> Pasta 'podcast-marketing' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(551 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`audio-processing.md`** _(531 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`content-atoms.md`** _(254 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`content-calendar.md`** _(319 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`content-templates.md`** _(326 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`quote-cards.md`** _(239 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`rss-and-batch.md`** _(360 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`video-clips.md`** _(661 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`youtube-processing.md`** _(329 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/product-manager/`
> Pasta 'product-manager' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(273 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/programmatic-seo/`
> Pasta 'programmatic-seo' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(1208 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/real-estate-analyzer/`
> Pasta 'real-estate-analyzer' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(787 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/recipe-creator/`
> Pasta 'recipe-creator' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(260 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/recreate-screenshot/`
> Pasta 'recreate-screenshot' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(216 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/resume-maker/`
> Pasta 'resume-maker' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(791 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/seo-auditor/`
> Pasta 'seo-auditor' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(449 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/skill-creator/`
> Pasta 'skill-creator' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(215 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/skill-finder/`
> Pasta 'skill-finder' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(298 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/stock-analyzer/`
> Pasta 'stock-analyzer' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(799 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/storyboard/`
> Pasta 'storyboard' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(559 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/supplier-research/`
> Pasta 'supplier-research' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(214 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/tax-reviewer/`
> Pasta 'tax-reviewer' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(132 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/travel-assistant/`
> Pasta 'travel-assistant' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(668 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/video-editing/`
> Pasta 'video-editing' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(706 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`dead-space-and-chunking.md`** _(1082 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`operations.md`** _(1720 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`virality-scoring.md`** _(1213 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`voiceover.md`** _(789 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/secondary_skills/website-cloning/`
> Pasta 'website-cloning' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(545 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`extraction.md`** _(1208 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`pitfalls.md`** _(298 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/agent-inbox/`
> Pasta 'agent-inbox' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(129 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/artifacts/`
> Pasta 'artifacts' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(22 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`bootstrap-legacy.js`** _(103 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`bootstrap.js`** _(106 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/canvas/`
> Pasta 'canvas' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(449 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`__init__.py`** _(2 linhas)_
Arquivo Python — codigo de logica ou script de automacao.

---

### 📁 `.local/skills/code_review/`
> Pasta 'code_review' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(83 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/database/`
> Pasta 'database' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(205 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/delegation/`
> Pasta 'delegation' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(202 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/deployment/`
> Pasta 'deployment' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(229 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/design/`
> Pasta 'design' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(223 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/design-exploration/`
> Pasta 'design-exploration' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(96 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/diagnostics/`
> Pasta 'diagnostics' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(123 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/environment-secrets/`
> Pasta 'environment-secrets' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(202 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/external_apis/`
> Pasta 'external_apis' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(22 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/follow-up-tasks/`
> Pasta 'follow-up-tasks' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(80 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/fullstack-js/`
> Pasta 'fullstack-js' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(118 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/integrations/`
> Pasta 'integrations' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(203 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/media-generation/`
> Pasta 'media-generation' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(251 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/mockup-extract/`
> Pasta 'mockup-extract' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(124 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/mockup-graduate/`
> Pasta 'mockup-graduate' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(98 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/mockup-sandbox/`
> Pasta 'mockup-sandbox' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(682 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/package-management/`
> Pasta 'package-management' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(263 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/post_merge_setup/`
> Pasta 'post_merge_setup' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(103 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/project_tasks/`
> Pasta 'project_tasks' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(380 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/query-integration-data/`
> Pasta 'query-integration-data' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(355 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/remove-image-background/`
> Pasta 'remove-image-background' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(56 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/repl_setup/`
> Pasta 'repl_setup' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(89 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/replit-docs/`
> Pasta 'replit-docs' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(82 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/revenuecat/`
> Pasta 'revenuecat' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(134 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/security_scan/`
> Pasta 'security_scan' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(50 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/skill-authoring/`
> Pasta 'skill-authoring' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(100 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/stripe/`
> Pasta 'stripe' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(456 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/suggest-new-project/`
> Pasta 'suggest-new-project' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(60 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/threat_modeling/`
> Pasta 'threat_modeling' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(241 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/validation/`
> Pasta 'validation' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(238 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/web-search/`
> Pasta 'web-search' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(126 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/workflows/`
> Pasta 'workflows' — agrupamento de arquivos relacionados.

**`.fingerprint`** _(1 linha)_
Arquivo FINGERPRINT — parte do projeto.

**`SKILL.md`** _(246 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/state/replit/`
> Pasta 'replit' — agrupamento de arquivos relacionados.

**`log-query.db`** _(1441 linhas)_
Arquivo DB — parte do projeto.

**`log-query.db-shm`** _(2 linhas)_
Arquivo DB-SHM — parte do projeto.

**`log-query.db-wal`** _(18614 linhas)_
Arquivo DB-WAL — parte do projeto.

---

### 📁 `.local/state/scribe/`
> Pasta 'scribe' — agrupamento de arquivos relacionados.

**`scribe.db`** _(1 linha)_
Arquivo DB — parte do projeto.

**`scribe.db-shm`** _(2 linhas)_
Arquivo DB-SHM — parte do projeto.

**`scribe.db-wal`** _(44 linhas)_
Arquivo DB-WAL — parte do projeto.

---

### 📁 `client/replit_integrations/audio/`
> Pasta 'audio' — agrupamento de arquivos relacionados.

**`audio-playback-worklet.js`** _(113 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`audio-utils.ts`** _(37 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

**`index.ts`** _(46 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`useAudioPlayback.ts`** _(106 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'audioplayback'.

**`useVoiceRecorder.ts`** _(53 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'voicerecorder'.

**`useVoiceStream.ts`** _(92 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'voicestream'.

---

### 📁 `client/src/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`pwa-install.tsx`** _(86 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`theme-provider.tsx`** _(47 linhas)_
Componente PROVIDER — 'fornece' dados/funcoes para todos os componentes filhos via Context API do React.

**`theme-toggle.tsx`** _(19 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tiptap-editor.tsx`** _(542 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

---

### 📁 `client/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(192 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `client/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`queryClient.ts`** _(58 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `client/src/pages/`
> Telas completas do app — cada arquivo aqui e uma pagina navegavel.

**`auditoria-financeira.tsx`** _(25 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`code-assistant.tsx`** _(1000 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`comparador-juridico.tsx`** _(25 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`comunicacoes-cnj.tsx`** _(403 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`consulta-corporativo.tsx`** _(479 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`consulta-pdpj.tsx`** _(671 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`consulta-processual.tsx`** _(656 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`filtrador.tsx`** _(732 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`jurisprudencia.tsx`** _(3837 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`legal-assistant.tsx`** _(5404 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`legal-assistant.tsx.recovered`** _(3763 linhas)_
Arquivo RECOVERED — parte do projeto.

**`login.tsx`** _(100 linhas)_
Componente de LOGIN/AUTENTICACAO — tela de entrada com usuario e senha.

**`not-found.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`painel-processos.tsx`** _(758 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`playground.tsx`** _(1473 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`previdenciario.tsx`** _(770 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`robo-djen.tsx`** _(1053 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`token-generator.tsx`** _(450 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tramitacao.tsx`** _(828 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `server/replit_integrations/audio/`
> Pasta 'audio' — agrupamento de arquivos relacionados.

**`client.ts`** _(275 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`index.ts`** _(15 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`routes.ts`** _(137 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

---

### 📁 `server/replit_integrations/batch/`
> Pasta 'batch' — agrupamento de arquivos relacionados.

**`index.ts`** _(8 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`utils.ts`** _(183 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `server/replit_integrations/chat/`
> Pasta 'chat' — agrupamento de arquivos relacionados.

**`index.ts`** _(4 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`routes.ts`** _(204 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

**`storage.ts`** _(44 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `server/replit_integrations/image/`
> Pasta 'image' — agrupamento de arquivos relacionados.

**`client.ts`** _(60 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`index.ts`** _(4 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`routes.ts`** _(32 linhas)_
Arquivo de ROTAS — define as URLs/enderecos respondidos pelo servidor.

---

### 📁 `.git/logs/refs/heads/`
> Pasta 'heads' — agrupamento de arquivos relacionados.

**`main`** _(14 linhas)_
Arquivo MAIN — parte do projeto.

**`replit-agent`** _(13 linhas)_
Arquivo REPLIT-AGENT — parte do projeto.

---

### 📁 `.git/logs/refs/notes/`
> Pasta 'notes' — agrupamento de arquivos relacionados.

**`commits`** _(4 linhas)_
Arquivo COMMITS — parte do projeto.

---

### 📁 `.git/refs/remotes/gitsafe-backup/`
> Pasta 'gitsafe-backup' — agrupamento de arquivos relacionados.

**`main`** _(2 linhas)_
Arquivo MAIN — parte do projeto.

---

### 📁 `.git/refs/remotes/origin/`
> Pasta 'origin' — agrupamento de arquivos relacionados.

**`main`** _(2 linhas)_
Arquivo MAIN — parte do projeto.

---

### 📁 `.local/secondary_skills/geo/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`content-patterns.md`** _(159 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`platform-notes.md`** _(129 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`scorecard.md`** _(114 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`technical-checklist.md`** _(258 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/artifacts/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`multi-artifact-creation.md`** _(95 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/deployment/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`deployment-logs.md`** _(148 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/external_apis/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`brave.md`** _(114 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/fullstack-js/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`hover_and_elevation.md`** _(61 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`layout_and_spacing.md`** _(41 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`shadcn_component_rules.md`** _(216 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`sidebar_rules.md`** _(161 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`visual_style_and_contrast.md`** _(74 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/repl_setup/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`angular.md`** _(104 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`react_vite.md`** _(122 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`vue.md`** _(103 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/revenuecat/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`initial-setup.md`** _(567 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`replit-revenuecat-sdk-docs.md`** _(280 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`subsequent-management.md`** _(64 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/skills/stripe/references/`
> Pasta 'references' — agrupamento de arquivos relacionados.

**`code-templates.md`** _(589 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

---

### 📁 `.local/state/replit/agent/`
> Pasta 'agent' — agrupamento de arquivos relacionados.

**`.agent_state_010f933fef4d29556d65cbbc93f332e897a7d836.bin`** _(129 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_14515c06f8093d46c9dadba5a5e38342eebb3a41.bin`** _(40 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_228c7a87b2158cc858eae600280602ea02e6f90b.bin`** _(333 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_432f32b1ed5f25004303af7a53d67cb073489545.bin`** _(205 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_5b85f37b666820fc6789e36500a8a25264d284fa.bin`** _(264 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_6000c948ca3852c784b63580855ddfd24a2fba8e.bin`** _(145 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_980bf1f4dc5aac2ba96d1039b6860b5f114f2a1e.bin`** _(313 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_ae5c07564541a2f6f84f1fec8fd5fd205dae3953.bin`** _(235 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_b03e72732c7c1d8a2998df671c552788b7c6d3ec.bin`** _(308 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_cc6307131a5395c2ba191ae542e984645b9a870e.bin`** _(196 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_f5a7f0a80a7d04b7e41a83c7516711775bb31af3.bin`** _(309 linhas)_
Arquivo BIN — parte do projeto.

**`.agent_state_main.bin`** _(364 linhas)_
Arquivo BIN — parte do projeto.

**`.latest.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`progress_tracker.md`** _(5 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`repl_state.bin`** _(34 linhas)_
Arquivo BIN — parte do projeto.

---

### 📁 `.local/state/workflow-logs/55Gr7v8DXu5ewWUWfs4Lq/`
> Pasta '55Gr7v8DXu5ewWUWfs4Lq' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(9 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/5cDC29B7tJw5XXbBOrhWh/`
> Pasta '5cDC29B7tJw5XXbBOrhWh' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(9 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/E1ZL-IAPLGApOqirZ4sJY/`
> Pasta 'E1ZL-IAPLGApOqirZ4sJY' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/GtNudELQEcgARdYMZXL2U/`
> Pasta 'GtNudELQEcgARdYMZXL2U' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/HPbCVcItFOa3mfeJFK8kf/`
> Pasta 'HPbCVcItFOa3mfeJFK8kf' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/hWQEAm0pGU0QvTGg2KeoI/`
> Pasta 'hWQEAm0pGU0QvTGg2KeoI' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/Ij6htOPNrryT22iN66-TE/`
> Pasta 'Ij6htOPNrryT22iN66-TE' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(14 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/Jg0_YczQpCvNyu5SPmfpI/`
> Pasta 'Jg0_YczQpCvNyu5SPmfpI' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(9 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/Kr4Rl61IQpvtOMDRHcc0d/`
> Pasta 'Kr4Rl61IQpvtOMDRHcc0d' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(29 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/LbZi5kZQB7Ym_CrpUVI_H/`
> Pasta 'LbZi5kZQB7Ym_CrpUVI_H' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(34 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/LN8Ypo2mUdcuyqFhIh6Fl/`
> Pasta 'LN8Ypo2mUdcuyqFhIh6Fl' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/naLrCNUov5fD0PtVxdPdU/`
> Pasta 'naLrCNUov5fD0PtVxdPdU' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(9 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/pITQDUoOlG2F1v9qoRwHb/`
> Pasta 'pITQDUoOlG2F1v9qoRwHb' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/Pw0Qq6gHq3cQ4SWSW6oQB/`
> Pasta 'Pw0Qq6gHq3cQ4SWSW6oQB' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/SQjKh0Fh_-kO7G-0Vi5bG/`
> Pasta 'SQjKh0Fh_-kO7G-0Vi5bG' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(15 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/tljoQIkZd--W9BtSbS0aX/`
> Pasta 'tljoQIkZd--W9BtSbS0aX' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(9 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/Ujr1I1TrA5ofTdJDo9VZP/`
> Pasta 'Ujr1I1TrA5ofTdJDo9VZP' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(9 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/x7K8OcA4UDDBilTnmKtwZ/`
> Pasta 'x7K8OcA4UDDBilTnmKtwZ' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `.local/state/workflow-logs/X8A4VPXQihbRxTi8hznz4/`
> Pasta 'X8A4VPXQihbRxTi8hznz4' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`start_application.shell.exec.0`** _(32 linhas)_
Arquivo 0 — parte do projeto.

---

### 📁 `.local/state/workflow-logs/zMCgmyyArMsumYNVrbt1S/`
> Pasta 'zMCgmyyArMsumYNVrbt1S' — agrupamento de arquivos relacionados.

**`metadata.json`** _(1 linha)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

---

### 📁 `client/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(57 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(52 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(39 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button.tsx`** _(63 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(69 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(86 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(366 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(152 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(123 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(119 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(199 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`form.tsx`** _(179 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(30 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(24 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`label.tsx`** _(25 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(257 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(161 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(728 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(118 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(31 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `.git/logs/refs/remotes/gitsafe-backup/`
> Pasta 'gitsafe-backup' — agrupamento de arquivos relacionados.

**`main`** _(12 linhas)_
Arquivo MAIN — parte do projeto.

---

### 📁 `.git/logs/refs/remotes/origin/`
> Pasta 'origin' — agrupamento de arquivos relacionados.

**`main`** _(2 linhas)_
Arquivo MAIN — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/automation/`
> Pasta 'automation' — agrupamento de arquivos relacionados.

**`artifact.yaml`** _(41 linhas)_
Arquivo YAML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/data-visualization/`
> Pasta 'data-visualization' — agrupamento de arquivos relacionados.

**`artifact.yaml`** _(48 linhas)_
Arquivo YAML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/expo/`
> Pasta 'expo' — agrupamento de arquivos relacionados.

**`OWNERS`** _(3 linhas)_
Arquivo OWNERS — parte do projeto.

**`artifact.yaml`** _(48 linhas)_
Arquivo YAML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/`
> Pasta 'mockup-sandbox' — agrupamento de arquivos relacionados.

**`artifact.yaml`** _(16 linhas)_
Arquivo YAML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/`
> Pasta 'react-vite' — agrupamento de arquivos relacionados.

**`artifact.yaml`** _(39 linhas)_
Arquivo YAML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/slides/`
> Pasta 'slides' — agrupamento de arquivos relacionados.

**`artifact.yaml`** _(34 linhas)_
Arquivo YAML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/video-js/`
> Pasta 'video-js' — agrupamento de arquivos relacionados.

**`artifact.yaml`** _(38 linhas)_
Arquivo YAML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/`
> Pasta 'files' — agrupamento de arquivos relacionados.

**`.gitignore`** _(9 linhas)_
Lista de arquivos/pastas que o Git deve IGNORAR (nao versionar). Ex: node_modules, .env

**`package.json.template`** _(48 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`tsconfig.json`** _(27 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/`
> Pasta 'files' — agrupamento de arquivos relacionados.

**`.gitignore`** _(42 linhas)_
Lista de arquivos/pastas que o Git deve IGNORAR (nao versionar). Ex: node_modules, .env

**`app.json.template`** _(39 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`babel.config.js`** _(7 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`metro.config.js`** _(4 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`package.json.template`** _(59 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`tsconfig.json`** _(24 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/files/`
> Pasta 'files' — agrupamento de arquivos relacionados.

**`components.json`** _(22 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html`** _(32 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`mockupPreviewPlugin.ts`** _(200 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`package.json.template`** _(76 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`tsconfig.json`** _(21 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(73 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/files/`
> Pasta 'files' — agrupamento de arquivos relacionados.

**`components.json`** _(20 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html.template`** _(17 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`package.json.template`** _(78 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`tsconfig.json`** _(23 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(76 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `.local/skills/artifacts/artifacts/slides/files/`
> Pasta 'files' — agrupamento de arquivos relacionados.

**`index.html.template`** _(47 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`package.json.template`** _(31 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`tsconfig.json`** _(17 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(75 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/`
> Pasta 'files' — agrupamento de arquivos relacionados.

**`index.html.template`** _(28 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`package.json.template`** _(37 linhas)_
Arquivo TEMPLATE — parte do projeto.

**`tsconfig.json`** _(17 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(80 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/scripts/`
> Pasta 'scripts' — agrupamento de arquivos relacionados.

**`build.sh`** _(7 linhas)_
Arquivo SH — parte do projeto.

**`inngest.sh`** _(19 linhas)_
Arquivo SH — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`global.d.ts`** _(2 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/tests/`
> Testes automatizados — verificam se o codigo funciona corretamente.

**`testCronAutomation.ts`** _(87 linhas)_
Arquivo de TESTES — verifica automaticamente se o codigo funciona corretamente.

**`testWebhookAutomation.ts`** _(119 linhas)_
Arquivo de TESTES — verifica automaticamente se o codigo funciona corretamente.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/app/`
> Pasta 'app' — agrupamento de arquivos relacionados.

**`+not-found.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`_layout.tsx`** _(61 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`ErrorBoundary.tsx`** _(55 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`ErrorFallback.tsx`** _(279 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`KeyboardAwareScrollViewCompat.tsx`** _(30 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/constants/`
> Pasta 'constants' — agrupamento de arquivos relacionados.

**`colors.ts`** _(60 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`useColors.ts`** _(25 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'colors'.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/scripts/`
> Pasta 'scripts' — agrupamento de arquivos relacionados.

**`build.js`** _(574 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/server/`
> Pasta 'server' — agrupamento de arquivos relacionados.

**`serve.js`** _(136 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/files/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`favicon.svg`** _(4 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/files/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(147 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(158 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/files/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`favicon.svg`** _(4 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/files/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(43 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(393 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `.local/skills/artifacts/artifacts/slides/files/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`favicon.svg`** _(4 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

---

### 📁 `.local/skills/artifacts/artifacts/slides/files/scripts/`
> Pasta 'scripts' — agrupamento de arquivos relacionados.

**`validate-slides.ts`** _(194 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/slides/files/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(236 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(49 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(15 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

**`slideLoader.ts`** _(52 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`favicon.svg`** _(4 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/scripts/`
> Pasta 'scripts' — agrupamento de arquivos relacionados.

**`validate-recording.sh`** _(39 linhas)_
Arquivo SH — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(6 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(51 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/mastra/`
> Pasta 'mastra' — agrupamento de arquivos relacionados.

**`index.ts`** _(213 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/triggers/`
> Pasta 'triggers' — agrupamento de arquivos relacionados.

**`cronTriggers.ts`** _(62 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`exampleConnectorTrigger.ts`** _(154 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`slackTriggers.ts`** _(639 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`telegramTriggers.ts`** _(95 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/app/(tabs)/`
> Pasta '(tabs)' — agrupamento de arquivos relacionados.

**`_layout.tsx`** _(87 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

**`index.tsx`** _(29 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/assets/images/`
> Pasta 'images' — agrupamento de arquivos relacionados.

**`icon.png`** _(1246 linhas)_
Arquivo de imagem.

---

### 📁 `.local/skills/artifacts/artifacts/expo/files/server/templates/`
> Pasta 'templates' — agrupamento de arquivos relacionados.

**`landing-page.html`** _(461 linhas)_
Arquivo HTML — parte do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/files/src/.generated/`
> Pasta '.generated' — agrupamento de arquivos relacionados.

**`mockup-components.ts`** _(4 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/files/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(190 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/files/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/files/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(192 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/files/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/files/src/pages/`
> Telas completas do app — cada arquivo aqui e uma pagina navegavel.

**`not-found.tsx`** _(22 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `.local/skills/artifacts/artifacts/slides/files/src/data/`
> Pasta 'data' — agrupamento de arquivos relacionados.

**`slides-manifest.json`** _(2 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`slidesManifestSchema.ts`** _(34 linhas)_
Arquivo de MODELO — define a estrutura dos dados (tabelas, campos, tipos).

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/mastra/agents/`
> Pasta 'agents' — agrupamento de arquivos relacionados.

**`agent.ts`** _(90 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/mastra/inngest/`
> Pasta 'inngest' — agrupamento de arquivos relacionados.

**`client.ts`** _(18 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`index.ts`** _(215 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/mastra/storage/`
> Pasta 'storage' — agrupamento de arquivos relacionados.

**`index.ts`** _(9 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/mastra/tools/`
> Pasta 'tools' — agrupamento de arquivos relacionados.

**`exampleTool.ts`** _(72 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/automation/files/src/mastra/workflows/`
> Pasta 'workflows' — agrupamento de arquivos relacionados.

**`workflow.ts`** _(204 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `.local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(44 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(66 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(368 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(169 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(728 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `.local/skills/artifacts/artifacts/react-vite/files/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(44 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(66 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(368 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(169 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(728 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/src/components/video/`
> Pasta 'video' — agrupamento de arquivos relacionados.

**`ReplitLoadingScene.tsx`** _(106 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`VideoTemplate.tsx`** _(31 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`index.ts`** _(2 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `.local/skills/artifacts/artifacts/video-js/files/src/lib/video/`
> Pasta 'video' — agrupamento de arquivos relacionados.

**`animations.ts`** _(240 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`hooks.ts`** _(105 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(20 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: SK-Code-Editor-APK (5)
Tipo: Full-Stack (React + Express)
Stack: React + Vite, TypeScript, Tailwind CSS, Python, Node.js + Express, PostgreSQL, Drizzle ORM
Arquivos: 697 | Linhas: ~394.870
Rotas API: 123 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: AI_INTEGRATIONS_OPENAI_BASE_URL, AI_INTEGRATIONS_OPENAI_API_KEY, OPENAI_BASE_URL, OPENAI_API_KEY, PORT, INNGEST_PORT, BASE_PATH, REPLIT_DOMAINS, DATABASE_URL, REPLIT_CONNECTORS_HOSTNAME, TELEGRAM_BOT_TOKEN, REPLIT_INTERNAL_APP_DOMAIN, REPLIT_DEV_DOMAIN, EXPO_PUBLIC_DOMAIN, REPL_ID, EXPO_PUBLIC_REPL_ID, SESSION_SECRET, PUBLIC_API_KEY, APP_PASSWORD, AI_INTEGRATIONS_GEMINI_API_KEY, AI_INTEGRATIONS_GEMINI_BASE_URL, PDPJ_PEM_PRIVATE_KEY, PUBLIC_API_MODEL, PUBLIC_API_URL, DATAJUD_API_KEY, PERPLEXITY_API_KEY

Estrutura principal:
  .config/replit/.semgrep/semgrep_rules.json
  .git/COMMIT_EDITMSG
  .git/FETCH_HEAD
  .git/HEAD
  .git/ORIG_HEAD
  .git/config
  .git/description
  .git/hooks/applypatch-msg.sample
  .git/hooks/commit-msg.sample
  .git/hooks/fsmonitor-watchman.sample
  .git/hooks/post-update.sample
  .git/hooks/pre-applypatch.sample
  .git/hooks/pre-commit.sample
  .git/hooks/pre-merge-commit.sample
  .git/hooks/pre-push.sample
  .git/hooks/pre-rebase.sample
  .git/hooks/pre-receive.sample
  .git/hooks/prepare-commit-msg.sample
  .git/hooks/push-to-checkout.sample
  .git/hooks/sendemail-validate.sample
  .git/hooks/update.sample
  .git/index
  .git/info/exclude
  .git/logs/HEAD
  .git/logs/refs/heads/main
  .git/logs/refs/heads/replit-agent
  .git/logs/refs/notes/commits
  .git/logs/refs/remotes/gitsafe-backup/main
  .git/logs/refs/remotes/origin/main
  .git/objects/01/0f933fef4d29556d65cbbc93f332e897a7d836
  .git/objects/02/098a71716e3d7afdc932143063317ab98e625c
  .git/objects/0e/21917b77641ea6f26d8a74dfef140c9bf43f05
  .git/objects/14/515c06f8093d46c9dadba5a5e38342eebb3a41
  .git/objects/1d/285d20d62239428f1515f5f44955a64da83633
  .git/objects/22/8c7a87b2158cc858eae600280602ea02e6f90b
  .git/objects/24/7631141629198a79def36d2294042f06cf0b4e
  .git/objects/26/fca19e2eff238ffc2e12be5dc2a204bae8e0a2
  .git/objects/2e/01f7292b88fcc769024d694fc1dd8e495f596c
  .git/objects/32/732dabf07f528bc24e32fb4b7f0b015f20157d
  .git/objects/32/a5e26d270d46b95e93f63a0ec7136b5560f8e2
  .git/objects/35/084c8476ac94669e1f80a8534ed18de568ff68
  .git/objects/35/631eaec75c63d864314099505ee79c2576ff11
  .git/objects/39/c5f0269ec451e3183151055ed16dd1f9aa9833
  .git/objects/41/e24d34bf37f6f5ecbdfaf5dcb122605656fef1
  .git/objects/42/3ef46bb5f85a04ffbbd5840217881b319d379f
  .git/objects/43/2f32b1ed5f25004303af7a53d67cb073489545
  .git/objects/47/61cd5f8d26b87a06fc2e709ef15c4269afddfd
  .git/objects/49/bab97114fbc2a34742c3b7c6258688f0c319ba
  .git/objects/4b/94b99fbe4c162976d6742e69c94dd63192fbc8
  .git/objects/51/7e9985a4234f707e20ff6aec2ce196991954fc
  .git/objects/56/ec5bf50fc10cc5dd65957655e07300db785f2c
  .git/objects/57/198b63dd5f1d8884ac4bad7c4ed41eea15bb56
  .git/objects/59/9920427066c4d18e30ab6d48579baaa730b730
  .git/objects/5a/a1184c12db15ed4de1161ada9baa581f3ea952
  .git/objects/5a/de295b22ce532a150cede219d04c1c5b87c0c5
  .git/objects/5b/85f37b666820fc6789e36500a8a25264d284fa
  .git/objects/5e/5d7f8c6017bf41f8aab2d4b6dddc436450ef81
  .git/objects/5f/8c4511a44324a3bb2e0b68d52381ab682166fe
  .git/objects/60/00c948ca3852c784b63580855ddfd24a2fba8e
  .git/objects/69/6e0d2b94fbc09e5bf2378678cfe86625c2f15c
  .git/objects/79/8dce67e8d5175e2abad3b31cf007b0737f7403
  .git/objects/7a/06badc3d5a93db6dbdc1ac0786e9f36027dcd4
  .git/objects/7e/b8aaa7dcf576558014a1dc8d500a9e6d21c870
  .git/objects/86/0358fa1fd66ac26404ada1e9268423984981dc
  .git/objects/89/7183c53372503a17fb0321783ec78dcc5b52bd
  .git/objects/8f/171f68dc233525d7c8304b4eeaf96283915ead
  .git/objects/91/84ee2c2a44a71b7805c33fec085636582e7ad6
  .git/objects/94/0375e8218a6553f013e2b76e04cace9eea8d8a
  .git/objects/98/0bf1f4dc5aac2ba96d1039b6860b5f114f2a1e
  .git/objects/9e/48cdbea6ca8e1e6ab2c6f9d3b3d504519ba8f1
  .git/objects/a3/23e8b8daf5cdfd7f719c6d77d3a1a60d175408
  .git/objects/a8/36626f7be22e6636f493f6f37bfd567fdc871d
  .git/objects/a8/49d26fa5350a0447d55a4f8a9a54bcc2f45d40
  .git/objects/ab/3d5fa8fd7d22f2c900ad376e6cae0c090cc44f
  .git/objects/ad/48952423c08b6975cc563c69baac60b1024e62
  .git/objects/ae/5c07564541a2f6f84f1fec8fd5fd205dae3953
  .git/objects/b0/3e72732c7c1d8a2998df671c552788b7c6d3ec
  .git/objects/b6/af4ac5b2b1e5f54d720e789263f8d2dd5a829f
  .git/objects/bc/6cce105c59e7cb61a4b46d3cbbfc42939de319
  .git/objects/c7/a0147554e624be84c0ec415bea358965f1f550
  .git/objects/c9/17b0279e3a7990eaa95c9540d9a0b0cb8dfd08
  .git/objects/ca/b18d2e5d58e5996b29efbb8a7df3730f753cd1
  .git/objects/cc/6307131a5395c2ba191ae542e984645b9a870e
  .git/objects/d6/40423b8635f174075473ce6c0fe7ddf3e63b45
  .git/objects/d8/3468ba8001865edc053aaae09e3067893f77a2
  .git/objects/df/2e36040de34bd6f71d78ad41119920dd7fd554
  .git/objects/e6/2b24e41b4988b9f5a88f75b067cadd547c7c86
  .git/objects/eb/44dc6928d1b538a84a0b5fff6663588c20fcde
  .git/objects/ec/c21a22441bd8496c15b725f5c0692a007076d6
  .git/objects/ee/154b37543bda3bb146ce702bc78be977629536
  .git/objects/f5/a7f0a80a7d04b7e41a83c7516711775bb31af3
  .git/objects/fe/11f3e11f23be794a79f703617530784e33940f
  .git/objects/pack/pack-b039e4dd2d5151432844012a311727745540bc68.idx
  .git/objects/pack/pack-b039e4dd2d5151432844012a311727745540bc68.pack
  .git/objects/pack/pack-b039e4dd2d5151432844012a311727745540bc68.rev
  .git/refs/heads/main
  .git/refs/heads/replit-agent
  .git/refs/notes/commits
  .git/refs/remotes/gitsafe-backup/main
  .git/refs/remotes/origin/main
  .git/refs/replit/agent-ledger
  .git/shallow
  .gitignore
  .local/secondary_skills/LICENSE.txt
  .local/secondary_skills/ad-creative/.fingerprint
  .local/secondary_skills/ad-creative/SKILL.md
  .local/secondary_skills/ai-recruiter/.fingerprint
  .local/secondary_skills/ai-recruiter/SKILL.md
  .local/secondary_skills/ai-sdr/.fingerprint
  .local/secondary_skills/ai-sdr/SKILL.md
  .local/secondary_skills/ai-secretary/.fingerprint
  .local/secondary_skills/ai-secretary/SKILL.md
  .local/secondary_skills/branding-generator/.fingerprint
  .local/secondary_skills/branding-generator/SKILL.md
  .local/secondary_skills/competitive-analysis/.fingerprint
  .local/secondary_skills/competitive-analysis/SKILL.md
  .local/secondary_skills/content-machine/.fingerprint
  .local/secondary_skills/content-machine/SKILL.md
  .local/secondary_skills/deep-research/.fingerprint
  .local/secondary_skills/deep-research/SKILL.md
  .local/secondary_skills/design-thinker/.fingerprint
  .local/secondary_skills/design-thinker/SKILL.md
  .local/secondary_skills/excel-generator/.fingerprint
  .local/secondary_skills/excel-generator/SKILL.md
  .local/secondary_skills/excel-generator/financial-models.md
  .local/secondary_skills/file-converter/.fingerprint
  .local/secondary_skills/file-converter/SKILL.md
  .local/secondary_skills/flashcard-generator/.fingerprint
  .local/secondary_skills/flashcard-generator/SKILL.md
  .local/secondary_skills/geo/.fingerprint
  .local/secondary_skills/geo/SKILL.md
  .local/secondary_skills/geo/references/content-patterns.md
  .local/secondary_skills/geo/references/platform-notes.md
  .local/secondary_skills/geo/references/scorecard.md
  .local/secondary_skills/geo/references/technical-checklist.md
  .local/secondary_skills/github-solution-finder/.fingerprint
  .local/secondary_skills/github-solution-finder/SKILL.md
  .local/secondary_skills/infographic-builder/.fingerprint
  .local/secondary_skills/infographic-builder/SKILL.md
  .local/secondary_skills/infographic-builder/antv-syntax.md
  .local/secondary_skills/infographic-builder/react-fallback.md
  .local/secondary_skills/insurance-optimizer/.fingerprint
  .local/secondary_skills/insurance-optimizer/SKILL.md
  .local/secondary_skills/interview-prep/.fingerprint
  .local/secondary_skills/interview-prep/SKILL.md
  .local/secondary_skills/invoice-generator/.fingerprint
  .local/secondary_skills/invoice-generator/SKILL.md
  .local/secondary_skills/legal-contract/.fingerprint
  .local/secondary_skills/legal-contract/SKILL.md
  .local/secondary_skills/meal-planner/.fingerprint
  .local/secondary_skills/meal-planner/SKILL.md
  .local/secondary_skills/personal-shopper/.fingerprint
  .local/secondary_skills/personal-shopper/SKILL.md
  .local/secondary_skills/photo-editor/.fingerprint
  .local/secondary_skills/photo-editor/SKILL.md
  .local/secondary_skills/podcast-generator/.fingerprint
  .local/secondary_skills/podcast-generator/SKILL.md
  .local/secondary_skills/podcast-marketing/.fingerprint
  .local/secondary_skills/podcast-marketing/SKILL.md
  .local/secondary_skills/podcast-marketing/audio-processing.md
  .local/secondary_skills/podcast-marketing/content-atoms.md
  .local/secondary_skills/podcast-marketing/content-calendar.md
  .local/secondary_skills/podcast-marketing/content-templates.md
  .local/secondary_skills/podcast-marketing/quote-cards.md
  .local/secondary_skills/podcast-marketing/rss-and-batch.md
  .local/secondary_skills/podcast-marketing/video-clips.md
  .local/secondary_skills/podcast-marketing/youtube-processing.md
  .local/secondary_skills/product-manager/.fingerprint
  .local/secondary_skills/product-manager/SKILL.md
  .local/secondary_skills/programmatic-seo/.fingerprint
  .local/secondary_skills/programmatic-seo/SKILL.md
  .local/secondary_skills/real-estate-analyzer/.fingerprint
  .local/secondary_skills/real-estate-analyzer/SKILL.md
  .local/secondary_skills/recipe-creator/.fingerprint
  .local/secondary_skills/recipe-creator/SKILL.md
  .local/secondary_skills/recreate-screenshot/.fingerprint
  .local/secondary_skills/recreate-screenshot/SKILL.md
  .local/secondary_skills/resume-maker/.fingerprint
  .local/secondary_skills/resume-maker/SKILL.md
  .local/secondary_skills/seo-auditor/.fingerprint
  .local/secondary_skills/seo-auditor/SKILL.md
  .local/secondary_skills/skill-creator/.fingerprint
  .local/secondary_skills/skill-creator/SKILL.md
  .local/secondary_skills/skill-finder/.fingerprint
  .local/secondary_skills/skill-finder/SKILL.md
  .local/secondary_skills/stock-analyzer/.fingerprint
  .local/secondary_skills/stock-analyzer/SKILL.md
  .local/secondary_skills/storyboard/.fingerprint
  .local/secondary_skills/storyboard/SKILL.md
  .local/secondary_skills/supplier-research/.fingerprint
  .local/secondary_skills/supplier-research/SKILL.md
  .local/secondary_skills/tax-reviewer/.fingerprint
  .local/secondary_skills/tax-reviewer/SKILL.md
  .local/secondary_skills/travel-assistant/.fingerprint
  .local/secondary_skills/travel-assistant/SKILL.md
  .local/secondary_skills/video-editing/.fingerprint
  .local/secondary_skills/video-editing/SKILL.md
  .local/secondary_skills/video-editing/dead-space-and-chunking.md
  .local/secondary_skills/video-editing/operations.md
  .local/secondary_skills/video-editing/virality-scoring.md
  .local/secondary_skills/video-editing/voiceover.md
  .local/secondary_skills/website-cloning/.fingerprint
  .local/secondary_skills/website-cloning/SKILL.md
  .local/secondary_skills/website-cloning/extraction.md
  .local/secondary_skills/website-cloning/pitfalls.md
  .local/skills/LICENSE.txt
  .local/skills/agent-inbox/.fingerprint
  .local/skills/agent-inbox/SKILL.md
  .local/skills/artifacts/.fingerprint
  .local/skills/artifacts/SKILL.md
  .local/skills/artifacts/artifacts/automation/artifact.yaml
  .local/skills/artifacts/artifacts/automation/files/.gitignore
  .local/skills/artifacts/artifacts/automation/files/package.json.template
  .local/skills/artifacts/artifacts/automation/files/scripts/build.sh
  .local/skills/artifacts/artifacts/automation/files/scripts/inngest.sh
  .local/skills/artifacts/artifacts/automation/files/src/global.d.ts
  .local/skills/artifacts/artifacts/automation/files/src/mastra/agents/agent.ts
  .local/skills/artifacts/artifacts/automation/files/src/mastra/index.ts
  .local/skills/artifacts/artifacts/automation/files/src/mastra/inngest/client.ts
  .local/skills/artifacts/artifacts/automation/files/src/mastra/inngest/index.ts
  .local/skills/artifacts/artifacts/automation/files/src/mastra/storage/index.ts
  .local/skills/artifacts/artifacts/automation/files/src/mastra/tools/exampleTool.ts
  .local/skills/artifacts/artifacts/automation/files/src/mastra/workflows/workflow.ts
  .local/skills/artifacts/artifacts/automation/files/src/triggers/cronTriggers.ts
  .local/skills/artifacts/artifacts/automation/files/src/triggers/exampleConnectorTrigger.ts
  .local/skills/artifacts/artifacts/automation/files/src/triggers/slackTriggers.ts
  .local/skills/artifacts/artifacts/automation/files/src/triggers/telegramTriggers.ts
  .local/skills/artifacts/artifacts/automation/files/tests/testCronAutomation.ts
  .local/skills/artifacts/artifacts/automation/files/tests/testWebhookAutomation.ts
  .local/skills/artifacts/artifacts/automation/files/tsconfig.json
  .local/skills/artifacts/artifacts/data-visualization/artifact.yaml
  .local/skills/artifacts/artifacts/expo/OWNERS
  .local/skills/artifacts/artifacts/expo/artifact.yaml
  .local/skills/artifacts/artifacts/expo/files/.gitignore
  .local/skills/artifacts/artifacts/expo/files/app.json.template
  .local/skills/artifacts/artifacts/expo/files/app/(tabs)/_layout.tsx
  .local/skills/artifacts/artifacts/expo/files/app/(tabs)/index.tsx
  .local/skills/artifacts/artifacts/expo/files/app/+not-found.tsx
  .local/skills/artifacts/artifacts/expo/files/app/_layout.tsx
  .local/skills/artifacts/artifacts/expo/files/assets/images/icon.png
  .local/skills/artifacts/artifacts/expo/files/babel.config.js
  .local/skills/artifacts/artifacts/expo/files/components/ErrorBoundary.tsx
  .local/skills/artifacts/artifacts/expo/files/components/ErrorFallback.tsx
  .local/skills/artifacts/artifacts/expo/files/components/KeyboardAwareScrollViewCompat.tsx
  .local/skills/artifacts/artifacts/expo/files/constants/colors.ts
  .local/skills/artifacts/artifacts/expo/files/hooks/useColors.ts
  .local/skills/artifacts/artifacts/expo/files/metro.config.js
  .local/skills/artifacts/artifacts/expo/files/package.json.template
  .local/skills/artifacts/artifacts/expo/files/scripts/build.js
  .local/skills/artifacts/artifacts/expo/files/server/serve.js
  .local/skills/artifacts/artifacts/expo/files/server/templates/landing-page.html
  .local/skills/artifacts/artifacts/expo/files/tsconfig.json
  .local/skills/artifacts/artifacts/mockup-sandbox/artifact.yaml
  .local/skills/artifacts/artifacts/mockup-sandbox/files/components.json
  .local/skills/artifacts/artifacts/mockup-sandbox/files/index.html
  .local/skills/artifacts/artifacts/mockup-sandbox/files/mockupPreviewPlugin.ts
  .local/skills/artifacts/artifacts/mockup-sandbox/files/package.json.template
  .local/skills/artifacts/artifacts/mockup-sandbox/files/public/favicon.svg
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/.generated/mockup-components.ts
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/App.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/accordion.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/alert-dialog.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/alert.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/aspect-ratio.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/avatar.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/badge.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/breadcrumb.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/button-group.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/button.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/calendar.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/card.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/carousel.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/chart.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/checkbox.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/collapsible.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/command.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/context-menu.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/dialog.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/drawer.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/dropdown-menu.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/empty.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/field.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/form.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/hover-card.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/input-group.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/input-otp.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/input.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/item.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/kbd.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/label.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/menubar.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/navigation-menu.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/pagination.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/popover.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/progress.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/radio-group.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/resizable.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/scroll-area.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/select.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/separator.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/sheet.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/sidebar.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/skeleton.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/slider.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/sonner.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/spinner.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/switch.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/table.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/tabs.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/textarea.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/toast.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/toaster.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/toggle-group.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/toggle.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/components/ui/tooltip.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/hooks/use-mobile.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/hooks/use-toast.ts
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/index.css
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/lib/utils.ts
  .local/skills/artifacts/artifacts/mockup-sandbox/files/src/main.tsx
  .local/skills/artifacts/artifacts/mockup-sandbox/files/tsconfig.json
  .local/skills/artifacts/artifacts/mockup-sandbox/files/vite.config.ts
  .local/skills/artifacts/artifacts/react-vite/artifact.yaml
  .local/skills/artifacts/artifacts/react-vite/files/components.json
  .local/skills/artifacts/artifacts/react-vite/files/index.html.template
  .local/skills/artifacts/artifacts/react-vite/files/package.json.template
  .local/skills/artifacts/artifacts/react-vite/files/public/favicon.svg
  .local/skills/artifacts/artifacts/react-vite/files/src/App.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/accordion.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/alert-dialog.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/alert.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/aspect-ratio.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/avatar.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/badge.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/breadcrumb.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/button-group.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/button.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/calendar.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/card.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/carousel.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/chart.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/checkbox.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/collapsible.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/command.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/context-menu.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/dialog.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/drawer.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/dropdown-menu.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/empty.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/field.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/form.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/hover-card.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/input-group.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/input-otp.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/input.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/item.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/kbd.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/label.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/menubar.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/navigation-menu.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/pagination.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/popover.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/progress.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/radio-group.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/resizable.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/scroll-area.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/select.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/separator.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/sheet.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/sidebar.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/skeleton.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/slider.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/sonner.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/spinner.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/switch.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/table.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/tabs.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/textarea.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/toast.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/toaster.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/toggle-group.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/toggle.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/components/ui/tooltip.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/hooks/use-mobile.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/hooks/use-toast.ts
  .local/skills/artifacts/artifacts/react-vite/files/src/index.css
  .local/skills/artifacts/artifacts/react-vite/files/src/lib/utils.ts
  .local/skills/artifacts/artifacts/react-vite/files/src/main.tsx
  .local/skills/artifacts/artifacts/react-vite/files/src/pages/not-found.tsx
  .local/skills/artifacts/artifacts/react-vite/files/tsconfig.json
  .local/skills/artifacts/artifacts/react-vite/files/vite.config.ts
  .local/skills/artifacts/artifacts/slides/artifact.yaml
  .local/skills/artifacts/artifacts/slides/files/index.html.template
  .local/skills/artifacts/artifacts/slides/files/package.json.template
  .local/skills/artifacts/artifacts/slides/files/public/favicon.svg
  .local/skills/artifacts/artifacts/slides/files/scripts/validate-slides.ts
  .local/skills/artifacts/artifacts/slides/files/src/App.tsx
  .local/skills/artifacts/artifacts/slides/files/src/data/slides-manifest.json
  .local/skills/artifacts/artifacts/slides/files/src/data/slidesManifestSchema.ts
  .local/skills/artifacts/artifacts/slides/files/src/index.css
  .local/skills/artifacts/artifacts/slides/files/src/main.tsx
  .local/skills/artifacts/artifacts/slides/files/src/slideLoader.ts
  .local/skills/artifacts/artifacts/slides/files/tsconfig.json
  .local/skills/artifacts/artifacts/slides/files/vite.config.ts
  .local/skills/artifacts/artifacts/video-js/artifact.yaml
  .local/skills/artifacts/artifacts/video-js/files/index.html.template
  .local/skills/artifacts/artifacts/video-js/files/package.json.template
  .local/skills/artifacts/artifacts/video-js/files/public/favicon.svg
  .local/skills/artifacts/artifacts/video-js/files/scripts/validate-recording.sh
  .local/skills/artifacts/artifacts/video-js/files/src/App.tsx
  .local/skills/artifacts/artifacts/video-js/files/src/components/video/ReplitLoadingScene.tsx
  .local/skills/artifacts/artifacts/video-js/files/src/components/video/VideoTemplate.tsx
  .local/skills/artifacts/artifacts/video-js/files/src/components/video/index.ts
  .local/skills/artifacts/artifacts/video-js/files/src/hooks/use-mobile.tsx
  .local/skills/artifacts/artifacts/video-js/files/src/index.css
  .local/skills/artifacts/artifacts/video-js/files/src/lib/utils.ts
  .local/skills/artifacts/artifacts/video-js/files/src/lib/video/animations.ts
  .local/skills/artifacts/artifacts/video-js/files/src/lib/video/hooks.ts
  .local/skills/artifacts/artifacts/video-js/files/src/lib/video/index.ts
  .local/skills/artifacts/artifacts/video-js/files/src/main.tsx
  .local/skills/artifacts/artifacts/video-js/files/tsconfig.json
  .local/skills/artifacts/artifacts/video-js/files/vite.config.ts
  .local/skills/artifacts/bootstrap-legacy.js
  .local/skills/artifacts/bootstrap.js
  .local/skills/artifacts/references/multi-artifact-creation.md
  .local/skills/canvas/.fingerprint
  .local/skills/canvas/SKILL.md
  .local/skills/canvas/__init__.py
  .local/skills/code_review/.fingerprint
  .local/skills/code_review/SKILL.md
  .local/skills/database/.fingerprint
  .local/skills/database/SKILL.md
  .local/skills/delegation/.fingerprint
  .local/skills/delegation/SKILL.md
  .local/skills/deployment/.fingerprint
  .local/skills/deployment/SKILL.md
  .local/skills/deployment/references/deployment-logs.md
  .local/skills/design-exploration/.fingerprint
  .local/skills/design-exploration/SKILL.md
  .local/skills/design/.fingerprint
  .local/skills/design/SKILL.md
  .local/skills/diagnostics/.fingerprint
  .local/skills/diagnostics/SKILL.md
  .local/skills/environment-secrets/.fingerprint
  .local/skills/environment-secrets/SKILL.md
  .local/skills/external_apis/.fingerprint
  .local/skills/external_apis/SKILL.md
  .local/skills/external_apis/references/brave.md
  .local/skills/follow-up-tasks/.fingerprint
  .local/skills/follow-up-tasks/SKILL.md
  .local/skills/fullstack-js/.fingerprint
  .local/skills/fullstack-js/SKILL.md
  .local/skills/fullstack-js/references/hover_and_elevation.md
  .local/skills/fullstack-js/references/layout_and_spacing.md
  .local/skills/fullstack-js/references/shadcn_component_rules.md
  .local/skills/fullstack-js/references/sidebar_rules.md
  .local/skills/fullstack-js/references/visual_style_and_contrast.md
  .local/skills/integrations/.fingerprint
  .local/skills/integrations/SKILL.md
  .local/skills/media-generation/.fingerprint
  .local/skills/media-generation/SKILL.md
  .local/skills/mockup-extract/.fingerprint
  .local/skills/mockup-extract/SKILL.md
  .local/skills/mockup-graduate/.fingerprint
  .local/skills/mockup-graduate/SKILL.md
  .local/skills/mockup-sandbox/.fingerprint
  .local/skills/mockup-sandbox/SKILL.md
  .local/skills/package-management/.fingerprint
  .local/skills/package-management/SKILL.md
  .local/skills/post_merge_setup/.fingerprint
  .local/skills/post_merge_setup/SKILL.md
  .local/skills/project_tasks/.fingerprint
  .local/skills/project_tasks/SKILL.md
  .local/skills/query-integration-data/.fingerprint
  .local/skills/query-integration-data/SKILL.md
  .local/skills/remove-image-background/.fingerprint
  .local/skills/remove-image-background/SKILL.md
  .local/skills/repl_setup/.fingerprint
  .local/skills/repl_setup/SKILL.md
  .local/skills/repl_setup/references/angular.md
  .local/skills/repl_setup/references/react_vite.md
  .local/skills/repl_setup/references/vue.md
  .local/skills/replit-docs/.fingerprint
  .local/skills/replit-docs/SKILL.md
  .local/skills/revenuecat/.fingerprint
  .local/skills/revenuecat/SKILL.md
  .local/skills/revenuecat/references/initial-setup.md
  .local/skills/revenuecat/references/replit-revenuecat-sdk-docs.md
  .local/skills/revenuecat/references/subsequent-management.md
  .local/skills/security_scan/.fingerprint
  .local/skills/security_scan/SKILL.md
  .local/skills/skill-authoring/.fingerprint
  .local/skills/skill-authoring/SKILL.md
  .local/skills/stripe/.fingerprint
  .local/skills/stripe/SKILL.md
  .local/skills/stripe/references/code-templates.md
  .local/skills/suggest-new-project/.fingerprint
  .local/skills/suggest-new-project/SKILL.md
  .local/skills/threat_modeling/.fingerprint
  .local/skills/threat_modeling/SKILL.md
  .local/skills/validation/.fingerprint
  .local/skills/validation/SKILL.md
  .local/skills/web-search/.fingerprint
  .local/skills/web-search/SKILL.md
  .local/skills/workflows/.fingerprint
  .local/skills/workflows/SKILL.md
  .local/state/replit/agent/.agent_state_010f933fef4d29556d65cbbc93f332e897a7d836.bin
  .local/state/replit/agent/.agent_state_14515c06f8093d46c9dadba5a5e38342eebb3a41.bin
  .local/state/replit/agent/.agent_state_228c7a87b2158cc858eae600280602ea02e6f90b.bin
  .local/state/replit/agent/.agent_state_432f32b1ed5f25004303af7a53d67cb073489545.bin
  .local/state/replit/agent/.agent_state_5b85f37b666820fc6789e36500a8a25264d284fa.bin
  .local/state/replit/agent/.agent_state_6000c948ca3852c784b63580855ddfd24a2fba8e.bin
  .local/state/replit/agent/.agent_state_980bf1f4dc5aac2ba96d1039b6860b5f114f2a1e.bin
  .local/state/replit/agent/.agent_state_ae5c07564541a2f6f84f1fec8fd5fd205dae3953.bin
  .local/state/replit/agent/.agent_state_b03e72732c7c1d8a2998df671c552788b7c6d3ec.bin
  .local/state/replit/agent/.agent_state_cc6307131a5395c2ba191ae542e984645b9a870e.bin
  .local/state/replit/agent/.agent_state_f5a7f0a80a7d04b7e41a83c7516711775bb31af3.bin
  .local/state/replit/agent/.agent_state_main.bin
  .local/state/replit/agent/.latest.json
  .local/state/replit/agent/progress_tracker.md
  .local/state/replit/agent/repl_state.bin
  .local/state/replit/log-query.db
  .local/state/replit/log-query.db-shm
  .local/state/replit/log-query.db-wal
  .local/state/scribe/scribe.db
  .local/state/scribe/scribe.db-shm
  .local/state/scribe/scribe.db-wal
  .local/state/workflow-logs/55Gr7v8DXu5ewWUWfs4Lq/metadata.json
  .local/state/workflow-logs/55Gr7v8DXu5ewWUWfs4Lq/start_application.shell.exec.0
  .local/state/workflow-logs/5cDC29B7tJw5XXbBOrhWh/metadata.json
  .local/state/workflow-logs/5cDC29B7tJw5XXbBOrhWh/start_application.shell.exec.0
  .local/state/workflow-logs/E1ZL-IAPLGApOqirZ4sJY/metadata.json
  .local/state/workflow-logs/GtNudELQEcgARdYMZXL2U/metadata.json
  .local/state/workflow-logs/HPbCVcItFOa3mfeJFK8kf/metadata.json
  .local/state/workflow-logs/Ij6htOPNrryT22iN66-TE/metadata.json
  .local/state/workflow-logs/Ij6htOPNrryT22iN66-TE/start_application.shell.exec.0
  .local/state/workflow-logs/Jg0_YczQpCvNyu5SPmfpI/metadata.json
  .local/state/workflow-logs/Jg0_YczQpCvNyu5SPmfpI/start_application.shell.exec.0
  .local/state/workflow-logs/Kr4Rl61IQpvtOMDRHcc0d/metadata.json
  .local/state/workflow-logs/Kr4Rl61IQpvtOMDRHcc0d/start_application.shell.exec.0
  .local/state/workflow-logs/LN8Ypo2mUdcuyqFhIh6Fl/metadata.json
  .local/state/workflow-logs/LbZi5kZQB7Ym_CrpUVI_H/metadata.json
  .local/state/workflow-logs/LbZi5kZQB7Ym_CrpUVI_H/start_application.shell.exec.0
  .local/state/workflow-logs/Pw0Qq6gHq3cQ4SWSW6oQB/metadata.json
  .local/state/workflow-logs/SQjKh0Fh_-kO7G-0Vi5bG/metadata.json
  .local/state/workflow-logs/SQjKh0Fh_-kO7G-0Vi5bG/start_application.shell.exec.0
  .local/state/workflow-logs/Ujr1I1TrA5ofTdJDo9VZP/metadata.json
  .local/state/workflow-logs/Ujr1I1TrA5ofTdJDo9VZP/start_application.shell.exec.0
  .local/state/workflow-logs/X8A4VPXQihbRxTi8hznz4/metadata.json
  .local/state/workflow-logs/X8A4VPXQihbRxTi8hznz4/start_application.shell.exec.0
  .local/state/workflow-logs/hWQEAm0pGU0QvTGg2KeoI/metadata.json
  .local/state/workflow-logs/naLrCNUov5fD0PtVxdPdU/metadata.json
  .local/state/workflow-logs/naLrCNUov5fD0PtVxdPdU/start_application.shell.exec.0
  .local/state/workflow-logs/pITQDUoOlG2F1v9qoRwHb/metadata.json
  .local/state/workflow-logs/tljoQIkZd--W9BtSbS0aX/metadata.json
  .local/state/workflow-logs/tljoQIkZd--W9BtSbS0aX/start_application.shell.exec.0
  .local/state/workflow-logs/x7K8OcA4UDDBilTnmKtwZ/metadata.json
  .local/state/workflow-logs/zMCgmyyArMsumYNVrbt1S/metadata.json
  .replit
  MANUAL_APK_ANDROID.md
  MANUAL_APK_ORIENTADO.md
  PLANO.md
  README.md
  RELATORIO_CORRECOES.md
  SECURITY.md
  api/index.ts
  client/index.html
  client/public/auditoria.html
  client/public/codigo-formatacao.txt
  client/public/comparador.html
  client/public/favicon.png
  client/public/icon-192.png
  client/public/icon-512.png
  client/public/manifest.json
  client/public/sw.js
  client/replit_integrations/audio/audio-playback-worklet.js
  client/replit_integrations/audio/audio-utils.ts
  client/replit_integrations/audio/index.ts
  client/replit_integrations/audio/useAudioPlayback.ts
  client/replit_integrations/audio/useVoiceRecorder.ts
  client/replit_integrations/audio/useVoiceStream.ts
  client/src/App.tsx
  client/src/components/pwa-install.tsx
  client/src/components/theme-provider.tsx
  client/src/components/theme-toggle.tsx
  client/src/components/tiptap-editor.tsx
  client/src/components/ui/accordion.tsx
  client/src/components/ui/alert-dialog.tsx
  client/src/components/ui/alert.tsx
  client/src/components/ui/aspect-ratio.tsx
  client/src/components/ui/avatar.tsx
  client/src/components/ui/badge.tsx
  client/src/components/ui/breadcrumb.tsx
  client/src/components/ui/button.tsx
  client/src/components/ui/calendar.tsx
  client/src/components/ui/card.tsx
  client/src/components/ui/carousel.tsx
  client/src/components/ui/chart.tsx
  client/src/components/ui/checkbox.tsx
  client/src/components/ui/collapsible.tsx
  client/src/components/ui/command.tsx
  client/src/components/ui/context-menu.tsx
  client/src/components/ui/dialog.tsx
  client/src/components/ui/drawer.tsx
  client/src/components/ui/dropdown-menu.tsx
  client/src/components/ui/form.tsx
  client/src/components/ui/hover-card.tsx
  client/src/components/ui/input-otp.tsx
  client/src/components/ui/input.tsx
  client/src/components/ui/label.tsx
  client/src/components/ui/menubar.tsx
  client/src/components/ui/navigation-menu.tsx
  client/src/components/ui/pagination.tsx
  client/src/components/ui/popover.tsx
  client/src/components/ui/progress.tsx
  client/src/components/ui/radio-group.tsx
  client/src/components/ui/resizable.tsx
  client/src/components/ui/scroll-area.tsx
  client/src/components/ui/select.tsx
  client/src/components/ui/separator.tsx
  client/src/components/ui/sheet.tsx
  client/src/components/ui/sidebar.tsx
  client/src/components/ui/skeleton.tsx
  client/src/components/ui/slider.tsx
  client/src/components/ui/switch.tsx
  client/src/components/ui/table.tsx
  client/src/components/ui/tabs.tsx
  client/src/components/ui/textarea.tsx
  client/src/components/ui/toast.tsx
  client/src/components/ui/toaster.tsx
  client/src/components/ui/toggle-group.tsx
  client/src/components/ui/toggle.tsx
  client/src/components/ui/tooltip.tsx
  client/src/hooks/use-mobile.tsx
  client/src/hooks/use-toast.ts
  client/src/index.css
  client/src/lib/queryClient.ts
  client/src/lib/utils.ts
  client/src/main.tsx
  client/src/pages/auditoria-financeira.tsx
  client/src/pages/code-assistant.tsx
  client/src/pages/comparador-juridico.tsx
  client/src/pages/comunicacoes-cnj.tsx
  client/src/pages/consulta-corporativo.tsx
  client/src/pages/consulta-pdpj.tsx
  client/src/pages/consulta-processual.tsx
  client/src/pages/filtrador.tsx
  client/src/pages/jurisprudencia.tsx
  client/src/pages/legal-assistant.tsx
  client/src/pages/legal-assistant.tsx.recovered
  client/src/pages/login.tsx
  client/src/pages/not-found.tsx
  client/src/pages/painel-processos.tsx
  client/src/pages/playground.tsx
  client/src/pages/previdenciario.tsx
  client/src/pages/robo-djen.tsx
  client/src/pages/token-generator.tsx
  client/src/pages/tramitacao.tsx
  components.json
  drizzle.config.ts
  fix_buttons.txt
  main.py
  migrations/0000_init.sql
  migrations/meta/0000_snapshot.json
  migrations/meta/_journal.json
  novo 1.zip
  package-lock.json
  package.json
  postcss.config.js
  public/auditoria.html
  pyproject.toml
  replit.md
  script/build.ts
  server/db.ts
  server/djen.ts
  server/index.ts
  server/replit_integrations/audio/client.ts
  server/replit_integrations/audio/index.ts
  server/replit_integrations/audio/routes.ts
  server/replit_integrations/batch/index.ts
  server/replit_integrations/batch/utils.ts
  server/replit_integrations/chat/index.ts
  server/replit_integrations/chat/routes.ts
  server/replit_integrations/chat/storage.ts
  server/replit_integrations/image/client.ts
  server/replit_integrations/image/index.ts
  server/replit_integrations/image/routes.ts
  server/routes.ts
  server/static.ts
  server/storage.ts
  server/vite.ts
  shared/models/chat.ts
  shared/schema.ts
  tailwind.config.ts
  tsconfig.json
  uv.lock
  vite.config.ts
```

---

*Plano gerado pelo SK Code Editor — 20/04/2026, 03:11:22*