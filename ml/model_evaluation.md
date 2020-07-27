# Model Evaluation

## Accuracy

```
∑ true positive + ∑ true negative
---------------------------------
∑ total population
```

## Precision

```
∑ true positive
---------------
∑ true positive + ∑ false positive
```

## Recall

```
∑ true positive
---------------
∑ true positive + ∑ false negative
```

## F1 (harmonic mean between precision and recall)

```
2 * precision * recall
----------------------
precision + recall
```


## Confusion Matrix

```
                               |--------------------------------------------|
                               |  predicted condition                       |
           |----------------------------------------------------------------|
           |total population   |  prediction positive | prediction negative |
 |---------|----------------------------------------------------------------|
 |true     |condition          |  true positive (TP)  | false negative (FN) |
 |condition|positive           |                      |                     |
 |         |----------------------------------------------------------------|
 |         |condition          | false positive (FP)  | true negative (TN)  |
 |         |negative           |                      |                     |
 |---------|----------------------------------------------------------------|
```
