# Talent Scouting mit Machine Learning

## Ziel
Vorhersage, ob Fußballspieler basierend auf Scout-Bewertungen **average** oder **highlighted** sind.

## Datensatz
- **scoutium_attributes.csv**  
  - `task_response_id`, `match_id`, `evaluator_id`, `player_id`, `position_id`, `analysis_id`, `attribute_id`, `attribute_value`  
  - `position_id` (1=Torwart, 2=Innenverteidiger, 3=Rechtsverteidiger, 4=Linksverteidiger, 5=Defensives Mittelfeld, 6=Zentrales Mittelfeld, 7=Rechtsaußen, 8=Linksaußen, 9=Offensives Mittelfeld, 10=Stürmer)  

- **scoutium_potential_labels.csv**  
  - `task_response_id`, `match_id`, `evaluator_id`, `player_id`, `potential_label` (Zielvariable)  

## Datenvorverarbeitung
- Torhüter und "below_average"-Klasse entfernt  
- Pivot: Spieler → Zeilen, Attribute → Spalten  
- Feature-Normalisierung mit `StandardScaler`  

## Modelle & Ergebnisse
- Algorithmen: Logistic Regression, KNN, SVM, Decision Tree, Random Forest, AdaBoost, Gradient Boosting, XGBoost  
- Bestes Modell: **AdaBoost** (Accuracy 0.88, Precision 1.0, F1 0.59)  

## Empfehlungen
- Einsatz von AdaBoost  
- Hyperparameter-Tuning & Cross-Validation  
- Feature Engineering für weitere Insights  

