# Preface
> **_The famous 5-star American general , MacArthur once said, "Don't use two animations for what one animation can accomplish!" This statement quickly attracted widespread attention from all sectors of society......_**
# Prompt
- Blender Version：3.6.4
- Animation: Run and Walk(UE5 Manny)
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
1.In [Outliner](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/2), Press **A** to select all, and press **Delete** to delete all
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/15297cdf-f7c2-48f4-8003-3ae1799f7e34)
2.Import two animations and rename to 'Walk' and 'Run',you can play animations in [Timeline](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/3),in Outliner choose the 'Walk' ,and  hide the 'Run'( eye icon has closed)
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/83718d97-dc45-4246-ae85-b1583bfe166e)
3.[Split a new area](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/10),you have two areas, change the top one to [Action Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/4)and the bottom one to [Nonlinear Animation](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/5)
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/bbc54883-335c-4196-80ca-10b030afc0c8)
4.rename the collection of F-Curves to 'Walking',and then push down
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/c158ef44-c1e9-4a7a-82a1-57335ca0219c)
5.Click the button ,select other ,rename to 'Running' and push down
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/9f271658-f561-4107-993b-ca4cb4fb29b2)
6.Click 'Running',Press **G** and move it to 'Walking' 's Frame End, Extrapolation:Hold->Hold Forward,Blend in:10;
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/138555ef-5b12-4d58-ab8e-b533cac6caf7)

> **when you check the two animations,the character in 3D Viewport will step back because [Graph Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/6) has not been modified yet**  

7.In top Area,Press **Shift**+**F6**,Open [Graph Editor](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/issues/6).Click 'Walking',Press **Tab**,search the data of the last frame of 'Y Location' under 'root',click eye icon to hide others
![image](https://github.com/Nanfengzhiwo1/BlenderCombineAnimations/assets/107869748/88f12bf2-28d2-40b5-b6ff-1bf578be6ddd)

8.Click 'Running',Press **G** ,Set the value of the last frame as the Cursor Y's initial value.Move all keyframes down by the corresponding distance(The second animation should start from the end position of the first animation, not from 0)  
9.  
10.  
Wait a minutes...improving....
