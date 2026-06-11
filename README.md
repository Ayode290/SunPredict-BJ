# SunPredict-BJ
### IA qui dimensionne le kit solaire idéal à Cotonou pour diviser par 2 la facture d'électricité des ménages

**Projet soumis au hackathon Arm Create : Défi d'optimisation de l'IA**

## 1. Le Problème
À Cotonou, les délestages CEB sont fréquents. 70% des ménages achètent un kit solaire trop grand ou trop petit. Résultat : argent perdu, groupes électrogènes polluants.

## 2. La Solution
SunPredict-BJ est un prototype d'IA léger qui tourne sur CPU Arm.
L'utilisateur entre : appareils, heures d'usage, budget.
L'IA calcule la taille de kit optimale : panneaux + batterie + onduleur.

Formule clé :
$$P_{optimal} = \frac{Conso_{journaliere \ kWh}}{Ensoleillement_{Cotonou} \times Rendement_{systeme}}$$
Avec `Ensoleillement_Cotonou = 5.5 kWh/m²/jour`

## 3. Fonctionnalités V1
- [50] Entrée des données conso ménage
- [2000] Moteur d'optimisation de coût sur 2 ans
- [100] Recommandation kit 300W à 1.5KVA
- [ 5000] Connexion Mobile Money - Prochaine version

## 4. Techno utilisées
`Python`, `Streamlit`, `Pandas`, `NumPy`, `Scikit-learn`, `Arm CPU`
Compatible CPU Arm pour respecter le thème du hackathon.

## 5. Installation & Lancement
```bash
git clone https://github.com/Ayod/SunPredict-BJ.git
cd SunPredict-BJ
pip install -r requirements.txt
streamlit run app.py
