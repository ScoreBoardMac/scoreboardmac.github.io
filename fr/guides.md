---
lang: fr
ref: guides
layout: page
title: Guide d'utilisation
description: >
  Tutoriels pas à pas pour ajouter un tableau de score ScoreBoard dans OBS, Streamlabs, Wirecast
  ou Meld : chronos texte, fond de tableau de score, chrono au dixième de seconde et compositions d'équipe.
image: /img/scoreboard_for_mac_light.png
permalink: /fr/guides/
---

Tutoriels pour ajouter un tableau de score dans OBS — les mêmes sources de fichiers TXT et image fonctionnent de la même façon dans Streamlabs, Wirecast et Meld.

_Les noms des menus d'OBS sont donnés pour l'interface en français, entre parenthèses pour l'interface en anglais._

- [Questions fréquentes](#faq)
- [Premiers pas](#getting-started)
- [Fichiers texte et image de sortie](#output-text-and-image-files)
- [Ajouter un chrono/compteur dans OBS](#how-to-add-a-text-timer-or-counter-in-obs)
- [Ajouter un fond de tableau de score](#how-to-add-a-scorebug-background-image-in-obs)
- [Afficher correctement les dixièmes](#how-to-display-tenths-of-a-second-in-obs)
- [Afficher les compositions d'équipe](#how-to-show-team-rosters-in-an-obs-broadcast)

---

## Questions fréquentes {#faq}

**Comment ajouter un tableau de score sportif en direct dans OBS sur Mac ?**  
Installez ScoreBoard pour Mac, puis ajoutez ses fichiers TXT de sortie comme sources *Texte (FreeType 2)* et ses images de promo/logo comme sources *Image* dans OBS — voir [Premiers pas](#getting-started) ci-dessous.

**Pourquoi ma source texte OBS ne se met-elle pas à jour instantanément ?**  
Par défaut, OBS relit les fichiers texte environ une fois par seconde. Pour des mises à jour plus rapides (par ex. les dixièmes de seconde d'un chrono), utilisez le plugin Advanced Scene Switcher — voir [Afficher les dixièmes de seconde](#how-to-display-tenths-of-a-second-in-obs).

**Puis-je afficher les compositions d'équipe dans mon stream ?**  
Oui — saisissez la composition sous forme de texte dans le champ Statut d'une équipe et/ou ajoutez-la comme image via les boutons promo, puis affichez-la avec des sources Texte et Image dans OBS — voir [Afficher les compositions d'équipe](#how-to-show-team-rosters-in-an-obs-broadcast).

**Est-ce que cela fonctionne dans Streamlabs, Wirecast ou Meld à la place d'OBS ?**  
Oui. ScoreBoard produit de simples fichiers TXT et image, que tout logiciel de streaming disposant de sources de type fichier texte ou image peut lire comme le fait OBS.

**Ai-je besoin d'une image de fond pour le tableau de score, ou les sources texte suffisent-elles ?**  
Les deux fonctionnent. Les sources texte seules affichent les valeurs en direct ; une image de fond placée derrière (voir [Ajouter un fond de tableau de score](#how-to-add-a-scorebug-background-image-in-obs)) donne un rendu plus soigné.

---

## Premiers pas {#getting-started}

**Scoreboard pour OBS sur macOS** est une application simple d'utilisation conçue pour les passionnés de sport, les diffuseurs et les streamers qui veulent afficher le score en direct de deux équipes ou joueurs dans leurs scènes OBS Studio. Cette application légère simplifie la gestion et l'intégration d'un tableau de score, pour que vous puissiez vous concentrer sur le match et votre public.

**Améliorez vos retransmissions sportives avec Scoreboard pour OBS sur macOS — simple, efficace et conçu pour le direct !**

## Cas d'usage idéaux {#ideal-use-cases}

- Événements sportifs (football, basket, volley, etc.)  
- Tournois d'e-sport et de jeux vidéo  
- Streams de commentaires et d'analyse en direct  

## Fonctionnalités {#features}

- **Mise à jour du score en direct :** modifiez facilement le score en temps réel pendant un match.  
- **Intégration par fichiers texte :** l'application génère et met à jour automatiquement des fichiers `.txt` avec les données du tableau de score, compatibles avec la source *Texte (FreeType 2)* d'OBS Studio.  
- **Faible consommation de ressources :** l'application est optimisée pour macOS et reste fluide même sur des machines modestes.  
- **Interface intuitive :** une interface simple et claire pour gérer les équipes, le score et les autres détails du match.
- **Mise en page personnalisable :** adaptez l'apparence du tableau de score au style de votre stream — taille de police, couleur et position. Cela se fait dans le logiciel de streaming, par exemple OBS.  

## Fonctionnement {#how-it-works}

1. **Installez l'application**  
   - Installez ScoreBoard pour Mac sur votre ordinateur :  
      - [Acheter sur le Mac App Store](https://apps.apple.com/app/id1579159150)  
      - [Télécharger la version gratuite](/free-apps/ScoreBoard-free.zip) et la décompresser — notariée par Apple et sûre  
   - Ouvrez l'application et configurez les noms des équipes/joueurs ainsi que les autres réglages initiaux.  

2. **Mettez à jour le score en temps réel**  
   - Modifiez le score des équipes avec les commandes simples de l'application.  
   - L'application enregistre automatiquement les valeurs dans des fichiers `.txt`. Dossier par défaut : `Téléchargements/ScoreBoard Outputs`.

3. **Intégrez avec OBS Studio**  
   - Dans OBS, créez une nouvelle source *Texte (FreeType 2)* ou faites simplement glisser le fichier texte voulu dans la fenêtre d'OBS.  
   - Activez l'option « Lire à partir d'un fichier » (*Read from File*) et sélectionnez le fichier `.txt` généré par l'application.  
   - Personnalisez la source texte dans OBS : position, taille, police, couleur, etc.  

4. **Diffusez ou enregistrez**  
   - Lorsque vous modifiez le score dans ScoreBoard, les changements apparaissent dans OBS en temps réel. OBS lit automatiquement les fichiers sur le disque (environ une fois par seconde) et affiche le résultat.  

---

## Fichiers texte et image de sortie {#output-text-and-image-files}

Par défaut, ScoreBoard écrit ces fichiers dans `Téléchargements/ScoreBoard Outputs` (vous pouvez choisir un autre dossier dans les Préférences). Chaque fichier `.txt` est mis à jour en direct pendant que vous gérez le match et s'ajoute dans OBS comme source **Texte (FreeType 2)** ; chaque fichier `.png` s'ajoute comme source **Image** — voir [Premiers pas](#getting-started) ci-dessus.

### Fichiers texte {#text-files}

| Fichier | Contenu | Exemple |
|---|---|---|
| `Timer.txt` | Chrono/chronomètre principal du match | `12:45` |
| `Timer_Extra.txt` | Chrono supplémentaire avec deux préréglages (par ex. chrono des tirs) | `14` |
| `Home_Name.txt` / `Away_Name.txt` | Noms des équipes | `Eagles` |
| `Match_Name.txt` | Nom du match/de l'événement | `Semifinal` |
| `Period.txt` | Période/quart-temps/mi-temps en cours (aussi OT, 2OT, 3OT…) | `2nd` |
| `Home_Goal.txt` / `Away_Goal.txt` | Score principal (buts/points) de chaque équipe | `3` |
| `Home_Shots.txt` / `Away_Shots.txt` | Compteur supplémentaire de tirs de chaque équipe | `18` |
| `Home_Points.txt` / `Away_Points.txt` | Compteur supplémentaire de points de chaque équipe | `2` |
| `Home_Status.txt` / `Away_Status.txt` | Description/statut de l'équipe — sert aussi pour les [compositions d'équipe](#how-to-show-team-rosters-in-an-obs-broadcast) | `#9 J. Smith` |
| `Match_Status.txt` | Description/statut du match | `Final` |
| `Home_Penalties_Numbers.txt` / `Away_Penalties_Numbers.txt` | Numéros des joueurs pénalisés, un par ligne | `12` |
| `Home_Penalties_Timers.txt` / `Away_Penalties_Timers.txt` | Temps restant de chaque pénalité en cours, un par ligne | `1:32` |
| `NHL_Penalties_Title.txt` | Libellé de la situation numérique pour la pénalité en cours la plus courte | `5 ON 4` |
| `NHL_Penalties_Time.txt` | Temps restant de la pénalité en cours la plus courte | `1:32` |

### Fichiers image {#image-files}

| Fichier | Contenu |
|---|---|
| `Home_Logo.png` / `Away_Logo.png` / `Match_Logo.png` | Logo de l'équipe/du match |
| `Home_Promo.png` / `Away_Promo.png` / `Match_Promo.png` | Visuel promo, par ex. une image de la composition d'équipe |
| `Home_Penalty_Card.png` / `Away_Penalty_Card.png` | Visuel de carton jaune/rouge |

Tous les fichiers ne servent pas pour tous les sports : les tirs et les points sont des compteurs indépendants que vous pouvez renommer selon votre sport, et les deux fichiers de pénalités NHL ne sont mis à jour que pendant une pénalité en cours.

---

## Ajouter un chrono ou un compteur texte dans OBS {#how-to-add-a-text-timer-or-counter-in-obs}

![Ajout dans OBS d'une source texte de chrono liée à un fichier TXT de ScoreBoard](/tutorial-img/how_add_text_to_obs.gif)

### 1. Ouvrez OBS Studio  
Lancez OBS Studio sur votre ordinateur.

### 2. Créez une nouvelle scène (facultatif)  
Pour organiser votre configuration, créez une nouvelle scène :  
- Cliquez sur le bouton **+** dans la section **Scènes** (*Scenes*).  
- Donnez un nom à la scène et enregistrez-la.

### 3. Ajoutez une source texte  
- Dans la section **Sources**, cliquez sur le bouton **+**.  
- Sélectionnez **Texte (FreeType 2)** (*Text (FreeType 2)*) dans la liste.  
*Ou faites simplement glisser le fichier texte voulu depuis le Finder dans la fenêtre d'OBS.*

### 4. Nommez la source texte  
- Saisissez un nom explicite pour la source (par ex. `Main Timer`).  
- Cliquez sur **OK** pour créer la source.

### 5. Activez la lecture depuis un fichier  
- Dans la fenêtre des propriétés de la source texte, cochez **Lire à partir d'un fichier** (*Read from File*).  
- Le texte sera ainsi mis à jour automatiquement à partir d'un fichier TXT.

### 6. Sélectionnez le fichier TXT  
- Cliquez sur **Parcourir** (*Browse*) à côté du champ du chemin de fichier.  
- Accédez à votre fichier TXT local, sélectionnez-le et cliquez sur **Ouvrir** (*Open*).

### 7. Placez le texte sur le canevas  
- Faites glisser la zone de texte dans l'aperçu pour la positionner dans la scène.  
- Redimensionnez-la si nécessaire.

### 8. Personnalisez l'apparence  
- Utilisez les options **Police**, **Taille** et **Couleur** (*Font*, *Size*, *Color*) pour régler le style du texte.  
- Essayez l'alignement, le dégradé et le fond pour l'adapter à votre mise en page.

### 9. Testez la mise à jour du fichier  
- Modifiez la valeur du compteur dans ScoreBoard, par exemple en lançant un chrono.  
- Vérifiez que les changements apparaissent dans OBS en temps réel.

**Ajoutez et configurez de la même façon tous les chronos/compteurs nécessaires au stream de votre sport.**

---

## Ajouter une image de fond de tableau de score dans OBS {#how-to-add-a-scorebug-background-image-in-obs}

![Ajout d'une source image de fond de tableau de score dans OBS](/tutorial-img/how_add_scoreboard_background_to_obs.gif)

### 1. Ajoutez une source Image  
- Dans la section **Sources**, cliquez sur le bouton **+**.  
- Sélectionnez **Image** dans la liste.  
*Ou faites simplement glisser l'image voulue depuis le Finder dans la fenêtre d'OBS.*

### 2. Nommez la source image  
- Saisissez un nom explicite pour la source (par ex. `Background`) et cliquez sur **OK**.  

### 3. Sélectionnez le fichier image  
- Cliquez sur **Parcourir** (*Browse*) à côté du champ du chemin de fichier.  
- Accédez à votre fichier image local, sélectionnez-le et cliquez sur **Ouvrir** (*Open*).
- Cliquez ensuite sur **OK** pour enregistrer la source.

### 4. Placez l'image sous les calques de texte  
- Faites glisser l'image dans l'aperçu pour la positionner dans la scène.  
- Redimensionnez-la si nécessaire.
- Dans la liste des sources, déplacez le fond tout en bas.

*Exemple de fond pour tableau de score :*
![Exemple de modèle de fond pour un tableau de score sportif](/tutorial-img/DefaultScoreBoard.png)

---

## Afficher les dixièmes de seconde dans OBS {#how-to-display-tenths-of-a-second-in-obs}

*Par défaut, OBS lit les fichiers texte environ une fois par seconde. Pour afficher correctement les dixièmes, il faut réduire ce délai.*

![Chrono au dixième de seconde dans OBS grâce à Advanced Scene Switcher](/tutorial-img/AdvancedSceneSwitcher/Show_tenths_timer.gif)

### 1. Installez le plugin [Advanced Scene Switcher](https://obsproject.com/forum/resources/advanced-scene-switcher.395/)
  
### 2. Ouvrez le plugin 
- Menu principal d'OBS – **Outils** (*Tools*) – **Advanced Scene Switcher**  
- Dans l'onglet **General**, réglez **Check conditions every** sur **100ms**

![Onglet General d'Advanced Scene Switcher avec un intervalle de vérification de 100 ms](/tutorial-img/AdvancedSceneSwitcher/Advanced_Scene_Switcher_General.png)

### 3. Ajoutez une nouvelle macro  
- Cliquez sur le bouton **+** en bas à gauche et renommez la macro (par ex. « Timer Delay »)  
- Décochez **Perform actions only on condition change**  

### 4. Ajoutez une nouvelle condition  
- Cliquez sur le bouton **+** dans la section des conditions  
- Sélectionnez **If**  
- Choisissez **File**  
- Cliquez sur **Browse**  
- Sélectionnez le fichier « Timer.txt » (ou un autre) dans le dossier de sortie de ScoreBoard  
- Réglez la condition sur **content changed**  

### 5. Ajoutez une nouvelle action  
- Cliquez sur le bouton **+** dans la section des actions  
- Sélectionnez **Source**  
- Choisissez **Set Settings**  
- Sélectionnez votre source FreeType 2 (par ex. « Main Timer »)  
- Réglez **Text(Text)**  
- Choisissez **Set to macro property**  
- Sélectionnez **File content**

![Condition et action d'une macro Advanced Scene Switcher pour mettre à jour la source texte OBS](/tutorial-img/AdvancedSceneSwitcher/Advanced_Scene_Switcher_Macro.png)

### 6. Changez le mode de saisie du texte de la source du chrono  
- Dans OBS, double-cliquez sur votre source FreeType 2 dans la liste des sources (par ex. « Main Timer »)  
- Passez le mode de saisie du texte (*Text input mode*) en manuel (*Manual*)  
- Saisissez un texte provisoire quelconque (par ex. une espace) dans le champ **Texte** (*Text*)  
- Cliquez sur **OK**

![Propriétés d'une source texte FreeType 2 dans OBS en mode de saisie manuel](/tutorial-img/AdvancedSceneSwitcher/OBS_Property_FreeType2_manual.png) 

### 7. Lancez le chrono principal dans ScoreBoard et testez  
- Dans les réglages de ScoreBoard, choisissez un style pour le chrono principal (par ex. [:5.3] ou [5.3])
- Pour tester, réglez le chrono de ScoreBoard sur 1 minute (1:00)
- Lancez le chrono et vérifiez le résultat dans OBS

---

## Afficher les compositions d'équipe dans une diffusion OBS {#how-to-show-team-rosters-in-an-obs-broadcast}
![Composition d'équipe affichée à côté d'un tableau de score ScoreBoard dans OBS](/tutorial-img/RostersScoreBoard.png)

### Source image {#image-source}
1. Créez un fichier graphique (PDF ou image) contenant la composition de l'équipe avec le logiciel de votre choix.

2. Ajoutez ce fichier au bouton promo de l'équipe à domicile (home promo) ou à l'extérieur (away promo) dans ScoreBoard et rendez-le visible.

3. Ajoutez dans OBS une source Image pour le fichier Home_Promo.png ou Away_Promo.png.

### Source texte {#text-source}
1. Ajoutez dans OBS une source texte pour les fichiers Home_Status.txt et Away_Status.txt.

2. Saisissez la composition dans le champ Statut (Status) de chaque équipe dans ScoreBoard. Par exemple :
>#4   Erik Lindqvist  
>#7   Marco Bianchi  
>#9   Connor MacLeod  
>#11  Lukas Weber  
>#13  Tomas Novak  
>#16  Henrik Andersson  
>#19  Diego Fernandez  
>#21  Kai Nakamura  
>#23  Owen Fitzgerald  
>#27  Niklas Berg  
>#29  Marek Kowalski  
>#33  Jesse Virtanen  
>#44  Liam O'Brien  
>#61  Pavel Dvorak  
>#71  Anders Holm  
>#88  Zach Whitfield  
>#91  Miroslav Klimek  

3. Ajoutez une image de fond ou une source de couleur unie (*Color Source*).

4. Regroupez les calques de texte et de fond dans un même groupe pour contrôler leur visibilité d'un seul clic.

---

Retour à la [présentation de ScoreBoard pour Mac](/fr/) ou [téléchargez la version d'essai gratuite](/free-apps/ScoreBoard-free.zip).

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "inLanguage": "fr",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Comment ajouter un tableau de score sportif en direct dans OBS sur Mac ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Installez ScoreBoard pour Mac, puis ajoutez ses fichiers TXT de sortie comme sources Texte (FreeType 2) et ses images de promo/logo comme sources Image dans OBS."
      }
    },
    {
      "@type": "Question",
      "name": "Pourquoi ma source texte OBS ne se met-elle pas à jour instantanément ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Par défaut, OBS relit les fichiers texte environ une fois par seconde. Pour des mises à jour plus rapides, comme les dixièmes de seconde d'un chrono, utilisez le plugin Advanced Scene Switcher : il réduit l'intervalle de vérification et transmet le contenu du fichier à la source texte."
      }
    },
    {
      "@type": "Question",
      "name": "Puis-je afficher les compositions d'équipe dans mon stream ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Oui. Saisissez la composition sous forme de texte dans le champ Statut d'une équipe et/ou ajoutez-la comme image via les boutons promo de ScoreBoard, puis affichez-la avec des sources Texte et Image dans OBS."
      }
    },
    {
      "@type": "Question",
      "name": "Est-ce que cela fonctionne dans Streamlabs, Wirecast ou Meld à la place d'OBS ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Oui. ScoreBoard produit de simples fichiers TXT et image, que tout logiciel de streaming disposant de sources de type fichier texte ou image peut lire comme le fait OBS."
      }
    },
    {
      "@type": "Question",
      "name": "Ai-je besoin d'une image de fond pour le tableau de score, ou les sources texte suffisent-elles ?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Les deux fonctionnent. Les sources texte seules affichent les valeurs en direct ; une image de fond placée derrière donne à la surimpression un rendu plus soigné."
      }
    }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "inLanguage": "fr",
  "name": "Ajouter un chrono ou un compteur texte dans OBS",
  "step": [
    { "@type": "HowToStep", "position": 1, "name": "Ouvrez OBS Studio", "text": "Lancez OBS Studio sur votre ordinateur." },
    { "@type": "HowToStep", "position": 2, "name": "Créez une nouvelle scène (facultatif)", "text": "Cliquez sur le bouton + dans la section Scènes, donnez un nom à la scène et enregistrez-la." },
    { "@type": "HowToStep", "position": 3, "name": "Ajoutez une source texte", "text": "Dans la section Sources, cliquez sur le bouton + et sélectionnez Texte (FreeType 2), ou faites glisser le fichier texte voulu depuis le Finder dans la fenêtre d'OBS." },
    { "@type": "HowToStep", "position": 4, "name": "Nommez la source texte", "text": "Saisissez un nom explicite pour la source et cliquez sur OK pour la créer." },
    { "@type": "HowToStep", "position": 5, "name": "Activez la lecture depuis un fichier", "text": "Dans la fenêtre des propriétés de la source texte, cochez Lire à partir d'un fichier." },
    { "@type": "HowToStep", "position": 6, "name": "Sélectionnez le fichier TXT", "text": "Cliquez sur Parcourir à côté du champ du chemin de fichier, accédez à votre fichier TXT local, sélectionnez-le et cliquez sur Ouvrir." },
    { "@type": "HowToStep", "position": 7, "name": "Placez le texte sur le canevas", "text": "Faites glisser la zone de texte dans l'aperçu pour la positionner dans la scène et redimensionnez-la si nécessaire." },
    { "@type": "HowToStep", "position": 8, "name": "Personnalisez l'apparence", "text": "Utilisez les options Police, Taille et Couleur pour régler le style du texte." },
    { "@type": "HowToStep", "position": 9, "name": "Testez la mise à jour du fichier", "text": "Modifiez la valeur du compteur dans ScoreBoard et vérifiez que les changements apparaissent dans OBS en temps réel." }
  ]
}
</script>

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "inLanguage": "fr",
  "name": "Ajouter une image de fond de tableau de score dans OBS",
  "step": [
    { "@type": "HowToStep", "position": 1, "name": "Ajoutez une source Image", "text": "Dans la section Sources, cliquez sur le bouton + et sélectionnez Image, ou faites glisser l'image voulue depuis le Finder dans la fenêtre d'OBS." },
    { "@type": "HowToStep", "position": 2, "name": "Nommez la source image", "text": "Saisissez un nom explicite pour la source et cliquez sur OK." },
    { "@type": "HowToStep", "position": 3, "name": "Sélectionnez le fichier image", "text": "Cliquez sur Parcourir à côté du champ du chemin de fichier, sélectionnez votre image locale, cliquez sur Ouvrir, puis sur OK pour enregistrer la source." },
    { "@type": "HowToStep", "position": 4, "name": "Placez l'image sous les calques de texte", "text": "Faites glisser l'image dans l'aperçu pour la positionner, redimensionnez-la si nécessaire et déplacez-la tout en bas de la liste des sources." }
  ]
}
</script>
