
# A* Pathfinding_Unity_Implementation
This project is an Implementation of A* pathfinding algorithm inside the Unity game engine

### What is A* Search Algorithm?
A* Search algorithm is one of the best and popular technique used in path-finding and graph traversals.

![image](https://github.com/AdityaNayak04/A-star_imp/assets/168894294/f79ccb81-58ae-4f4c-bdc9-a1ab584866b5)


Consider a square grid having many obstacles and we are given a starting cell and a target cell. We want to reach the target cell (if possible) from the starting cell as quickly as possible.
What A* Search Algorithm does is that at each step it picks the node according to a **F-cost**.
#### **F-cost = G-cost + H-cost**
  G-cost = Distance from starting node <br>
  H-cost = Distance from end node (heuristic)
  
![ezgif-3-8a6cceeb6d](https://github.com/AdityaNayak04/A-star_imp/assets/168894294/c659707f-18bf-40d3-b1aa-f0b7d51a8404)

### Pseudocode for A* Pathfinding - 
![image](https://github.com/AdityaNayak04/A-star_imp/assets/168894294/1dff8b8f-a749-4b0d-8b7f-9869156cc65b)

# Implementation in Unity
We have implemented A* pathfinding algorithm in the Unity game engine by filling the map with nodes and making a 2-D array out of them. 


https://github.com/AdityaNayak04/A-star_imp/assets/168894294/b9309214-136e-45d3-82b3-49bfed31b362



**These nodes can be visualised using the gizmos in the unity scene. Here, the white box gizmos show the walkable nodes whereas the red ones show the non-walkable nodes. This classification is done by checking a collision
in each node, if it collides with anything belonging to the unwalkable layermask then that node is classified as unwalkable.**
Now, in this array of nodes, the code A* search will be implemented.
<br>
### This is how the final implementation looks like



https://github.com/AdityaNayak04/A-star_imp/assets/168894294/2ce847fb-f8be-4fc8-868e-ccba13b2e6e1




There is one target object used as the target position for the seeker objects to move to. The black gizmo lines show the final path obtained from the A* search i.e., the shortest path.
There are multiple seeker units as you can see which ask for the best path from the A* object based on the current and the target world position.



#### **To see this project in action a version of Unity has to be installed. This project is made using Unity 2023.2.5f1.**
Unity can be installed from the **[Unity Hub](https://unity.com/unity-hub)** installer.<br>
An executable build is also present in the repository. But, please note that the gizmos won't be visible in the build as they are in the Unity editor.
