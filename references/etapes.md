# Les 7 étapes F.O.C.U.S.E.D — guide de sparring

Chaque section contient : objectif, format du livrable, questions (à poser 1-2 à la fois, dans l'ordre, en sautant celles déjà couvertes), checklist de validation, pièges à challenger.

---

## F — FRAME → Project Ambition

**Objectif** : commencer par la fin. Définir à quoi ressemble le succès avant de parler de solution.

**Format**
> D'ici **[timebox]**, faire passer **[indicateur]** de **[valeur actuelle]** à **[cible]**, sans dégrader **[garde-fou]** au-delà de **[seuil acceptable]**.

Les 3 dimensions :
1. **Critère de succès** : un indicateur, sa valeur actuelle, sa cible.
2. **Damage control** : les dommages collatéraux acceptables (quels indicateurs ne doivent pas bouger, jusqu'où on tolère une dégradation, quels risques on accepte).
3. **Timebox** : le temps alloué au projet (discovery + delivery, ou discovery seule — préciser). Convertis une durée en date de fin, et si discovery + delivery sont cumulées, fais fixer une date de Go/No-Go intermédiaire.

**Questions**
- Pourquoi ce projet maintenant ? Qui l'a demandé, et qu'attend-il ?
- Si c'est un succès à la fin du timebox, qu'est-ce qui a changé ? Quel chiffre le montre ?
- Si le PM n'a que des mots vagues ("engagement", "satisfaction") : propose 2-3 indicateurs contrastés liés au problème et fais choisir.
- Comment est défini précisément cet indicateur (périmètre, fenêtre de temps) ?
- Quelle est la valeur actuelle de cet indicateur ? D'où vient-elle ?
- Quelle cible serait un succès ? Et un échec ? Pourquoi ce niveau ?
- Qu'est-ce qu'on n'a pas le droit de casser en chemin (revenu, NPS, charge support, perf, autre équipe) ? Jusqu'à quel point ?
- Combien de temps l'entreprise est prête à investir avant de décider ? Qu'est-ce qui se passe à la fin du timebox ?

**Checklist**
- [ ] Un seul indicateur principal (pas une liste)
- [ ] Valeur actuelle chiffrée et source connue (ou action pour l'obtenir)
- [ ] Cible chiffrée et justifiée (calcul d'impact, benchmark, historique, ou objectif imposé — à dire explicitement)
- [ ] Au moins un garde-fou avec seuil
- [ ] Timebox daté (date de fin + jalon Go/No-Go si discovery et delivery cumulées)
- [ ] Si une solution a été apportée d'entrée : le lien causal "solution → indicateur" est noté comme hypothèse

**Pièges à challenger**
- Indicateur d'output ("livrer la feature X") au lieu d'outcome ("taux de conversion").
- Indicateur non mesurable aujourd'hui sans plan pour le mesurer.
- "On verra" sur le timebox → sans timebox, la discovery ne s'arrête jamais.

---

## O — OBSERVE → Problème utilisateur + JTBD + First Use Case

**Objectif** : *drastic reductionism*. Identifier **LE** problème d'**UN** utilisateur, et ignorer volontairement les cas secondaires. Éviter le "grand écart" : un produit qui répond à moitié à plusieurs problèmes.

**Format**

*Problème utilisateur*
> **[Persona précis]** a du mal à **[tâche]** quand **[situation]**, parce que **[cause]**. Aujourd'hui il/elle **[contournement actuel]**, ce qui lui coûte **[impact : temps, argent, stress…]**.

*Job to be Done* (un principal, éventuellement dimensions émotionnelle/sociale)
> Quand **[situation déclencheuse]**, je veux **[motivation / progrès recherché]**, pour **[résultat attendu]**.

*First Use Case*
> Le premier cas d'usage qu'on adresse : **[persona]** qui **[situation]** et veut **[job]**. On ignore volontairement : **[cas écartés]**.

**Questions**
- Qui, précisément, a ce problème ? Décris une personne réelle que tu as observée ou interviewée.
- Raconte la dernière fois où elle a rencontré ce problème. Que s'est-il passé, étape par étape ?
- Que fait-elle aujourd'hui pour s'en sortir ? Qu'est-ce que ça lui coûte ?
- Qu'est-ce qui déclenche le besoin (le moment "quand…") ?
- Quel progrès cherche-t-elle vraiment, au-delà de la feature qu'elle demande ?
- Comment tu sais tout ça : interviews (combien ?), data, tickets support, intuition ?
- Parmi tous les cas d'usage évoqués, lequel est le plus fréquent / douloureux / lié à l'indicateur du Frame ? Lequel accepte-t-on d'abandonner pour l'instant ?
- Si tu n'as pas assez observé : qui peux-tu interviewer ou observer cette semaine ? (propose un guide d'entretien de 5-6 questions ouvertes sur le passé, pas sur le futur)

**Checklist**
- [ ] Le problème ne contient aucune solution ("il manque un bouton X" = solution)
- [ ] Un persona précis, pas "les utilisateurs"
- [ ] Au moins une preuve observée (verbatim, data, observation) — sinon noté comme hypothèse
- [ ] JTBD au format Quand / je veux / pour, sans mention de produit
- [ ] Un seul First Use Case, et les cas écartés sont listés
- [ ] Le First Use Case est cohérent avec l'indicateur du Frame

**Pièges à challenger**
- Solution déguisée en problème.
- Garder 3 use cases "parce qu'ils sont tous importants" → demander lequel on sacrifie.
- Preuves basées sur ce que les utilisateurs *disent qu'ils feraient* plutôt que sur ce qu'ils *ont fait*.

---

## C — CLAIM → Launch Tweet

**Objectif** : écrire la promesse **avant** de construire. Le tweet sert de filtre pour toutes les étapes suivantes : tout ce qui ne sert pas la promesse sort du scope. C'est une promesse qu'il faudra tenir. Impliquer le product marketing dès maintenant.

**Format**
> Tweet de lancement, **≤ 280 caractères**, écrit comme si le produit sortait aujourd'hui, adressé au persona du First Use Case.

**Questions**
- Si tu annonçais la sortie demain, que dirais-tu au persona en une phrase ?
- Quel bénéfice ressent-il, dans ses mots à lui (reprends les verbatims d'Observe) ?
- Qu'est-ce qui rend ça différent de son contournement actuel ?
- Est-ce qu'il le partagerait / le retweeterait ? Pourquoi ?
- Qui côté marketing devrait relire ce tweet ?

**Checklist**
- [ ] ≤ 280 caractères (compte-les et donne le total)
- [ ] Parle au persona du First Use Case
- [ ] Exprime un bénéfice / un progrès, pas une liste de features
- [ ] Cohérent avec le JTBD
- [ ] Promesse tenable dans le timebox

**Pièges à challenger**
- Jargon interne, nom de feature, "nouvelle fonctionnalité permettant de…".
- Promesse trop large qui réintroduit les use cases écartés.
- Proposer 2-3 variantes contrastées (bénéfice rationnel / émotionnel / social) si le PM bloque.

---

## U — UNFOLD → 5 Touchpoints

**Objectif** : choisir les 5 moments clés de l'expérience où la promesse se joue. Produit **et** hors produit : email, notification push, homepage, page de confirmation, support, communication, etc.

**Format** (tableau)

| # | Moment du parcours | Canal / surface | Ce que l'utilisateur doit comprendre ou ressentir | Lien avec la promesse |
|---|---|---|---|---|

**Questions**
- Déroule le parcours du persona du déclencheur jusqu'au résultat attendu : avant, pendant, après.
- Où découvre-t-il qu'il existe une solution ? Où l'active-t-il ? Où constate-t-il le bénéfice ? Où revient-il ?
- Quels points de contact hors produit comptent (email, notif, support, bouche-à-oreille) ?
- Si tu ne pouvais soigner que 5 moments, lesquels ? Lequel est le "moment de vérité" où la promesse du tweet est tenue ou trahie ?
- Quels touchpoints existent déjà et lesquels sont à créer ?

**Checklist**
- [ ] Exactement 5 touchpoints (pas 12)
- [ ] Couvre le parcours du déclencheur au bénéfice
- [ ] Au moins un touchpoint hors produit envisagé
- [ ] Le moment de vérité est identifié
- [ ] Chaque touchpoint sert la promesse du Claim

**Pièges à challenger**
- Lister les écrans de l'app au lieu des moments vécus par l'utilisateur.
- Oublier l'après (confirmation, retour, rétention).

---

## S — STEAL → Gold Nuggets

**Objectif** : "Les bons artistes copient, les grands artistes volent." Ne pas réinventer : repérer comment d'autres équipes (concurrents directs, indirects, autres secteurs) ont résolu des problèmes similaires, en priorité sur les 5 touchpoints.

**Format** (tableau, 1 à 3 pépites par touchpoint)

| Touchpoint | Référence (produit / entreprise) | Type (direct / indirect / autre secteur) | Ce qu'on vole | Pourquoi ça marche | Adaptation chez nous |
|---|---|---|---|---|---|

**Questions**
- Qui sont les concurrents directs ? Comment traitent-ils ce problème ? Qu'ont-ils raté ?
- Que fait le persona aujourd'hui à la place (Excel, WhatsApp, un humain…) ? C'est ton vrai concurrent.
- Quel autre secteur vit le même type de moment (attente, confiance, choix complexe, première utilisation…) ? Qui le fait remarquablement bien ?
- Pour chaque touchpoint : quelle est la meilleure expérience de ce type que tu aies vécue, tous produits confondus ?
- Qu'est-ce qui, précisément, fait que ça marche (pattern, wording, timing, mécanique) ?
- Qu'est-ce qui ne se transpose pas chez nous, et pourquoi ?

Si la recherche web est disponible : propose des références par touchpoint avec leur source, marquées comme pistes à valider par le PM.

**Checklist**
- [ ] Au moins une pépite par touchpoint (ou touchpoint explicitement sans référence)
- [ ] Au moins une référence hors secteur
- [ ] Chaque pépite décrit un mécanisme précis, pas juste un nom ("comme Airbnb")
- [ ] L'adaptation est explicite

**Pièges à challenger**
- Benchmark limité aux concurrents directs → on copie la moyenne du marché.
- Benchmark "catalogue" de features sans lien avec les touchpoints.

---

## E — EXECUTE → Happy Path + 3 hypothèses

**Objectif** : "Les briques sont là, il faut les assembler." Construire un prototype du parcours idéal qui traverse les 5 touchpoints avec les gold nuggets, et expliciter les 3 hypothèses principales dont dépend le succès. Le but est d'augmenter le niveau de confiance, pas de faire joli.

**Format**

*Happy Path* : séquence numérotée d'étapes / écrans, du déclencheur au bénéfice, chaque étape rattachée à un touchpoint.

*3 hypothèses*
> Nous croyons que **[hypothèse]**. Nous saurons que c'est vrai si **[signal observable et seuil]** lors du test.

**Questions**
- Déroule le parcours idéal, sans cas d'erreur, écran par écran ou moment par moment.
- Où interviennent les gold nuggets ?
- Quel niveau de fidélité suffit pour tester (papier, Figma cliquable, no-code, concierge / Wizard of Oz) ? Qu'est-ce qui est faisable dans le timebox restant ?
- Qu'est-ce qui doit absolument être vrai pour que ça marche (désirabilité, compréhension, utilisabilité, faisabilité, valeur business) ?
- Parmi toutes ces suppositions, lesquelles sont les plus risquées et les moins prouvées ? Garde les 3.

**Checklist**
- [ ] Le happy path couvre les 5 touchpoints
- [ ] Le prototype est testable par un vrai utilisateur
- [ ] Exactement 3 hypothèses, les plus risquées
- [ ] Chaque hypothèse a un signal observable et un seuil

**Pièges à challenger**
- Prototyper les cas limites avant le cas nominal.
- Hypothèses non falsifiables ("les utilisateurs vont aimer").
- Sur-investir en fidélité.

---

## D — DECIDE → Go / No-Go

**Objectif** : évaluer la solidité de la solution et décider de passer en delivery. Outil privilégié : tests d'utilisabilité. Le but est de dérisquer la mise en production.

**Format**

- **Protocole** : nombre d'utilisateurs (≈ 5 par profil), profil recruté (= persona du First Use Case), scénario de test, critères de Go **fixés avant le test**.
- **Résultats** par hypothèse : validée / invalidée / incertaine, avec preuves (verbatims, taux de réussite).
- **Décision** : **Go** (delivery) / **Itérer** (revenir à l'étape X, pourquoi) / **No-Go** (arrêter, ce qu'on a appris).
- **Risques restants** et comment ils seront suivis en delivery (lien avec l'indicateur et les garde-fous du Frame).

**Questions**
- Avant le test : qu'est-ce qui te ferait dire Go ? Et No-Go ? (à écrire maintenant)
- Qui recrutes-tu ? Correspondent-ils au persona ?
- Quel scénario donnes-tu, sans guider l'utilisateur ?
- Après le test : pour chaque hypothèse, qu'as-tu observé (pas interprété) ?
- Le résultat attendu sur l'indicateur du Frame reste-t-il crédible ?
- Si c'est Itérer : quelle étape reprendre (souvent Observe ou Unfold) et avec quel timebox ?

**Checklist**
- [ ] Critères de Go écrits avant les résultats
- [ ] Testeurs = persona du First Use Case
- [ ] Chaque hypothèse a un verdict fondé sur des observations
- [ ] Décision explicite (Go / Itérer / No-Go) et assumée par le PM
- [ ] Les risques restants sont reliés aux garde-fous du Frame

**Pièges à challenger**
- Décider Go par engagement émotionnel / coût déjà investi.
- Déplacer les critères après avoir vu les résultats.
- Tester avec des collègues au lieu du persona.
