### input batch

1. ~~'agents/keypoints': agent_keypoint~~  (now removed due to high bandwidth and low contribution)
2. 'agents/position': agent_position
    * detection data box3d containing: cs, cy (coordinate x forward, y left, z up)
3. 'agents/orientation': agent_orientation
    * * detection data box3d containing: rot_z (coordinate x forward, y left, z up)
4. 'robot/position': robot_position
5. 2d map data: how to integrate this to the transformer


Ideas:
1. from Chris, treat the robot as human and pick a predicted path as local traj trade-off the global goal.
2. More in AI, GAN like model, predict human intention as an encoder, decode human intention to human path. Utilize this to robot goal to robot end effector traj.
3. How to represent the human intention? A designated reward function, a representation factor, a latent space? RLHF may be a good way?