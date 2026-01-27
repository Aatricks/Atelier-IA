# LightDiffusion-Next : Débuter Simplement

Avant de plonger dans des graphes de nœuds complexes, commençons par une expérience simplifiée. **LightDiffusion-Next** est conçu pour être rapide, efficace et accessible.

---

## 🕹️ L'Interface en un Coup d'Œil

LightDiffusion-Next se concentre sur les "Trois Piliers" de la génération d'images :
1.  **Le Prompt :** Ce que vous voulez voir.
2.  **Le Prompt Négatif :** Ce que vous *ne voulez pas* voir (ex: "flou, mauvaise qualité").
3.  **Le Modèle (Checkpoint) :** Le "cerveau" de l'IA (SDXL, SD1.5, etc.).

![Capture d'écran : Disposition de l'interface LightDiffusion-Next](images/ld_ui_layout.png)

---

## 🛠️ Votre Première Génération

Suivez ces étapes pour créer votre premier chef-d'œuvre :

### 1. Rédiger le Prompt
Tapez une description précise. Utilisez des virgules pour séparer les concepts.
- **Exemple :** `Une ville cyberpunk futuriste, néons, rues mouillées par la pluie, éclairage cinématographique, résolution 8k`

### 2. Choisir vos Réglages
- **Sampling Steps (Étapes) :** 20 à 30 est généralement parfait. Trop peu et l'image sera floue ; trop et cela prendra du temps inutilement.
- **CFG Scale :** Généralement entre 5 et 8. Cela contrôle la fidélité de l'IA par rapport à votre texte.
- **Résolution :** Commencez par `512x512` (pour SD1.5) ou `1024x1024` (pour SDXL).

### 3. Cliquez sur "Générer"
Attendez quelques secondes. Grâce aux optimisations comme `Stable-Fast`, vous verrez votre image apparaître presque instantanément !

---

## 💡 Astuces pour Débutants
- **Poids des mots-clés :** Dans la plupart des interfaces, vous pouvez utiliser `(mot-clé:1.2)` pour lui donner plus d'importance.
- **Formats d'image :** Essayez `768x512` pour des paysages ou `512x768` pour des portraits.
- **Styles :** N'hésitez pas à ajouter des styles comme "Studio Ghibli", "Cyberpunk" ou "Peinture à l'huile".

!!! tip "Essayez ceci !"
    Générez une image de "Un chalet confortable dans les bois en automne". Ensuite, essayez d'ajouter "sous la neige" au prompt et regardez comment l'IA adapte toute la scène !

---

[Suivant : Nœuds avancés avec ComfyUI &rarr;](comfyui.md)