# PAYEZ MIEUX, GARDEZ VOS MEILLEURS

Business web « stratégie salariale pour dirigeants de PME » — le playbook qui transforme la masse salariale en avantage stratégique.

## Contenu du livrable

| Fichier | Rôle |
|---|---|
| `index.html` | Landing page (bleu roi / or / ivoire, « business premium ») : hero 90k/55k, 3 arguments, 6 chapitres, 3 offres, formulaire EmailJS |
| `playbook-payer-mieux.md` | Le playbook complet (~40 pages) : 6 chapitres (leçon dense + exemple chiffré réel + exercice), conclusion (10 règles d'or), annexes (checklist d'audit, glossaire, repères de salaires) |
| `templates/grille-salariale.md` | Grille salariale vierge : repères marché, échelons, positionnement, budget, revue semestrielle |
| `templates/calcul-cout-remplacement.md` | Calculateur du coût de remplacement : les 6 composantes (recrutement, intégration, productivité, erreurs, opportunité, collectif) |
| `templates/argumentaire-augmentation.md` | Argumentaire d'une page : valeur, risque, comparaison chiffrée, objections anticipées |
| `templates/processus-progression.md` | Processus de progression : échelons, critères de passage, revue annuelle |
| `templates/entretien-retention.md` | Guide d'entretien de rétention : questions, grille d'analyse des 5 leviers, erreurs à éviter |
| `README.md` | Ce fichier |

## Offres (prix affichés sur la page)

- **Le Playbook — 27 € TTC** : playbook complet, ~40 pages, 6 chapitres.
- **Playbook + 5 Templates — 47 € TTC** : playbook + les 5 templates modifiables.
- **Pack Direction — 97 € TTC** : playbook + templates + grille salariale personnalisée (livrée sous 72 h ouvrées, via le formulaire EmailJS).

## Commande — EmailJS (réel, zéro simulateur)

- `serviceId` : `service_cy1ytdb`
- `templateId` : `template_xpo58cv`
- `publicKey` : `8Pui4ZEqxW2jRVF7h`
- Payload envoyé par le formulaire `#contactForm` : `{ site, name, email, question }` (site = `payer-mieux`, champ caché).
- Paiement documenté : virement ou message direct après échange (Stripe en attente). Réponse sous 24 h ouvrées.

## Design

Palette « business premium » distincte : fond ivoire `#fbf8f2`, bleu roi `#1e3a8a`, or `#d4a017`. Typographie Playfair Display (serif) + Source Sans 3. Monogramme « PM », filets or, coins d'or sur les cartes, registre salarial 90k/55k dans le hero. Responsive, aucune image externe (100 % CSS).

## Déploiement

Site statique, zéro dépendance serveur (EmailJS côté client). Ne pas publier sur GitHub sans instruction explicite. Pour tester localement : `python3 -m http.server` dans ce dossier, puis ouvrir `http://localhost:8000`.

## Vérification rapide

```bash
grep -c "service_cy1ytdb" index.html      # doit renvoyer 1 (câblage EmailJS)
grep -c "template_xpo58cv" index.html     # doit renvoyer 1
grep -c "8Pui4ZEqxW2jRVF7h" index.html    # doit renvoyer 1 (init)
```
