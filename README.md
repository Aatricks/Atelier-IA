# Atelier IA : Architecture de la Diffusion

Ce dépôt contient le support de cours et les ressources pour l'atelier dédié à l'architecture des modèles de diffusion. L'objectif est de comprendre les mécanismes internes de la génération d'images, de l'espace latent au décodage final.

## Objectifs de la formation
- Comprendre le processus de débruitage gaussien.
- Analyser l'impact des paramètres techniques (Seed, Steps, CFG Scale, Samplers).
- Manipuler une structure de génération nodale.

## Programme de l'atelier

### Module 1 : Validation des concepts (LightDiffusion)
Utilisation d'une interface simplifiée pour isoler les variables fondamentales et observer leur influence sur le résultat visuel.
- Lien : [LightDiffusion-Next](https://github.com/Aatricks/LightDiffusion-Next)

### Module 2 : Architecture nodale (ComfyUI)
Approche structurelle consistant à reconstruire manuellement une pipeline de génération fonctionnelle.
- Lien : [ComfyUI](https://github.com/comfyanonymous/ComfyUI)

## Ressources techniques

### Documentation locale
- [Guide de l'atelier](docs/index.md) : Support détaillé structuré par modules.

### Écosystème et outils
- [ComfyUI Manager](https://github.com/ltdrdata/ComfyUI-Manager) : Gestionnaire d'extensions et de nœuds personnalisés.
- [Civitai](https://civitai.com/) : Plateforme de partage de modèles et de ressources (Checkpoints, LoRA).

### Références théoriques
- [ComfyUI for Beginners](https://youtu.be/xoq5IesqCUE) : Tutoriel sur la logique des workflows.
- [Stable Diffusion Explained](https://www.youtube.com/watch?v=1CIpzeNxIhU) : Analyse technique par Computerphile.