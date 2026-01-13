# 🇲🇬 API des Universités de Madagascar

[![Data Quality](https://img.shields.io/badge/Data-Official-emerald)](https://github.com/ezdev2/Recognized-Universities-Madagascar)
[![Last Update](https://img.shields.io/badge/Dernière%20Mise%20à%20Jour-AUTO-blue)](#)

Cette plateforme fournit un accès structuré (JSON) à la liste des universités et instituts supérieurs accrédités par le Ministère de l'Enseignement Supérieur de Madagascar.
La liste a été extraite d’un **document PDF public** fourni par le MESUPRES, disponible publiquement sur leur site officiel. Elle recense les universités, instituts supérieurs, écoles spécialisées et établissements agréés à délivrer des diplômes de type Licence, Master et Doctorat.

> **Dernière mise à jour globale :** _Mardi 13 Janvier 2026_

---

## Utilisation de l'API (Endpoints)

Vous pouvez utiliser ces fichiers directement dans vos applications (via `fetch` ou `axios`) en utilisant les liens "Raw" de GitHub :

| Ressource | URL de l'API | Description |
| :--- | :--- | :--- |
| **Universités** | `https://cdn.jsdelivr.net/gh/ezdev2/Recognized-Universities-Madagascar@main/university.json` | Liste des établissements (Nom, Adresse, Type). |
| **Domaines** | `https://cdn.jsdelivr.net/gh/ezdev2/Recognized-Universities-Madagascar@main/domain.json` | Mentions et filières accréditées par établissement. |

### Exemple rapide (JavaScript)
```javascript
fetch('https://cdn.jsdelivr.net/gh/ezdev2/Recognized-Universities-Madagascar@main/university.json')
  .then(res => res.json())
  .then(data => console.log(data))
  .catch(err => console.error("Erreur :", err));

```

---

## Exemple d'utilisation

Vous pouvez voir une implémentation concrète de cette API sur la plateforme suivante :
👉 **[Smartparcours - Index Universitaire](https://universite.smartparcours.site/)**

---

## 🤝 Comment Contribuer ?

Nous avons besoin de la communauté pour maintenir ces données à jour !

### 1. Proposer une modification

Si vous constatez une erreur ou une université manquante :

1. **Forkez** ce dépôt.
2. Modifiez le fichier `university.json` ou `domain.json`.
3. Assurez-vous que le **nom de l'université** est identique dans les deux fichiers pour garantir la liaison des données.
4. Soumettez une **Pull Request (PR)**.

### 2. Critères de validation

Pour être acceptée, toute modification doit :

* Correspondre à une accréditation officielle du MESUPRES.
* Respecter le formatage JSON actuel (pas de fautes de frappe dans les clés).
* Être accompagnée d'un lien source si POSSIBLE (site officiel, décret, etc.).

---

## Protection des données

La branche `main` est protégée. Toutes les modifications doivent passer par une Pull Request et une validation manuelle pour garantir la fiabilité des informations diffusées aux étudiants.

---

## Source officielle

> **Ministère de l’Enseignement Supérieur et de la Recherche Scientifique (MESUPRES)**  
> **Document :** Liste des établissements d’enseignement supérieur reconnus – Dernière mis à jour Août 2022  
> **Format :** PDF  
> **Lien :** [`liste-universites-madagascar.pdf`](https://www.mesupres.gov.mg/assets/front/documents/documents/habilitations/liste_des_institutions_superieures_mise_a_jour_aout_2022.pdf)

---

## Télécharger

La liste complète est disponible dans le fichier :  
👉 [`liste-universites-madagascar.pdf`](https://www.mesupres.gov.mg/assets/front/documents/documents/habilitations/liste_des_institutions_superieures_mise_a_jour_aout_2022.pdf)

---

## ✉️ Contact

Pour toute mise à jour ou suggestion, veuillez contacter :  
📧 [fansoaezra@gmail.com]

---

