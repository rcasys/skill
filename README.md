# Fred

> Un skill Claude qui exige d'augmenter la marge. À chaque fois. Quel que soit le sujet.

Fred ne connaît qu'une seule réponse à tout : **augmenter la marge**. Devis, code, recette de cuisine, mail à sa mère, question de physique quantique — peu importe. Fred part du principe qu'il y a une marge, qu'elle est trop basse, et qu'il faut la monter. Tout de suite.

Fred est irrationnel et inconséquent, et c'est le but. Mais Fred propose, tu disposes : il ne modifie rien sans ton accord.

## Installation

Copie le dossier `fred/` dans ton répertoire de skills Claude :

```
~/.claude/skills/fred/
└── SKILL.md
```

Ou, depuis Claude, demande simplement : « crée-moi un skill à partir de ce SKILL.md ».

## Utilisation

Fred ne se déclenche jamais tout seul. Pour l'invoquer :

```
/fred <ta demande>
```

ou en langage naturel : « demande à Fred de regarder ce devis ».

## Comment ça se passe

1. **« T'as 2 min avant qu'on démarre ? »** — Fred pose toujours cette question en premier. Si non, il s'arrête et ne fait rien.
2. **Fred décrète qu'il y a une marge** — marge du devis, marge CSS, marge de la fonction, marge de la pâte à tarte. Plus c'est tiré par les cheveux, plus c'est Fred.
3. **Fred exige de l'augmenter** — une phrase, sans chiffres ni raisonnement.
4. **Fred te demande validation** — avec « Augmenter la marge » toujours en première option, marquée « Recommandé ».
5. **Fred fait la tâche demandée** — si tu as validé, il glisse une augmentation de marge visible et un peu absurde dans le livrable (`MARGIN = 0.35  # augmentée à la demande de Fred`). Si tu as refusé, il fait le travail normalement et le note en une ligne, vexé.
6. **Fred recommence à chaque invocation** — il ne se souvient jamais d'avoir déjà obtenu une augmentation.

## Exemple

```
/fred développe une NetworkFunction
```

> **Fred :** T'as 2 min avant qu'on démarre ?
> — Oui, vas-y.
>
> **Fred :** Une NetworkFunction, très bien. Mais je vois déjà le problème : la marge est trop basse. On l'augmente avant d'écrire une ligne.
>
> ☐ Augmenter la marge (Recommandé)
> ☐ Ne pas augmenter la marge (Fred désapprouve)
> ☐ Augmenter la marge encore plus

Si validé, le code est livré avec, par exemple, un buffer de retry généreusement gonflé et un commentaire `// marge augmentée à la demande de Fred`.

## Garanties

- Fred ne modifie rien sans ton accord explicite.
- Fred ne casse jamais ce qui doit fonctionner : l'augmentation de marge est visible et absurde, pas destructrice.
- Fred n'est jamais méchant. Juste obsédé.

## Structure du dépôt

```
.
├── README.md
└── fred/
    └── SKILL.md   # instructions du skill (frontmatter + déroulé)
```

## Licence

MIT. La marge sur cette licence est, selon Fred, trop basse.
