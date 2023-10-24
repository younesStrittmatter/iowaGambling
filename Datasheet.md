# Iowa gambling task (columns)

| name         | description                               | options                           |
|--------------|-------------------------------------------|-----------------------------------|
| choice       | The choice of the participant as letter   | A, B, C, D                        |
| value        | The value of the choice                   | -25, -5, 5 , 10                   |
| score_before | The score before the choice               | some number                       |
| score_after  | The score after the choice                | some number                       |
| values       | The values of all the decks in this trial | [-25 or -5 or 5 or 10, ..., ..., ...] |
| choice_index | The choice as an index choice             | 0, 1, 2, 3                        |
| reward       | The reward of the chosen deck             | 5, 10                             |
| penalty      | The penalty of the chosen deck            | -25, -5                           |
| chance       | The reward probability of the chosen deck | some number between 0 and 1       |
| type         | The type of the deck                      | "safe" of "risky"                 |