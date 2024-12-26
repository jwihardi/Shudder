# ☯ Shudder [[runnable]](https://github.com/Possibility-1B/Possibility/releases/tag/Java8Binarries)


<div style="display: flex; justify-content: space-around;">
  <img align="left" src="https://github.com/user-attachments/assets/b3f574e9-09a8-4b91-b0a5-8a327e5b7e2f" width="47%"/>
  <img align = "right" src="https://github.com/user-attachments/assets/a71e8b26-1326-4b52-b354-e6bd111e182e" width="47%"/>
</div>   
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

_Shudder_ is a 3D game created for our highschool senior project by a team of 2 utilizing Blender and Unreal Engine 5. This was our capstone project, so it was a cumulation of all the knowledge we've learned for three years, AP Computer Science Principles, AP Computer Science A, and the first half of out C++ class (the class this was made for).

## 📜 Description

_Shudder_ is a 3D horror/puzzle game consisting of one level, a house. The player has to manage the battery of their flashlight, not using it too much, and pick up batteries when necessary. To get out, there is one main puzzle utilizing the color wheel, Morse Code, and alphabetical numeration. Completing these puzzles gives you the padlock code to escape the house. While the player is doing all of this, there is an AI monster roaming around that will reset progress if the player is killed. The player has some methods to hide from the monster, such as hiding in beds, closets, and closing doors since the monster cannot open doors.

For this project we were tasked with making the process as "industry like" as possible, having a manager, company name, tasks, etc. We name our company, _Rat Man Games_ and kept track of our tasks through [Trello](https://trello.com).

### Features:
- **Monster**: An AI monster that roams around the house. Once the monster sees the player, it will give chase even after breaking the line of sight for a while. It will also check closets randomly and flip light switches when passing by. It will occasionally make eerie sounds and a single footstep.
  
- **Player**: The player can do default movements: walk in all directions, sprint while having stamina, and jump. The player can interact with interactables via the specified keybinds (E to pickup | H to hide). 

- **Flashlight/Battery**: A interactable flashlight that the player will pick up to illuminate dark spaces. The flashlight is not infinite and the player will need to pick up batteries to recharge it.

- **Lights/Light Switches**: Instead of wasting flashlight battery, the player can turn on overhead lights with light switches. 

-  **Closets**: A space that the player can hide in, although the monster might open closets and check inside.

-  **Beds**: Similar to the **Closet**, however they are more sparingly places around the house and the monster will not check under them.

-  **Radios**: They are scattered around the house and will play a letter in Morse Code.

-  **Note Cards**: An object that displays text or images that can be picked up momentarily for a clear view.

-  **Keys**: Some doors are locked so the player must pick up keys to open them.

-  **Drawer**: An interactable dresser with drawers that can have items played within.

-  **Settings**: A menu allows the player to customize their experience, such as fullscreen/windows, 4 resolutions, 5 FPS settings, post-processing, anti-aliasing, texture quality, shadow quality, and volume and sensitivity sliders. There is also a **key binds** subsetting allowing the player to change the interact, hide, sprint, jump, flashlight, and pause key binds.

-  **Saving**: Progress is automatically saved every 30 seconds and the player can resume their session by pressing "Continue" instead of "New Game".

---
## ⧸⧸ Cloning _Shudder_

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

