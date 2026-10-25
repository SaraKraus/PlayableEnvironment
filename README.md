# Bat Game

An unsettling forest with danger lurking around every corner. Developed with Unreal Engine 5. 


## **Open The Project:**

1. Install Unreal Engine 5.8
2. Clone/download the repository and extract it if needed.
3. Open PlayableEnvironment.
4. Wait for shaders to compile, then press Play.
5. L_MainMenu is the first level that you're loaded into


## **Build it:**

1. Open the project and save everything.
2. In Project Settings > Packaging, use the Shipping configuration.
3. From the Platforms menu, select Windows and Package Project.
4. Choose an output folder and wait for packaging to finish.


## **Play the packaged game**

1. Download it here: https://golabekk.itch.io/bat-game
2. Extract the whole ZIP.
3. Open the Windows folder and run PlayableEnvironment
4. Keep all the included files and folders together.


## **Controls**

- WASD = move
- Mouse = look
- Space = jump
- Ecs/P = Pause
- Shift = Sprint
- F = Flashlight


## **Requirements**

### **Variables:**
1. Within BP_HitBox: 
- PointLight
- Box
- DefaultSceneRoot

2. Within BP_ThirdPersonPlayerController:
- Touch Controls Widget Class
- Force Touch Controls

3. Within BP_ThirdPersonCharacter:
- Camera: FollowCamera, CameraBoom
- Components: BP_Flashlight
- Flashlight Ref
- As BP Flashlight
- HP
- As Player Controller
- Stamina
- Sprint?

### **Events:**
1. Within BP_ThirdPersonCharacter:
- EnhancedInputAction IA_Jump
- EnhancedInputAction IA_Move
- EnhancedInputAction IA_Look
- Event Secondary Thumbstick
- EnhancedInputAction IA_MouseLook
- Event Primary Thumbstick
- Event Touch Jump Start
- Event Touch Jump End
- EnhancedInputAction IA_Flashlight
- Event BeginPlay
- HitPlayer
- Event Destroyed
- Stamina+
- Ragdoll Event

2. Within BP_ThirdPersonPlayerController:
- Even BeginPlay
- RespawnPlayer

3. Within BP_HitBox:
- Event BeginPlay
- Event ActorBeginOverlap
- Event Tick
- On Component Begin Overlap (Box)

### **Functions**
1. Within BP_ThirdPersonPlayerController: 
- Construct Script
- Should us touch controls

2. Within BP_ThirdPersonCharacter:
- Construction Script
- Move
- Aim

### **Loops:**
1. Within BP_ThirdPersonCharacter:
- Stamina constantly replenishes until it hits 100

### **Branches:**
1. Within BP_ThirdPersonCharacter:
- Deals Damage to Player: The branch allows the actor to be destroyed if its true

### **Triggers:**
- Upon walking into the hitbox the player takes damage
- Upon walking into teleportation collision the player gets teleported
- Upon walking into sound effect collider a sound effect plays

### **Object Casting:**
- Within Blueprints

### **Debugging:**
- Used to have E key binded to respawn player up until I had it be automated whenever player dies
- You can pause the game with both Esc and P because in order for me to test it within unreal I had to have the input be bound to a key other than esc
- Upon entering the sound effect collider a string was printed

1. Within BP_ThirdPersonCharacter:
- Deals Damage to Player: When player takes damage a string is printed in the top left showing how much hp you are now on

### **Asset Importing:**
1. Structures:
- decimus_burton_church
- medieval_fountain_empty_free
- medieval_houses_10

2. Additional:
- SM_Section1
- SM_Gate
- flash_light

### **Terrain**
- Very detailed texturing and sculpt
- Used Foliage tool

### **Moddeling Tools:**
- Used on the gravestones

### **UI Elements:**
- HP bar
- Stamina bar
- Pause Menu
- Main Menu
---
**PLUS MORE**

---
## **Credits**
Listed on itch: https://golabekk.itch.io/bat-game

