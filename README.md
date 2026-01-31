# fetch-table-setup-ai
This repository contains a Fetch mobile manipulator control model and task definition for setting up a table in ManiSkill / MS-HAB simulation environments.
The model follows the official AI Fetch Interface specification and is compatible
with `pd_joint_delta_pos` control mode.

## Robot
- Fetch Mobile Manipulator

## Task
- Setup the table
- Place plates, cups, and utensils
- Arrange items neatly on the table surface

## Observation Mode
- state (flattened tensor or dictionary)

## Input
- Shape: (state_dim,) or (batch_size, state_dim)
- Data type: float32

## Output
- Shape: (13,)
- Range: [-1.0, 1.0]
- Control:
  - 7 arm joints
  - 1 gripper
  - 3 body joints
  - 2 base velocity controls

## Control Mode
- pd_joint_delta_pos

## Framework
- PyTorch

## Status
Submitted for AI Miner onboarding and Fetch robot evaluation.

## Author
GitHub: https://github.com/Aanika03
