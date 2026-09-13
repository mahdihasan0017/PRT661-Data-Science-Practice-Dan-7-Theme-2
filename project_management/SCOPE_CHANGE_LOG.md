# Scope Change Log

| Change | Reason / evidence | Impact |
|---|---|---|
| Added traditional Logistic Regression baseline | Feedback required a traditional comparator | Added interpretable baseline evidence. |
| Added leaf-group-aware splitting | Prevent related captures of the same leaf crossing splits | Stronger leakage control than ordinary image-level splitting. |
| Added MobileNetV2 transfer learning alongside PotatoCNN | Stronger comparative benchmark | Added staged fine-tuning and efficiency comparison. |
| Locked checkpoints/thresholds on validation data only | Prevent test/external tuning | Improved evaluation integrity. |
| Added untouched PlantDoc external evaluation | Test domain generalisation beyond PlantVillage | Revealed field-domain shift without retuning. |
| Added calibration, robustness, ablation, segmentation, Grad-CAM and efficiency analyses | Reliability/explainability feedback | Expanded diagnostics and limitations. |
| Added safeguarded research interface | Demonstrate complete proof of concept | Explicitly non-diagnostic and non-production. |
