---
hide:
 - toc
 - path
 - title
---
## Player Controller
### Locomotion/Movement

- [ ] Move Forward
	- [ ] Animation
		- Walk forward
	- [ ] Logic
		- 
- [ ] Move Backward
	- [ ] Animation
		- Walk backward
	- [ ] Logic
		- 
- [ ] Move Left
	- [ ] Animation
		- Walk left
	- [ ] Logic
		- 
- [ ] Move Right
	- [ ] Animation
		- Walk right
	- [ ] Logic
		- 

### Vehicle Inspection Exterior
- [ ] Tire Check
	- [ ] Animation
		-  Leg kicks to tire 
	- [ ] Logic
		- Press F
		- Set Loc/Rot
		- Disable Input
		- Play Montage
		- Enable Input
- [ ] Bonnet Open
	- [ ] Animation
		-  Open bonnet with hands
	- [ ] Logic
		- Press F
		- Disable User Input
		- Set Loc/Rot
		- Play Montage
		- Loop last frame
		- Prompt ==**RADIAL MENU**==
		- Enable mouse input
- [ ] Bonnet Close
	- [ ] Animation
		- Close bonnet with hands
	- [ ] Logic
		- Select **CLOSE BONET** from ==**RADIAL MENU**==
		- Disable mouse input
		- Close ==**RADIAL MENU**==
		- Play Montage
		- Set Loc/Rot
		- Enable user input
- [ ] Engine Check
	- [ ] Animation
		-  Touch engine with left hand
	- [ ] Logic
		- Select **CHECK ENGINE** from ==**RADIAL MENU**==
		- Close ==**RADIAL MENU**==
		- Disable mouse input
		- Play Montage
		- Enable mouse input
		- Prompt ==**RADIAL MENU**==
- [ ] Radiator Check
	- [ ] Animation
		-  Pull radiator with left hand
	- [ ] Logic
		- Select **CHECK RADIATOR** from ==**RADIAL MENU**==
		- Close ==**RADIAL MENU**==
		- Disable mouse input
		- Play Montage
		- Enable mouse input
		- Prompt ==**RADIAL MENU**==

### Vehicle Inspection Interior

- [ ] Mobile Phone Switch Off
	- [ ] Animation
		- Take phone > switch it off > put it back
	- [ ] Logic
		- Disable user input
		- Play Montage
		- Enable user input
- [ ] License put on Glove Box
	- [ ] Animation
		- Take license > Look at it > Put in glove box
	- [ ] Logic
		- 
- [ ] Side Mirrors Check
	- [ ] Animation
		- 
	- [ ] Logic
		-  
- [ ] Put Seat Belt 
	- [ ] Animation
		- 
	- [ ] Logic
		-  
- [ ] Gear Change
	- [ ] Animation
		- 
	- [ ] Logic
		-  
- [ ] Signal Light Knob
	- [ ] Animation
		- 
	- [ ] Logic
		-  

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
	- [ ] AnimBP
		-  
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
	- [ ] Animation
		- Blend
	- [ ] Logic
		-  af

- [ ] Idle
	- [ ] Animation
		- 
	- [ ] Logic
		-  sdgv



## KineFX Control Rig

- Root
	- Root Bone
	- Root Motion

- Pelvis
	 - FK Spines
	 - Head
		 - Look at 
 
- Leg
	- *Reverse Foot*
	- FK Leg
		- Knee
		- Foot
	- IK Leg
		- Knee Pole
		- Foot

- Hand
	- *Realistic Shoulder*
	- FK Hand
		- Elbow
		- Wrist
		- Fingers 
	- IK Hand
		- Elbow Pole
		- Wrist
			- Pelvis/Root Constraint Switch  
	
 !!! note
 asdasd
 asd
 asd    fsdf
