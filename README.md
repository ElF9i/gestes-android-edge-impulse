# Reconnaissance de gestes — Android + Edge Impulse

Application Android (Java + XML) qui lit le **gyroscope/accéléromètre** du téléphone et classifie le geste en temps réel avec un modèle **TinyML** entraîné sur Edge Impulse.

## Gestes reconnus
`horizontal` · `vertical` · `cercle`

## Fonctionnalités
- Affichage en direct des valeurs x, y, z
- Collecte de données pour l'entraînement
- Inférence avec le modèle exporté d'Edge Impulse

## Stack
- Android Studio, Java, XML
- Edge Impulse (cible Cortex-M4F pour le projet d'entraînement)

## Lancer le projet
1. Cloner le dépôt et l'ouvrir dans Android Studio
2. Placer le modèle exporté d'Edge Impulse dans `app/libs/` ou `app/src/main/cpp/`  <!-- À adapter -->
3. Compiler et lancer sur un téléphone physique (les capteurs ne sont pas simulés)

## Structure
```
app/src/main/java/   # activités, capteurs, inférence
app/src/main/res/    # layouts XML
```

## Contexte
Dérivé du TP « TinyML – IA embarquée » — ISET Charguia.
