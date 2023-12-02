


 class TreeNode:
     def __init__(self, val=0, left=None, right=None):
         self.val = val
         self.left = left
         self.right = right
class Solution:
    def invertTree(self, root: TreeNode or None):
       if root is None:
           return
       root.left,root.right=root.right,root.left #swaping the lefft and right nodes
       self.invertTree(root.left)
       self.invertTree(root.right)
       return root
  # Definition for a binary tree node.
  Inverting or inverting a binary tree means swapping the left and right subtrees of every node in the tree. Mathematically, if T is a binary tree, the inverted tree T' is obtained by swapping the left and right children of every node in T.[BST]
