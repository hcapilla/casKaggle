# Cas Kaggle : Pokemon with stats

Repositorio creado con el objetivo de trabajar en el Caso Kaggle de la asignatura de ApC con el motivo: Pokémon with stats.

Dataset de Kaggle original: https://www.kaggle.com/abcsds/pokemon

**OBJETIVO:** predecir si un Pokémon es o no legendario basado en sus estadísticas básicas.

Trabajo realizado por Hernán Capilla.

***

El dataset tiene 721 Pokémon. Cada Pokémon es una criatura fantástica existente en el mundo Pokémon, perteneciente a la franquicia The Pokémon Company©.

Estas criaturas serían en su mundo lo que para nosotros son los animales. Con la diferencia de que cada una de estas puede tener diferentes atributos físicos y mágicos. Ahora lo explicaré con más profundidad por orden de atributos:

- '#': ID de cada Pokémon.

- Name: Nombre de cada Pokémon.

- Type 1: Cada Pokémon tiene un tipo, este tipo determinará sus debilidades o resistencias a los aatques de cierto tipo.

- Type 2: Algunos Pokémon tienen dos tipos diferentes. Las debilidades y resistencias se acumulan.

- Total: La suma de todos los campos de las estadísticas de un Pokémon.

- HP: En inglés 'Health Points', determina cuanta vida tiene un Pokémon y cuantos golpes aguanta.

- Attack: El modificador base que afectará al cálculo de daño de los ataques físicos.

- Defense: La resistencia base al daño de los ataques físicos.

- SP Atk: En inglés 'Special Attack', modificador base que afectará al cálculo de daño de los ataques especiales.

- SP Def: En inglés 'Special Defense', la resistencia base al daño de los ataques especiales.

- Speed: Determina, según quien la tiene mayor, qué Pokémon ataca antes en un combate.

- Generation: Cada entrega de los juegos para consola de Pokémon cuenta como una nueva generación. Empezamos por la 1ª que fue la del 1996 y llegamos hasta día de hoy.

- Legendary: En el mundo Pokémon hay algunas de estas criaturas que tienen el sobrenombre de Pokémon Legendarios. Esto proviene del hecho de que los calificados con ese pseudónimo tienen habilidades extraordinarias y fuera de lo común en su mundo. Pueden ser habilidades muy poderosas, o una dificultad de ser vistas gigantesca, o también que tengan unas estadísticas más elevadas de los común.


***

**Puntuaciones totales con los diferentes modelos y métodos probados:**

| Método | Puntuación (%) |
| --- | :---: |
| `Regresión Logística` | 95.625 |
| `RL con procesamiento` | 96.25 |
| `SVM` | 91.875 |
| `Random Forest` | 95.625 |
| `Gradient Boosting` | 98.75 |

Parámetros para el Gradient Boosting:
- learning_rate=0.9
- n_estimators = 100
- validation_fraction = 0.2
- n_iter_no_change=100
- random_state=10 (no es un parámetro como tal pero hay que ponerlo para mantener la coherencia con las demás pruebas)
