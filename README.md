#  Shudder [[runnable]](https://github.com/Possibility-1B/Possibility/releases/tag/Java8Binarries)


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
   git clone https://github.com/jwihardi/Shudder.git
```

Our .gitignore is from GitHub's [UnrealEngine.gitignore](https://github.com/github/gitignore/blob/main/UnrealEngine.gitignore).

---

## 🎮 Default Controls

| Key                     | Action              |
|-------------------------|---------------------|
| `W` or `⭡`              | Move Forward        |
| `A`                     | Move Left           |
| `S` or `↓`              | Move Backward       |
| `D`                     | Move Right          |
| `SHIFT`                 | Sprint              |  
| `_`                    | Jump                |
| `E`                     | Interact            |  
| `H`                     | Hide                |  
| `F`                     | Turn on Flashlight  |  
| `Esc`                   | Pause/Menus         |  

---



## 📋 Menus
<div style="display: flex; justify-content: space-around;">
  <img align="left" src="https://github.com/user-attachments/assets/093557cd-e24b-41e2-bb27-dd044dad2f44" width = "47%"/>
  <img align = "right" src="https://github.com/user-attachments/assets/9fc661b1-a1d3-40f7-8de2-5903765ad982" width= "47%"/>
</div>   
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

<div style="display: flex; justify-content: space-around;">
  <img align="left" src="https://github.com/user-attachments/assets/5c644e07-4b2c-4050-8ec4-200462c21c9d" width = "47%"/>
  <img align = "right" src="https://github.com/user-attachments/assets/5f6f939d-8c5d-4639-b98f-889f47c8fd78" width= "47%"/>
</div>   
<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>

---

## 🚀 Things We Should Have Done

While this project served as a great learning experience, there are many areas that could have been improved:

- **Audio**: The player has a "wood sounding" footstep which doesn't change in the basement and garage which had different materials. The jumpscare and death sound aren't very impactful and could have been better. The menu music isn't really eerie or matching either. Some more organic sounds should have been incorporated, such as groans that come from the monster.

- **Movement**: The movement feels awkward. The FOV is too low and makes it confusing when turning around in a small area. Turning feels slightly delayed, though this isn't a big deal since it's not an FPS game.

- **Map Design**: The map design is a little lack luster. There should be more clutter to make it feel more like a house, such as curtains blowing in the wind. The window texture is too clear, it doesn't look like there is even a window frame. There are also some issues regarding lighting and the map, some areas seem lit even when there is no light on.

- **Multiplayer**: This feature should have been completely removed. Multiplayer doesn't work at all since everything is client-sided and desynced, although players can join each other locally.

- **Assets**: More assets should have been custom-made rather than using online free assets since many don't fit quite right. The stairs were extremely hard to make work since the monster's pathfinding wouldn't go up it if it was too steep and neither could the player. The light switches don't animate which could have easily been added.

---


## 📄 License

This project is under the MIT [License](./LICENSE).

