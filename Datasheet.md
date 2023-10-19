# Iowa gambling task (columns)

name            | description                                                                                       | options 
choice          | The choice of the participant as letter   | A, B, C, D
value           | The value of the choice                   | -250, -50, 50 , 100
score_before    | The score before the choice               | some number
score_after     | The score after the choice                | some number
values          | The values of all the decks in this trial | [-250 or -50 or 50 or 100, ..., ..., ...]                                               | 0, 1
choice_index    | The choice as an index choice             | 0, 1, 2, 3
reward          | The reward of the chosen deck             | 50, 100
penalty         | The penalty of the chosen deck            | -250, -50
chance          | The reward probability of the chosen deck | some number between 0 and 1

choice: choice,
                    value: value,
                    score_before: trial.current_score,
                    score_after: trial.current_score + trial.values[i],
                    values: JSON.stringify(trial.values),
                    choice_index: i,
                    reward: trial.reward_penalty[i][0],
                    penalty: trial.reward_penalty[i][1],
                    chance: trial.chance