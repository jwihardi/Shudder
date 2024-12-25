# ☯ Shudder [[runnable]](https://github.com/Possibility-1B/Possibility/releases/tag/Java8Binarries)

<div style="display: flex; justify-content: space-around;">
  <img align="left" src="https://github.com/user-attachments/assets/05b214e7-a524-41a1-924f-ab4537dc0abc" width="47%"/>
  <img align = "right" src="https://github.com/user-attachments/assets/4ae1b347-0dfd-4321-b615-e6706b8f8586" width="47%"/>
</div>   
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

_Possibility_ is a 2D game developed as part of a themed senior high school project (2022) by a team of three collaborators. The theme was duality which we translated into the game using Java and Slick2D through the mechanics of reversing gravity.

## 📜 Description

_Possibility_ is a 2D side scroller and platformer consisting of 8 levels where the player has to obtain a key to pass through the level door. 

### Features:
- **Gravity Switch**: A box interactable with an arrow indicating which way gravity will be flipped. There is a cooldown at the bottom left of the screen that shows when you can flip gravity again.
  
- **Spike**: A triangular obstacle that will kill the player if touched. There are stationary spikes and moving spikes, which activate once the player passes the x-coordinate of the spike.

- **Ice**: A rectangular obstacle, usually embedded into the floor, that will freeze horizontal movement until the player leaves the ice.

-  **Surfboard**: A box-shaped obstacle that moves very freely when the player stands on top of it. Gravity affects the surfboard, but not as much as it does with the player.

---
## ⧸⧸ Cloning _Possibility_

   ```bash
   git clone https://github.com/Possibility-1B/Possibility.git
```

Make sure to set the res folder as a source folder.

---

## 🎮 Controls

| Key                     | Action              |
|-------------------------|---------------------|
| `W` or `⭡`              | Move Up             |
| `A` or `←`              | Move Left           |
| `S` or `↓`              | Move Down           |
| `D` or `→`              | Move Right          |
| `_ `or `W` or `↑`       | Jump                |
| `E`                     | Interact            |  

---

## 📸 Media
<div style="display: flex; justify-content: space-around;">
  <img align="left" src="https://github.com/user-attachments/assets/5167ea94-3f0e-4513-b3b8-ad09b712a455" width = "47%"/>
  <img align = "right" src="https://github.com/user-attachments/assets/6e9c4696-91cf-4db5-be4a-a80f207dc80a" width= "47%"/>
</div>   
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

---

## 🚀 Things We Should Have Done

While this project served as a great learning experience, there are many areas that could have been improved:

- **Audio**: There was no audio, although we did start writing code for it.
  
- **Hard Code**: The levels are hard coded a little too much, especially level 8. Code for the levels could be greatly simplified and reduced.

- **Gravity**: Originally the whole map was the rotate but we couldn't figure that out. Gravity changed horizontally could have been a nice touch.

- **Action Listener**: We should've code the controls you don't have to click at the exact moment, but can click a little before. 

- **Menu Buttons**: Some of the menu buttons don't work and need to be clicked several times - only the death menu.

- **Static**: At the time of the project, we didn't really understand what static did and would make mostly everything static because Eclipse would tell us.

- **Surfboard**: Originally the surfboard was supposed to be a push box, but the push block code made a surfboard instead.

-  **Level Design**: The level design is mostly lacking and there are only 8 levels.

---

## 🧹 Post Completion Cleanup

Cleanup was done after completion of Possibility, limited functionality changes were implemented.

- **Usage**: [UCDetector](https://marketplace.eclipse.org/content/unnecessary-code-detector) was used to find and remove unecessary code.

- **Modifiers**: [UCDetector](https://marketplace.eclipse.org/content/unnecessary-code-detector) was used to located and change unnecessary modifiers.

- **Imports**: Unecessary imports were removed. Imports were changed to be sorted from top to bottom: packages, classes, third-party libraries, and Java libraries.

- **Attributes**: Class attributes were organized in order from top to bottom in memory size then objects. Depending on context, variables were converted to single line declarations versus multiple lines.

- **Media**: The media classes [AnimationLoader.java](https://github.com/Possibility-1B/Possibility/blob/main/src/Media/AnimationLoader.java) and [ImageLoader.java](https://github.com/Possibility-1B/Possibility/blob/main/src/Media/ImageLoader.java) were altered to use a HashMap instead of multiple variables. File paths were changed to be Jar friendly using getResourceAsStream().

- **Level Completion**: Originally there was a variable keeping track of level completion to enforce levels had to be completed in succcession but wasn't ever used. This was fixed.
  
---

## 📚 Libraries [[download]](https://github.com/user-attachments/files/17930581/libs.zip)
<pre
    <b>
• Slick2D           • LWJGL (core | util | applet)           • IBXM           • JInput           • JNLP   
        
• JOGG              • JOrbis                                 • TinyLinePP     • DirectInput      • OpenAL
    </b>
</pre>

---


## 📄 License

This project is under the MIT [License](./LICENSE).

