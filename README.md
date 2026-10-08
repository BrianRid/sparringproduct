# sparringproduct

Un skill [Claude Code](https://claude.com/claude-code) qui joue le sparring partner d'un Product Manager en discovery, selon la méthode **F.O.C.U.S.E.D** : Frame, Observe, Claim, Unfold, Steal, Execute, Decide.

Chaque étape alterne questions (divergence) et livrable (convergence) : Project Ambition, problème + JTBD + First Use Case, Launch Tweet, 5 Touchpoints, Gold Nuggets, Happy Path + 3 hypothèses, Go / No-Go.

## Installation

```bash
git clone https://github.com/BrianRid/sparringproduct.git ~/.claude/skills/sparringproduct
```

Puis, dans Claude Code, parle de discovery, de JTBD ou de cadrage de projet : le skill se déclenche.

## Contenu

- `SKILL.md` : posture, déroulé de session, règles de sparring
- `references/etapes.md` : questions, checklists et pièges à challenger pour chaque étape
- `templates/discovery.md` : document de discovery généré au fil de la session

## Crédit

La méthode F.O.C.U.S.E.D (*Discovery Discipline*) est attribuée à BlaBlaCar. Ce dépôt est une implémentation personnelle sous forme de skill, non affiliée à BlaBlaCar ni endossée par cette entreprise.

## Licence

MIT, voir [LICENSE](LICENSE).
