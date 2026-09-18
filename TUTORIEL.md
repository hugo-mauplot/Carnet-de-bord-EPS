# Guide d'utilisation — Studio EPS Collège

Ce document accompagne l'application `eps-college-dashboard.html`. Le même guide est accessible **dans l'app** via le bouton **?** (aide) en haut à droite de l'**Accueil** ou des **Réglages**.

---

## 1. Principe de l'application

**Studio EPS** est un tableau de bord pour enseignant·e d'EPS au collège. Il permet de :

- Générer et suivre les **séances** à partir de l'emploi du temps et des APSA
- Faire l'**appel** (présent / retard / absent) et rédiger un **résumé** par séance
- Joindre un **PDF** par séance
- Gérer les **dispenses** (avec ou sans certificat)
- Signaler les **oublis de matériel** et repérer les élèves en alerte
- Consulter la **programmation EPS** de l'établissement (PDF)
- Visualiser la **participation** des élèves par APSA

### Navigation

| Zone | Rôle |
|------|------|
| **Accueil** (⌂) | Vue du jour : indicateurs, cours, planning, tâches |
| **Classes** (📚) | Liste des classes et accès aux fiches séances |
| **Réglages** (⚙️) | Configuration, calendriers, sauvegarde, tutoriel |

Sur ordinateur : menu latéral avec accès direct à chaque classe.  
Sur iPhone : barre de navigation en bas.

> **Important :** les données sont stockées dans le **navigateur** (pas dans le fichier HTML). Un export JSON régulier est recommandé.

---

## 2. Configuration initiale (une fois par année)

Suivez cet ordre. Après toute modification structurelle (EDT, APSA, année scolaire), cliquez sur **↻ Régénérer les séances** en haut de l'Accueil.

| Étape | Où ? | Action |
|-------|------|--------|
| 1 | Réglages → Sauvegarde | Définir les dates de **début** et **fin** d'année scolaire |
| 2 | Réglages → Mes classes | Créer chaque **classe** (nom, cycle, effectif, couleur) |
| 3 | Même écran → ⚙️ sur la carte | Importer ou saisir la **liste des élèves** (prénoms) |
| 4 | Réglages → Organisation → Périodes | Créer P1, P2, P3… avec dates et classes associées |
| 5 | Réglages → Créneaux des classes | Renseigner l'**emploi du temps** hebdomadaire (jour, horaire, lieu) |
| 6 | Réglages → APSA & séquences | Créer les **activités** par classe, période et jours de cours |
| 7 | Réglages → Lieux de pratique | Ajouter gymnase, stade, piscine… |
| 8 | Réglages → Calendriers | Vacances, fériés ; **Appliquer le calendrier officiel** (zone académique) |
| 9 | Accueil → bouton **↻** | **Régénérer les séances** pour toute l'année |
| 10 | Réglages → Programmation | Déposer le **PDF** de programmation de l'établissement |

Sans périodes ni APSA sur la période du jour, l'Accueil n'affichera pas d'avancement pertinent dans « Séquences en cours ».

---

## 3. Routine quotidienne (Accueil)

### Navigation par date

- **◀ ▶** : jour précédent / suivant
- **Aujourd'hui** : revenir à la date du jour

### Les 4 indicateurs (grille en haut)

1. **Séances aujourd'hui** — nombre et détail des cours du jour affiché
2. **Élèves dispensés** — élèves dispensés qui ont cours ce jour-là
3. **Programmation EPS** — **Consulter** le PDF (si déposé dans les réglages)
4. **Oublis de matériel répétés** — élèves dépassant le seuil (⚙️ sur la carte pour le modifier, défaut : 3 oublis sur la période)

### Cours du jour

Chaque ligne est **cliquable**. Elle ouvre la fiche séance :

- Résumé de la séance
- Rappel des **absents au cours précédent** (même APSA)
- Liste des **élèves dispensés** pour ce cours
- **Appel** : Présent / Retard / Absent, ou « Tous présents »
- **Dispense** et **oubli de matériel** pour ce créneau
- **PDF** de séance (optionnel)

Badges sur la ligne : 📝 résumé saisi · 📄 PDF joint · **3P 1R 2A** = appel (Présents, Retards, Absents)

### Blocs secondaires (repliables)

- **À faire** — tâches personnelles
- **Séquences en cours** — avancement par classe/APSA (carte cliquable → page classe)
- **Modifications EDT à venir** — annulations et cours ajoutés sur 3 semaines

---

## 4. Page classe

Accès : onglet **Classes** ou carte sur l'Accueil.

### En-tête

- Effectif, cycle, prochaine / dernière séance
- **+ Ajouter un cours** : séance exceptionnelle hors APSA

### Blocs fixes

- **Dispenses** — tableau avec certificat, durée, statut ; ajouter / modifier / supprimer
- **Oublis de matériel** — historique de la période sélectionnée

### Sélecteur de période

Filtre les tableaux de séances (P1, P2… ou toutes les périodes).

### Tableau des séances (par APSA)

| Action | Comment |
|--------|---------|
| Cliquer une ligne | Ouvrir **résumé + appel + PDF** |
| **Annuler** | Sur une séance à venir (motif : pluie, gymnase, sortie…) |
| Badge appel | Ex. `12P 2R 1A` sur la ligne |

### Participation

Bouton **Participation des élèves aux séances** sous chaque APSA :

- Compte uniquement les séances **effectuées** (passées, non annulées)
- **Compté** : présent ou retard à l'appel
- **Exclu** : absent ou dispensé
- Détail sous le nom : *Dispensé le …* / *Absent le …* avec les dates

---

## 5. Dispenses médicales

### Avec certificat

- Date du certificat
- Durée en **nombre de jours** ou **date de fin** inscrite sur le certificat
- S'applique à **toutes les séances** de la classe sur la plage de dates

### Sans certificat

| Origine | Portée |
|---------|--------|
| **Cours du jour** (Accueil) | Case cochée par défaut → **ce cours uniquement** |
| **Page classe** → + Ajouter une dispense | Case « journée uniquement » → **tous les cours EPS de l'élève ce jour-là** |

### Où voir les dispensés ?

- Bandeau discret en haut de la fiche **Cours du jour**
- KPI **Élèves dispensés** sur l'Accueil
- Tableau **Dispenses** sur la page classe

---

## 6. Oublis de matériel

**Objets :** gourde, tenue, baskets.

**Saisie :**

- Fiche **Cours du jour** (Accueil)
- **Page classe** → + Ajouter un oubli

**Alerte :** carte **Oublis répétés** sur l'Accueil si un élève atteint le seuil sur la période en cours. Cliquer un nom pour ouvrir la classe.

---

## 7. Calendrier et annulations

### Calendrier scolaire (Réglages → Calendriers)

- Vacances, fériés, journées banalisées
- Bouton **Appliquer le calendrier officiel** selon votre académie / zone

### Calendrier visuel

Vues **mois** et **semaine** avec code couleur des statuts de séance.

### Annulations manuelles

- Depuis le **tableau de séances** d'une classe (bouton Annuler)
- Ou écran dédié dans **Calendriers**

Motifs proposés : pluie, gymnase indisponible, sortie, formation, absence enseignant, grève, journée banalisée, autre.

---

## 8. Sauvegarde et transfert

**Réglages → Sauvegarde**

| Bouton | Usage |
|--------|--------|
| **Export JSON** | Sauvegarde complète à archiver |
| **Import JSON** | Restaurer sur un autre appareil / navigateur |
| **Reset données** | Efface tout (irréversible) |
| **PDF (via impression)** | Imprimer la vue courante |

### Où sont mes données ?

Elles sont liées à l'**adresse exacte** utilisée pour ouvrir le fichier :

- Fichier local `file://…`
- Serveur local `http://127.0.0.1:…`
- Aperçu Cursor, Safari, Chrome…

→ Ce sont des emplacements **distincts**. Pour transférer : **Export** depuis l'ancien, **Import** dans le nouveau.

### Mode fichier sur iPhone

Si un **bandeau jaune** apparaît sur l'Accueil : les données peuvent être perdues à la fermeture de l'onglet. **Exportez souvent.**

---

## 9. Utilisation sur iPhone (conseils)

1. **Ajouter à l'écran d'accueil** (Safari → Partager → Sur l'écran d'accueil)
2. Utiliser l'**Accueil** le matin : indicateurs + **Cours du jour**
3. Pendant le cours : ouvrir la ligne → **appel** + dispenses / oublis éventuels
4. **Export JSON** hebdomadaire si vous n'utilisez pas de serveur local
5. Portrait recommandé (interface optimisée)

---

## 10. Raccourcis utiles

| Besoin | Chemin |
|--------|--------|
| Voir les cours de demain | Accueil → ▶ |
| Régénérer l'année | Accueil → ↻ |
| Liste des élèves | Réglages → Mes classes → ⚙️ |
| PDF programmation | Accueil → Programmation EPS → Consulter |
| Imprimer une classe | Page classe → Imprimer |
| Thème clair / sombre | Menu ☰ → Thème |
| Ce tutoriel | Bouton **?** (aide) sur Accueil ou Réglages |

---

*Studio EPS Collège — tableau de bord pédagogique local, sans compte ni serveur.*
