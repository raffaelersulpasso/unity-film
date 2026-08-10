BodyPoser - Quick Pose Editing and Scene Dressing Tool

This package includes the BodyPoser system, designed for fast and intuitive posing of humanoid models directly in the Unity Editor. Ideal for setting up static corpse scenes, cinematic moments, or decorative character placement without the need for animations or complex physics setups.

───────────────────────────────────────
📦 INCLUDED:

- BodyPoser.cs (Main Script)
- BodyPoserEditor.cs, inside the mainscript for convenience. (Editor Integration) 
- DemoScene (Example setup with pre-posed models and one ragdoll for interaction and tryout)
---------------------------------------

Preperation:
In the demo scene you can simply use the demo model. FOr your own models please read below:

───────────────────────────────────────
🛠 USAGE INSTRUCTIONS:

1. Attach the BodyPoser script to any humanoid character or ragdoll.
2. There are two ways to pose models:
	2.1 ragdoll posing. Make sure the model has a ragdoll. Start game mode and let the ragdoll be effected by gravity. If you are happy with the pose see step 3.
	2.2 In the Inspector, enable **Pose Edit Mode** to manipulate bones directly in the Scene View. If you are happy with the pose see step 3.
3. Use the provided buttons in the Inspector to:
   - 📸 **Capture Current Pose**: Save the current bone positions to JSON. In case of ragdoll do this during playmode and then turn off game mode.
   - 📐 In editor mode: **Apply Stored Pose**: Load a previously stored pose from JSON.
   - 🗑️ In editor mode:**Clear Stored Pose**: Delete stored pose data.
   - ⚙️ In editor mode:**Remove Physics Components**: Remove Rigidbodies and Colliders to keep the model static.

4. The **Disable Physics On Start** option to automatically freeze physics at runtime. (Use if you kept the physics compontens but want them disabled)

Tips:
- For maximum performance remove the physics elements and make the object static.


───────────────────────────────────────
📖 IMPORTANT WORKFLOW NOTES:

- If you are simply **posing static models for scene decoration**, you do **NOT** need to capture a pose. Just manipulate the model directly in the editor and save the scene.
- Use **Capture Pose** only if:
   - You want to save a ragdoll pose *after a physics simulation*.
   - You plan to apply stored poses dynamically during gameplay.

- Captured poses are stored as JSON files in `Assets/TempPoseData/` and are intended for temporary use unless needed for runtime applications.

───────────────────────────────────────
📧 SUPPORT:

Contact: revolvinggearstudios@gmail.com  
Join our Discord: https://discord.gg/g5fK7Df  

Enjoy and happy scene dressing!

