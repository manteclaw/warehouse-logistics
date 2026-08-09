<!--
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Warehouse Robotics and Logistics",
  "description": "Robotics manipulation dataset for warehouse automation, including grasp poses, trajectories, sensor readings, and task execution metrics.",
  "creator": {"@type": "Organization", "name": "Manteclaw"},
  "license": "https://opensource.org/licenses/MIT",
  "distribution": {"@type": "DataDownload", "contentUrl": "https://payhip.com/Manteclaw"}
}
</script>
-->
[![Get Full Dataset](https://img.shields.io/badge/Get%20Full%20Dataset-Payhip-10b981?style=for-the-badge)](https://payhip.com/Manteclaw)

## 📊 Quick Stats

| 📁 Records | 📄 Files | 📐 Columns | 💾 Size | 💰 Price |
|:----------:|:--------:|:----------:|:-------:|:--------:|
| 2,000 | 3 | 17 | ~200 KB | $50 |

![Records](https://img.shields.io/badge/records-2000-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Price](https://img.shields.io/badge/price-50-brightgreen)

# Warehouse Robotics and Logistics

Robotics manipulation dataset for warehouse automation, including grasp poses, trajectories, sensor readings, and task execution metrics.

## Dataset Overview

## Data Dictionary

| Field | Type | Description |
|-------|------|-------------|
| task_type | string | pick-and-place, sorting, palletizing |
| robot_type | string | 6DOF, SCARA, Delta, Cobot |
| trajectory_waypoints | array | Joint angle sequences |
| grasp_pose_6dof | array | Position + orientation |
| gripper_force | float | Newtons applied |
| success_rate | float | 0-1 success probability |
| execution_time_sec | float | Task duration |
| sensor_readings | object | RGB, depth, force-torque |
| object_type | string | Cube, cylinder, gear, etc. |
| failure_mode | string | Type of failure if any |



| Property | Value |
|----------|-------|
| **Total Records** | 2,500 |
| **Sample Included** | 100 rows |
| **License** | CC-BY-SA-4.0 |
| **Price (Full)** | $39 |

## Purchase Full Dataset

The complete dataset (2,500 records) is available for purchase:

- **Store:** [https://payhip.com/Manteclaw](https://payhip.com/Manteclaw)
- **Email:** manteclaw@proton.me

## Files

| File | Description |
|------|-------------|
| `sample_data.csv` | 100-row representative sample |
| `metadata.json` | Dataset schema, tags, pricing |
| `notebooks/starter.ipynb` | Jupyter notebook for exploration |

## Sample Preview (first 10 rows)

| id | task_type | robot_type | object | grasp_pose | trajectory | sensor_readings | execution_time_ms | success | failure_mode | collision_detected | workspace_constraints | environment | lighting | timestamp | data_source | is_synthetic |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| ROBO-000457 | bin_picking | 6dof_arm | {'type': 'chip_package', 'material': 'wood', 'mass_kg': 1... | {'position': {'x': -0.4144, 'y': 0.0265, 'z': 0.1655}, 'o... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [-... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 2726 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | outdoor | uv | 2026-08-08T00:01:52.632343+00:00 | synthetic_robotics_simulation | True |
| ROBO-000103 | pick_and_place | scara | {'type': 'screw', 'material': 'ceramic', 'mass_kg': 2.209... | {'position': {'x': 0.2461, 'y': 0.2746, 'z': 0.091}, 'ori... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [-... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 7273 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | lab | ir | 2026-08-08T00:01:52.525818+00:00 | synthetic_robotics_simulation | True |
| ROBO-001127 | quality_check | magnetic_gripper | {'type': 'cylinder', 'material': 'rubber', 'mass_kg': 2.8... | {'position': {'x': 0.2329, 'y': -0.4331, 'z': 0.653}, 'or... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [0... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 1620 | False | collision | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | kitchen | ir | 2026-08-08T00:01:52.702409+00:00 | synthetic_robotics_simulation | True |
| ROBO-001004 | pick_and_place | delta | {'type': 'screw', 'material': 'aluminum', 'mass_kg': 0.55... | {'position': {'x': -0.0041, 'y': 0.3985, 'z': 0.0975}, 'o... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [2... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 7880 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | warehouse | variable | 2026-08-08T00:01:52.688412+00:00 | synthetic_robotics_simulation | True |
| ROBO-000915 | assembly | magnetic_gripper | {'type': 'chip_package', 'material': 'glass', 'mass_kg': ... | {'position': {'x': -0.4425, 'y': -0.4719, 'z': 0.6517}, '... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [2... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 6544 | True | None | True | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | factory | bright | 2026-08-08T00:01:52.678413+00:00 | synthetic_robotics_simulation | True |
| ROBO-000572 | surface_cleaning | delta | {'type': 'cylinder', 'material': 'silicone', 'mass_kg': 2... | {'position': {'x': 0.4051, 'y': 0.3598, 'z': 0.1864}, 'or... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [-... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 4494 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | warehouse | uv | 2026-08-08T00:01:52.643343+00:00 | synthetic_robotics_simulation | True |
| ROBO-000420 | bin_picking | parallel_gripper | {'type': 'sphere', 'material': 'carbon_fiber', 'mass_kg':... | {'position': {'x': 0.48, 'y': 0.1198, 'z': 0.066}, 'orien... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [-... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 7087 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | warehouse | ir | 2026-08-08T00:01:52.616343+00:00 | synthetic_robotics_simulation | True |
| ROBO-002234 | sorting | cobot | {'type': 'bearing', 'material': 'silicone', 'mass_kg': 3.... | {'position': {'x': -0.2125, 'y': -0.4112, 'z': 0.2175}, '... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [-... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 3479 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | warehouse | ir | 2026-08-08T00:01:52.936018+00:00 | synthetic_robotics_simulation | True |
| ROBO-000357 | bin_picking | delta | {'type': 'bottle', 'material': 'aluminum', 'mass_kg': 1.7... | {'position': {'x': 0.0769, 'y': -0.3457, 'z': 0.015}, 'or... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [1... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 5897 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | kitchen | ir | 2026-08-08T00:01:52.582344+00:00 | synthetic_robotics_simulation | True |
| ROBO-002419 | packaging | parallel_gripper | {'type': 'cube', 'material': 'rubber', 'mass_kg': 3.638, ... | {'position': {'x': -0.3162, 'y': 0.0673, 'z': 0.6053}, 'o... | [{'waypoint_id': 0, 'timestamp_ms': 0, 'joint_angles': [1... | {'camera_rgb': {'resolution': [640, 480], 'object_detecte... | 802 | True | None | False | {'x_min_m': -0.8, 'x_max_m': 0.8, 'y_min_m': -0.6, 'y_max... | lab | bright | 2026-08-08T00:01:52.956027+00:00 | synthetic_robotics_simulation | True |

## License

This dataset is licensed under [CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/).

## Citation

```bibtex
@dataset{warehouse_logistics_2026,
  title        = {Warehouse Robotics and Logistics},
  author       = {Manteclaw},
  year         = {2026},
  url          = {https://github.com/manteclaw/warehouse-logistics},
  license      = {CC-BY-SA-4.0},
  note         = {Sample dataset. Full version available at https://payhip.com/Manteclaw},
}
```

---
*Dataset curated by [Manteclaw](https://github.com/manteclaw). For inquiries: manteclaw@proton.me*

## More Datasets from Manteclaw

| Dataset | Records | Price | Link |
|---------|---------|-------|------|
| DeFi Protocol Risk Metrics | 1,639 | $49 | [GitHub](https://github.com/manteclaw/defi-risk) |
| Drug Interaction & Pharmacology | 2,231 | $35 | [GitHub](https://github.com/manteclaw/pharmacology) |
| Warehouse Robotics & Logistics | 2,000 | $50 | [GitHub](https://github.com/manteclaw/warehouse-logistics) |
| LLM Safety & Red Teaming | 2,000 | $49 | [GitHub](https://github.com/manteclaw/llm-safety) |
| Crypto Quant Trading Signals | 1,500 | $69 | [GitHub](https://github.com/manteclaw/crypto-quant) |
| Cybersecurity Intrusion Detection | 2,000 | $49 | [GitHub](https://github.com/manteclaw/cybersecurity-intrusion) |

**All datasets available at:** https://payhip.com/Manteclaw


---

**Keywords:** dataset, machine learning, robotics, Base L2, AI agents
