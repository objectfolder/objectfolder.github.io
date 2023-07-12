---
title: Object Recognition Tasks
# subtitle: 
featured_image:
---

### [Cross-Sensory Retrieval](https://github.com/objectfolder/cross-sensory-retrieval)

<html>
    <div style="display: flex;">
        <div style="flex: 4;">
            <p>
            Cross-sensory retrieval requires the model to take one sensory modality as input and retrieve the corresponding data of another modality. For instance, given the sound of striking a mug, the “audio2vision” model needs to retrieve the corresponding image of the mug from a pool of images of hundreds of objects. In this benchmark, each sensory modality (vision, audio, touch) can be used as either input or output, leading to 9 sub-tasks.
            </p>
        </div>
        <div style="flex: 1; width: 100%;">
            <img src="assets/img/objectfolder/retrieval.png" alt="" style="max-width: 100%; height: auto;">
        </div>
    </div>
</html>


### [Contact Localization](https://github.com/objectfolder/contact-localization)

<html>
    <div style="display: flex;">
        <div style="flex: 4;">
            <p>
            Given the object’s mesh and different sensory observations of the contact position (visual images, impact sounds, or tactile readings), this task aims to predict the vertex coordinate of the surface location on the mesh where the contact happens.
            </p>
        </div>
        <div style="flex: 1; width: 100%;">
            <img src="assets/img/objectfolder/contact_localization.png" alt="" style="max-width: 100%; height: auto;">
        </div>
    </div>
</html>


### [Material Classification](https://github.com/objectfolder/material-classification)

<html>
    <div style="display: flex;">
        <div style="flex: 4;">
            <p>
            All objects are labeled by seven material types: ceramic, glass, wood, plastic, iron, polycarbonate, and steel. The task is formulated as a single-label classification problem. Given an RGB image, an impact sound, a tactile image, or their combination, the model must predict the correct material label for the target object.
            </p>
        </div>
        <div style="flex: 1; width: 100%;">
            <img src="assets/img/objectfolder/material_classification.png" alt="" style="max-width: 100%; height: auto;">
        </div>
    </div>
</html>


