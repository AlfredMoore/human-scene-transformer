### input batch

1. ~~'agents/keypoints': agent_keypoint~~  (now removed due to high bandwidth and low contribution)
2. 'agents/position': agent_position
    * detection data box3d containing: cs, cy (coordinate x forward, y left, z up)
3. 'agents/orientation': agent_orientation
    * * detection data box3d containing: rot_z (coordinate x forward, y left, z up)
4. 'robot/position': robot_position
5. 2d map data: how to integrate this to the transformer
