# 🎯 sacado-auto-validator

![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Browser](https://img.shields.io/badge/Browser-Console-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**Auto-valide tes exercices Sacado en un copier-coller.**

Colle le script dans la console, il s'occupe du reste. Pas de serveur, pas d'install, zéro dépendance externe.

---

## ⚡ Usage rapide

1. Ouvre ta page de cours Sacado
2. `F12` → onglet **Console**
3. Colle le script, appuie sur `Entrée`
4. Regarde les logs passer en vert

---

## 🔧 Ce que ça fait concrètement

- **Nettoie** les iframes existantes sur la page
- **Détecte** automatiquement tous les liens d'exercices Sacado
- **Charge** chaque exo dans un iframe caché
- **Attend** 3 secondes le chargement complet
- **Falsifie** le temps de travail (entre 2 et 6 min aléatoirement)
- **Envoie** la validation via le système AJAX natif de Sacado
- **Supprime** l'iframe proprement après chaque envoi

| Champ modifié | Valeur injectée |
|---|---|
| `start_time` | Heure reculée de 2 à 6 min |
| `numexo` | Situation + 2 |
| `score` | `1` (100%) |
| `reponse` | `"automatique"` |

---

## 📋 Prérequis

- Être connecté à Sacado
- Un navigateur moderne (Chrome, Firefox, Edge...)
- jQuery dispo sur les pages cibles (c'est déjà le cas nativement sur Sacado)

---

## 🔖 Version bookmarklet

Tu peux aussi l'utiliser comme bookmarklet pour ne pas avoir à ouvrir la console à chaque fois :

```
javascript:(function(){ /* code minifié ici */ })();
```

Crée un nouveau favoris dans ton navigateur, colle ça dans le champ URL, et clique dessus depuis n'importe quelle page Sacado.

---

## ⚠️ Disclaimer

> **Ce projet est à but éducatif et de recherche uniquement.**
> L'utiliser sur des devoirs notés peut violer la politique d'intégrité académique de ton établissement.
> L'auteur n'est pas responsable des conséquences liées à un mauvais usage.

---

## 📄 Licence

MIT
