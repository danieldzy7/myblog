---
title: BinaryTree
date: 2022-10-21
categories: Data Structure
tags:
  - Binary Tree
  - Traversal
  - Preorder
  - Inorder
  - Postorder
---

# Binary Tree

#### 1.Binary Tree Preoder, Inorder, Postorder traversal

{% asset_img assets/1.png 1 %}

一套模版走天下

```` java
class Solution {
	根左右
    public List<Integer> preorderTraversal(TreeNode root) {
        List<Integer> res = new LinkedList<>();
        Stack<TreeNode> stack = new Stack<>();
        TreeNode cur = root;

        while(cur != null || !stack.isEmpty()) {
            while (cur != null) {
                stack.push(cur);
                res.add(cur.val);
                cur = cur.left;
            }
            TreeNode temp = stack.pop();
            cur = temp.right;
        }
        return res;
    }
    ------------------------------------------------------------
    左根右    
    public List<Integer> inorderTraversal(TreeNode root) {
        List<Integer> res = new LinkedList<>();
        Stack<TreeNode> stack = new Stack<>();
        TreeNode cur = root;

        while(cur != null || !stack.isEmpty()) {
            while (cur != null) {
                stack.push(cur);
                cur = cur.left;
            }
            TreeNode temp = stack.pop();
            res.add(temp.val);
            cur = temp.right;
        }
        return res;
    }
    -------------------------------------------------------------
     左右根 = 根右左 + 反过来存res
     public List<Integer> postorderTraversal(TreeNode root) {
        List<Integer> res = new LinkedList<>();
        Stack<TreeNode> stack = new Stack<>();
        TreeNode cur = root;

        while(cur != null || !stack.isEmpty()) {
            while (cur != null) {
                res.addFirst(cur.val);
                stack.push(cur);
                cur = cur.right;
            }
            TreeNode temp = stack.pop();
            cur = temp.left;
        }
        return res;
    }
}


````

