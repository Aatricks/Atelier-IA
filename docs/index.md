# Atelier : Architecture de la Diffusion

La majorité des outils d'IA génératrice d'images (Midjourney, ChatGPT, DALL-E) masquent la complexité technique derrière une simple barre de texte. Cet atelier propose d'ouvrir la "boîte noire" pour comprendre les mécanismes fondamentaux qui permettent à une machine de transformer des données numériques en représentations visuelles cohérentes.

---

## Fonctionnement théorique

La génération d'images par diffusion repose sur un processus de réduction du bruit. Contrairement à une croyance commune, l'IA ne "dessine" pas ; elle sculpte une information à partir d'un chaos statistique.

!!! info "Le concept de débruitage"
    Le processus commence par un bruit gaussien pur (une image composée de pixels aléatoires). L'IA, entraînée sur des millions d'exemples, prédit à chaque étape la quantité de bruit à retirer pour se rapprocher d'un concept connu.
    
    ![Processus de débruitage](images/denoising_process.webp)
    *Visualisation de l'émergence d'une forme à travers les étapes de débruitage.*

---

## Composants fondamentaux

Pour manipuler ces modèles, il est essentiel de comprendre trois composants techniques :

!!! abstract "1. L'Espace Latent"
    Travailler sur des images en haute résolution pixel par pixel est coûteux en ressources. La diffusion s'effectue donc dans un **espace latent**, une version compressée et mathématique de l'image. Le **VAE (Variational AutoEncoder)** est le composant chargé de la compression et de la décompression de ces données.

!!! abstract "2. Le Guidage (Conditioning)"
    Le texte que vous saisissez (le prompt) est converti par un encodeur de texte (**CLIP**) en vecteurs mathématiques. Ces vecteurs agissent comme des contraintes qui orientent le processus de débruitage vers un résultat spécifique.

!!! abstract "3. Le Planificateur (Scheduler)"
    Le scheduler détermine la vitesse et la méthode de retrait du bruit. C'est lui qui définit la trajectoire mathématique que prendra l'IA pour passer du bruit pur à l'image finale.

---

## Structure de l'atelier

L'apprentissage est divisé en deux modules complémentaires :

1.  **Validation des paramètres :** Utilisation de l'interface simplifiée **LightDiffusion** pour isoler et comprendre l'impact des variables de base (Seed, Steps, CFG).
2.  **Architecture nodale :** Utilisation de **ComfyUI** pour reconstruire manuellement le flux de données et comprendre l'interdépendance des composants.

[Accéder au Module 1 : LightDiffusion &rarr;](light-diffusion.md)