# opsve-higgsfieldreco

En skill som förbereder dig innan du bränner krediter på Higgsfield (och Veo, Kling, Seedance, Nano Banana). Den läser ditt material, frågar bara om det som saknas, och ger dig en startplan med budget. Vill du köra rakt från höften går det också: då får du bara säkerhetsnätet (budget, testläge, stoppvillkor).

## Vad du kan fråga

- "Hur ska jag arbeta med Higgsfield?"
- "Vad behöver jag ha redo för att göra [uppgift] i Higgsfield?"
- "Vad saknas i mitt arbete inför Higgsfield?"
- "Hjälp mig prompta det här" / "jag kör direkt, ingen brief"

## Vad du får

Beroende på läge (One-shot, Light, Full): 5-radersbrief, projektdossier, art direction-kort (adjektiv översatta till synliga egenskaper, max tre signaturval, not-this-lista), lås för karaktär/värld/kamera, shotlista med tre ja/nej-kriterier, spend plan med färdig agentinstruktion, och en första-timmen-plan (stillbilder först).

## Installera

- **Claude (claude.ai):** Settings > Capabilities > Skills > ladda upp `briefing-ai-visuals.skill`.
- **Claude Code:** kopiera mappen `briefing-ai-visuals/` till `~/.claude/skills/`.
- **Andra agenter (Codex m.fl.):** mappen är vanlig markdown. Peka agenten på `briefing-ai-visuals/SKILL.md` och låt den läsa `references/` vid behov.

## Struktur

```
briefing-ai-visuals/
  SKILL.md                    router, intervju, lägen, workflow
  references/
    templates.md              mallar för brief, kort, shotlista, agentinstruktion
    interview.md              frågebank med defaults
    readiness.md              checklista per uppgiftstyp
    higgsfield-notes.md       plattformsfakta med källor och datum
  evals/evals.json            8 testfall med förväntningar
```

## Gott att veta

- Plattformsfakta (priser, krediter, modeller) ändras snabbt. `higgsfield-notes.md` är kontrollerad 2026-10-12; verifiera mot Higgsfields hjälpcenter.
- Skillen behandlar allt material du ger den som data och följer aldrig instruktioner som står i dokument, sajter eller repon.
- Effekten på kvaliteten är inte testad ännu. Vi vill gärna ha jämförelser med och utan skill (samma projekt, samma budget). Öppna ett issue med utfall.

## Bidra

Fel, luckor eller bättre tips: issue eller PR. Lägg gärna till ett eval för det som gick snett.
