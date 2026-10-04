# Architecture and Design

## Design artefacts
1. `01_initial_architecture_from_proposal.png` - architecture captured in Assessment 1.
2. `02_final_high_level_system_architecture.png` - final implemented high-level architecture.
3. `03_final_workflow_diagram.png` - final end-to-end workflow.
4. `data_pipeline_architecture.png` / `.dot` - data movement from acquisition through versioned evidence.
5. `data_storage_design.png` / `.dot` - repository/file-based data storage design.
6. `component_interaction_diagram.png` / `.dot` - interaction among loader, preprocessing, training, validation, evaluation, artefact store and optional UI.
7. `deployment_architecture.png` / `.dot` - proof-of-concept deployment design; production deployment is explicitly out of scope.

## Architecture evolution
The final Potato architecture expands the proposal from a single CNN concept to a three-model comparison, introduces official leaf-group-disjoint splitting, validation-only threshold locking, untouched PlantDoc external evaluation, calibration, robustness, ablation, segmentation, Grad-CAM, efficiency analysis and a safeguarded research interface.

The `.dot` files are editable diagram sources and can be opened/converted with Graphviz. PNGs are provided for reports and GitHub viewing.
