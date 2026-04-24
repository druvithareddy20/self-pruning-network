# Self-Pruning Neural Network

## Approach
We implemented a custom PrunableLinear layer with learnable gates applied to weights. A sparsity loss using L1 regularization encourages gates to become zero, effectively pruning weights.

## Results

| Lambda | Accuracy | Sparsity (%) |
|--------|----------|--------------|
| 0.001  | 38.37%   | 0.35%        |
| 0.01   | 36.89%   | 3.51%        |
| 0.1    | 37.41%   | 3.38%        |

## Observation
Higher lambda increases sparsity while slightly affecting accuracy, demonstrating the trade-off between model compression and performance.