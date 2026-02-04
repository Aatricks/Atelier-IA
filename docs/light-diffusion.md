# Module 1 : Validation des concepts de base

Cette première phase utilise l'interface **LightDiffusion-Next**. L'objectif est de valider les connaissances théoriques en observant l'impact direct des paramètres de génération sur une interface épurée.

---

## Paramètres de contrôle

Trois variables fondamentales permettent de piloter la génération.

!!! success "Le Prompt (Conditioning)"
    C'est la directive textuelle. L'IA interprète vos mots pour orienter le débruitage.
    *   **Positif :** Les éléments à inclure.
    *   **Négatif :** Les éléments ou styles à exclure explicitement.
    
    ![Interface des Prompts](images/LDN/Prompts.png)

!!! success "Le Sampling (Steps)"
    Le nombre d'itérations que l'IA effectue pour retirer le bruit. 
    *   **Observation :** Un nombre trop faible (ex: 10) laisse l'image inachevée. Un nombre trop élevé (ex: 50) s'avère souvent inefficace passé un certain point de convergence.
    
    ![Réglages de Sampling](images/LDN/Sampling.png)

!!! success "La Seed (Déterminisme)"
    La Seed est la valeur numérique qui initialise le bruit de départ. 
    *   **Fixe :** Permet de reproduire exactement la même image ou de tester l'influence d'un changement de texte sur une base identique.
    *   **Aléatoire (-1) :** Produit un nouveau point de départ à chaque génération.

!!! success "Le CFG Scale (Fidélité au Prompt)"
    Le **Classifier Free Guidance** contrôle l'équilibre entre la créativité de l'IA et le respect strict de vos instructions.
    *   **Valeur basse (1-3) :** L'IA est très libre, les couleurs sont souvent délavées et le prompt est peu suivi.
    *   **Valeur standard (7-9) :** Le compromis idéal pour la plupart des modèles.
    *   **Valeur haute (15+) :** L'IA force les traits, les contrastes deviennent extrêmes ("deep fried") et des artefacts peuvent apparaître.

!!! success "Le Sampler (Méthode de calcul)"
    C'est l'algorithme qui choisit comment retirer le bruit. Certains convergent très vite (Euler a, UniPC), d'autres demandent plus de temps mais offrent une texture plus fine (DPM++ 2M SDE).

---

## Exercices d'application

!!! note "Consignes de test"
    Pour chaque exercice, utilisez un modèle (checkpoint) de type SDXL ou SD1.5 disponible dans le sélecteur.
    
    1.  **Stabilité :** Générez une image, notez sa Seed, puis relancez la génération. Observez la reproduction identique.
    2.  **Variabilité :** Modifiez un seul adjectif dans votre prompt tout en conservant la même Seed. Analysez comment l'IA adapte la structure existante au nouveau concept.
    3.  **L'effet CFG :** Avec une Seed fixe, comparez une génération à CFG 1.0, 7.0 et 30.0. Observez la dégradation de l'image aux extrêmes.
    4.  **Comparaison de Samplers :** Testez le même prompt et la même Seed avec `Euler a` puis avec `DPM++ 2M Karras`. Notez les différences de détails, notamment sur les textures complexes.
    5.  **Convergence :** Observez la différence de netteté entre 15 et 30 steps sur un même prompt.

---

[Accéder au Module 2 : Architecture nodale (ComfyUI) &rarr;](comfyui.md)