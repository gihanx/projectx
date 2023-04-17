# Summery
- Development of a video game to adhere employees to follow Unilever functional
standards.

---
# U for Safe Drive
---
# Game Overview
---
# Branding
---
# Account System
---
# General
## Player Controller
### Locomotion/Movement

- [ ] Move Forward
	- [ ] Animation
		- Forward moving Leg/Arm
	- [ ] Logic
		- x
- [ ] Move Backward
	- [ ] Animation
		- Backward moving Leg/Arm animation 
	- [ ] Logic
		- x
- [ ] Move Left
	- [ ] Animation
		- Left moving Leg/Arm animation
	- [ ] Logic
		- x
- [ ] Move Right
	- [ ] Animation
		- Right moving Leg/Arm animation
	- [ ] Logic
		- x

### Vehicle Inspection Exterior
- [ ] Tire Check
	- [ ] Animation
		-  Ch kicks to tire w/ leg 
	- [ ] Logic
		- Press F
		- Move
		- Disable Input
		- Play Montage
		- Enable Input
- [ ] Bonet Open
	- [ ] Animation
		-  Cha opens bonet w/ hands
	- [ ] Logic
		- Press F
		- Disable User Input
		- Set Loc/Rot
		- Play Montage
		- Loop last frame
		- Prompt ==**RADIAL MENU**==
		- Enable mouse input
- [ ] Bonet Close
	- [ ] Animation
		- Ch close bonet w/ hands
	- [ ] Logic
		- Select **CLOSE BONET** from ==**RADIAL MENU**==
		- Disable mouse input
		- Close ==**RADIAL MENU**==
		- Play Montage
		- Set Loc/Rot
		- Enable user input
- [ ] Engine Check
	- [ ] Animation
		-  Ch touch engine
	- [ ] Logic
		- Select **CHECK ENGINE** from ==**RADIAL MENU**==
		- Close ==**RADIAL MENU**==
		- Disable mouse input
		- Play Montage
		- Enable mouse input
		- Prompt ==**RADIAL MENU**==
- [ ] Radiator Check
	- [ ] Animation
		-  Ch Pull Radiator
	- [ ] Logic
		- Select **CHECK RADIATOR** from ==**RADIAL MENU**==
		- Close ==**RADIAL MENU**==
		- Disable mouse input
		- Play Montage
		- Enable mouse input
		- Prompt ==**RADIAL MENU**==

### Vehicle Inspection Interior

- [ ] Mobile Phone Switch Off
- [ ] License put on Glove Box
- [ ] Side Mirrors Check
- [ ] Put Seat Belt 
- [ ] Gear Change
- [ ] Signal Light Knob
### Vehicle Enter/Exit
- [ ] Door Unlock
	- [ ] Animation
		- Key for Door
	- [ ] Logic
		-  x	      

- [ ] Helmet
    - [ ] Animation
	    - Wear Helmet
    - [ ] Logic
	    - x

- [ ] Enter
    - [ ] Animation
	    -  Character Enter
    - [ ]  Logic
        1. Press F
        2. Player Moves to Enter Location 
        3. Disable Userinput  
        4. Open Door 
        5. Player/Actor/Capsule/Mesh move to seat  
        6. Also plays the Anim w/ Rootmotion  
        7. Blend Player Cam to Vehicle Cam  
        8. Close Door  
        9. Posses the Car/Car Controls  
        10. Enable Steerwheel IK Hands  
- [ ] Exit
    - [ ] Animation
	     - Character Exit
    - [ ] Logic
        1. Press F 
        2. Disable IK Hands 
        3. Open Door
        4. Player/Actor/Capsule/Mesh move to EnterLoc  
        5. Also plays the Anim w/ Rootmotion -reverse
        6. Blend VehiclCam to Player Cam 
        7. Close Door 
        8. Posses the PlayerCharacter  
        9. Enable UserInput


### Vehicle Driving 
- [ ] Hand to Steerwheel
    Anim:
        Hands Blend
    Logic:
	 Enable IK Hands for Steerwheel
## Vehicle Component
- 
# Levels Overview
---
# Traning Level
---
# Road and Driving
---
# Level 1
---
# Player Staticstics
### Summarized Statistics
> A summary of the player progress statistics shown in the menu, up right corner

Reference:
> Marking Scheme
---
# Settings
### Controller Settings
### Graphics Settings
---
# Admin Dashboard
### Summerizied Statistics
---