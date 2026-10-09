# Modifications to NeuroSim V1.4

This branch is based on `neurosim/NeuroSim`, branch `2DInferenceV1.4`
(base commit `8a88abf`). The original tool is by Prof. Shimeng Yu's group
(Georgia Tech) under CC BY-NC 4.0. Please cite:
J. Lee, A. Lu, W. Li, S. Yu, "NeuroSim V1.4: Extending Technology Support
for Digital Compute-in-Memory Toward 1nm Node", IEEE TCAS-I, 2024.

## Changes relative to upstream

| File | Change |
| --- | --- |
| `Inference_pytorch/NeuroSIM/Chip.cpp` | Count conv windows with "same" padding (new `numWindows()` helper) instead of the no-padding count |
| `Inference_pytorch/NeuroSIM/main.cpp` | Operation count uses real output positions (stride and same padding) |
| `Inference_pytorch/inference.py` | Per-batch progress output (batch, elapsed time, running accuracy) |
| `Inference_pytorch/models/dataset.py` | Default CIFAR-10 data root changed to a local path; edit it for your machine |
