Tree
--------------
--------------
Non linear  

Each node can have > 1 next’s.  

root is a node with no previous nodes.  

parent of a node is the node that is prev.  

Tree has 0 or 1 root.  

Subtree:
		-Tree formed by taking any node as a root  

Count of most number of edges you follow  

Depth of node is number of edges.  

leaf is node with no children  


Binary Tree  
       -2 children  
Ternary Tree  
	-3 children  


For binary trees
    node = n
leftchild = 2n+1
rightchild = 2n+2
parent = (n-1)/2
Don’t need references can mathematically find children



Use recursive methods to calculate things like height.  
##Tree Traversal


Breadth First Traversal  
	- Visit each level, one at a time.  
	- Never use it in a node based system, use when in an array.  

Depth First Traversal  
      	- Always visit you children first before visiting any neighboring node.  

Pre Order Traversal
      	- Visit node before you visit any children.  

Post Order Traversal  
      	- Visit node after you visit all the children.  

Inorder Traversal  
	- Visit the node after you visit the left but before you visit the right.  


```java

void DFS(){
    DFS(head);
}


void DFS(BTNode<E> h){
    if(h == null){

    }
    else{
        DFS(h.left);
        DFS(h.right);
    }
}
```


Binary Search Tree  
       - Not guaranteed to be bushy
       - In order traversal will visit in order, for BST
       - Removal is tricky, if removing a leaf just remove reference
       - If parent has one child move child up to parent position
       - If you have 2 children, move largest from left subtree, or smallest in
       	 right subtree
       - Red-Black tree

```java
void insert(E d){
     if (root == null)
     	root = new BTNode(d)
     else{
	node = new BTNode(d)
	insert(Node, root)
	}
}

void insert(n, h)
     int cmp = h.compareTo(h)
     	if(cmp < 0)
	       if(h.right == null)
	       		  h.right = n
		else
			insert(n, h.right)
	else if(cmp > 0)
	     if(h.left == null)
	     	       h.left = n
	     else
		insert(n, h.left)
        else
	     // deal with stuff
```


#Heap

Ordered tree from top to bottom

`
    12  
   /  \  
  10   8  
 /  \  
3    4 `

Priority queues almost always use heaps
