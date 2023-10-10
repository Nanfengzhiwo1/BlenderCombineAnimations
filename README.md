# Preface
> **_The famous 5-star American general , MacArthur once said, "Don't use two animations for what one animation can accomplish!" This statement quickly attracted widespread attention from all sectors of society......_**
# Prompt
- Blender Version：3.6.4
- Animation: Run and Walk(UE5 Manny)
# Why these animations were chosen as examples
- They 're easy to get
- Their animations are not related
- These animations all have displacement, and blending them requires modifying the initial position
# Base Mannual
- [3D Viewport](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/1)
- [Outliner](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/2)
- [Timeline](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/3)
- [Dope Sheet - Action Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/4)
- [Nonlinear Animation](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/5)
- [Graph Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/6)
- [Pose Mode](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/7)
- [Pose - Animation - Bake Action](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/8)
- [Export](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/9)
# Operating manual
- [Split Area](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/10)
# How to start
### Step1
* In [Outliner](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/2), Press **A** to select all,
*  and press **Delete** to delete all
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/15297cdf-f7c2-48f4-8003-3ae1799f7e34)

### Step2
* Import two animations and rename to 'Walk' and 'Run',you can play animations in [Timeline](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/3),
* in Outliner choose the 'Walk' ,and  hide the 'Run'( eye icon has closed)
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/83718d97-dc45-4246-ae85-b1583bfe166e)

### Step3
* [Split a new area](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/10),
* you have two areas, change the top one to [Action Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/4)and the bottom one to [Nonlinear Animation](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/5)
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/bbc54883-335c-4196-80ca-10b030afc0c8)

### Step4
* rename the collection of F-Curves to 'Walking',
* and then push down
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/c158ef44-c1e9-4a7a-82a1-57335ca0219c)

### Step5
* Click the button ,select other ,
* rename to 'Running' and push down
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/9f271658-f561-4107-993b-ca4cb4fb29b2)

### Step6
* Click 'Running',Press **G** and move it to 'Walking' 's Frame End,
* Extrapolation:Hold->Hold Forward,Blend in:10;
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/138555ef-5b12-4d58-ab8e-b533cac6caf7)

> **when you check the two animations,the character in 3D Viewport will step back because [Graph Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/6) has not been modified yet**  

### Step7
* In top area,Press **Shift**+**F6**,Open [Graph Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/6).
* Click 'Walking',Press **Tab**,search the data of the last frame of 'Y Location' under 'root',click eye icon to hide others
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/88f12bf2-28d2-40b5-b6ff-1bf578be6ddd)

### Step8
* Click 'Running',Press **G** ,Set the value of the last frame as the Cursor Y's initial value.
* Move all keyframes down by the corresponding distance(The second animation should start from the end position of the first animation, not from 0)
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/95efb808-190c-40e5-ab34-01c37e80b513)


### Step9!!!
* In bottom area, press **A**,select all animations.
* Change 'Object Mode' to 'Pose Mode',click 'pose'-'Animation'-'Bake Action...'
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/599c6e46-a4cf-44bd-a8d0-a905a807295d)

### Step10
* Modify the end frame，
* Bake Data select Pose and Object,**Shift-Click** to select multiple,click 'OK'
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/022924ed-3a33-4a78-bbb4-bef8663a9be4)

### Step11
* Delete 'Running' and 'Walking',push down the new animation
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/93f40799-e98e-42f3-941d-856120c0baa6)

### Step12
* In Outliner,delete 'Run'
* Export as FBX，export selected objects and do not add leaf bones
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/4d47b3f9-7ff4-4936-a991-46321401a3f7)
# Preview


https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/d8e1b3ba-3f21-4a10-945c-b9b775a96877

