# Unity tutorial - external models
## 1. Introduction to models
In Unity, models are files describing 3D objects. This includes their shape and appearance. Models are used to create for example characters or terrain, and are also able to create animations.

They often include textures or materials. It's common to create the models in external programs like Blender and then import them in Unity.

Unity provides the possibility to create prefabs - a model with presaved settings that can be reused for creating multiple instances of the same object.
## 2. Creating modes
Add your content here.
## 3. Importing models
In the [Unity asset store](https://assetstore.unity.com/?category=3d&free=true&orderBy=1), you can find many (also free) resources, including models. However, also [mixamo](https://www.mixamo.com) provides great resources.

It's best to import the model as a fbx file (best support). Furthermore, humanoid models should be in a T-pose, then several skinless animations can be added almost effortless.
### 3.1 Importing a model
There are several steps to import a model:
1. Open import settings window
    - Move the model and its animations to the asset folder in the project window.
    - Open the import setting window (opens up in inspector tab) by clicking on the model.
2. Set importer options
    - change scale
    - influence details to improve performance
    - activate colliders
    - decide what shall be imported (visibility, camera, lights)
3. Rigs and animation settings
    - differentiate between animation types humanoid and non-humanoid settings -> humanoid needs bone structure / avatar
    - avatar masking can be used to adjust the skeleton and also influence animations
4. Apply materials and textures
    - with fbx files, just extract both in the materials tab of the model

### 3.2 Special settings for humanoid models
5. In the Rig tab of the animation, change the animation type to humanoid
6. As avatar definition, choose "Copy from other avatar" and point to your model avatar
7. In the assets folder, create an Animator controller
8. Click on the Animator controller and drag and drop the animation
9. Drag and drop this animator controller in your models animator tab in the controller field

---

### Resources
- https://docs.unity3d.com/2023.3/Documentation/Manual/models.html
- https://www.youtube.com/watch?v=0QA2O7juuWQ