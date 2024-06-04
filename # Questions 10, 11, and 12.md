# 4.3 planar graphs

## Questions 10, 11, and 12

### **10.** Euler's formula $(v - e + f = 2)$ holds for all connected planar graphs. 
### What if a graph is not connected? Suppose a planar graph has two components. 
### What is the value of $v - e + f$ now? What if it has $k$ components?

- In a case that a graph is not connect e.g. A triangle and A line segment. 
That would have 5 vertices, 4 edges, and 2 faces which leads us to 5 - 4 + 2 = 2 which is false. 
if the two where connected we can see that the count of vertices decreases telling us the action of separation causes an added vertice without the balanced increase in edges. 

$$v - e + f = k + 1$$

This is because adding a face adds a vertice without adding an edge increaseing the total.
If you have one face it would just be 1 + 1 as k would be 1. 

***

### **11.** Prove that the Petersen graph (below) is not planar. 
### Hint: What is the length of the shortest cycle? (This quantity is usually called the girth of the graph.)

![Image of graph](Anar's CSC208/Screenshot 2024-06-04 at 3.15.57 AM.png)

- The shortest cycle is 5

- any planar graph must acomplish $e \le 3v - 6\text{.}$    
 $$15 \le 3(10)-6\text{.}$$
 
 $$15 \le 14$$
***

### **12.** Prove that any planar graph with $v$ vertices and $e$ edges satisfies  $e \le 3v - 6\text{.}$ 

Proof. We know in any planar graph the number of faces $f$ satisfies $3f \le 2e$ since each face is bounded by at least three edges, but each edge borders two faces. Combine this with Euler's formula:



$v - e + f = 2$

$3f \le 2e$

$\dfrac{2e}{3} \geq f$

$v - e + \dfrac{2e}{3} \geq 2$

$3v - e \geq 6$

$e \le 3v - 6\text{.}$ 
