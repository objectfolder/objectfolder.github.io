---
title: Object Manipulation Tasks
# subtitle: 
featured_image: 
---

### [Grasp-Stability Prediction](https://github.com/objectfolder/objectfolder_manipulation_tasks)

<html>
    <div style="display: flex;">
        <div style="flex: 4;">
            <p>
            The goal is to predict whether a robotic gripper can successfully grasp and stably hold an object between its left and right fingers based on either an image of the grasping moment from an externally mounted camera, a tactile RGB image obtained from the GelSight robot finger, or their combination. The grasp is considered failed if the grasped object slips by more than 3 cm.
            </p>
        </div>
        <div style="flex: 1; width: 100%;">
            <img src="assets/img/objectfolder/grasp_stability.jpg" alt="" style="max-width: 100%; height: auto;">
        </div>
    </div>
</html>



### [Contact Refinement](https://github.com/objectfolder/objectfolder_manipulation_tasks)

<html>
    <div style="display: flex;">
        <div style="flex: 4;">
            <p>
            Given an initial pose of the robot finger, the task is to change the finger’s orientation to contact the point with a different target orientation. Each episode is defined by the following: the contact point, the start orientation of the robot finger along the vertex normal direction of the contact point, and observations from the target finger orientation in the form of either a third view camera image, a tactile RGB image, or both. We use a continuous action space over the finger rotation dimension. The task is successful if the finger reaches the target orientation within 15 action steps with a tolerance of one degree.
            </p>
        </div>
        <div style="flex: 1; width: 100%;">
            <img src="assets/img/objectfolder/contact_refinement.jpg" alt="" style="max-width: 100%; height: auto;">
        </div>
    </div>
</html>


### [Surface Traversal](https://github.com/objectfolder/objectfolder_manipulation_tasks)
<html>
    <div style="display: flex;">
        <div style="flex: 4;">
            <p>
            Given an initial contacting point, the goal of this task is to plan a sequence of actions to move the robot finger horizontally or vertically in the contact plane to reach another target location on the object’s surface. Each episode is defined by the following: the initial contact point, and observations of the target point in the form of either a third-view camera image, a tactile RGB image, or both. The task is successful if the robot finger reaches the target point within 15 action steps with a tolerance of 1 mm.
            </p>
        </div>
        <div style="flex: 1; width: 100%;">
            <img src="assets/img/objectfolder/surface_traversal.jpg" alt="" style="max-width: 100%; height: auto;">
        </div>
    </div>
</html>

### [Dynamic Pushing](https://github.com/objectfolder/objectfolder_manipulation_tasks)
<html>
    <div style="display: flex;">
        <div style="flex: 4;">
            <p>
            Given example trajectories of pushing different objects together with their corresponding visual and tactile observations, the goal of this task is to learn a forward dynamics model that can quickly adapt to novel objects with a few contextual examples. With the learned dynamics model, the robot is then tasked to push the objects to new goal locations.
            </p>
        </div>
        <div style="flex: 1; width: 100%;">
            <img src="assets/img/objectfolder/dynamic_pushing.png" alt="" style="max-width: 100%; height: auto;">
        </div>
    </div>
</html>

