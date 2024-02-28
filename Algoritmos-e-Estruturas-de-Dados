class TreeNode:
    def __init__(self, key):
        self.val = key
        self.left = None
        self.right = None

def insert(root, key):
    if root is None:
        return TreeNode(key)
    else:
        if key < root.val:
            root.left = insert(root.left, key)
        else:
            root.right = insert(root.right, key)
    return root

def inorder_traversal(root):
    res = []
    if root:
        res = inorder_traversal(root.left)
        res.append(root.val)
        res = res + inorder_traversal(root.right)
    return res

# Exemplo de uso
if __name__ == "__main__":
    root = None
    keys = [8, 3, 10, 1, 6, 14, 4, 7, 13]
    
    for key in keys:
        root = insert(root, key)

    print("Árvore Binária de Busca (BST) construída:")
    print(inorder_traversal(root))
