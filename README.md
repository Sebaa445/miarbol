# miarbol
package avl

import ()

type tree struct {
	root *node
}

type node struct {
	left  *node
	right *node
	value int
}


func New() *tree {
	func equilibrar( tree*a, node, rama int, nuevo int){
		for fe int, fe> root, fe++{
			if nuevo{
		if rama == left{
		node.fe--
		}else{
			node.fe++
		}
		else{
			if rama == right{
				node.fe--

			}else{
				node.fe++
			}
		}
	}
	if node.fe == -2{
		if node.left.fe==1, rdd a, node{

		}else{
			rsd a,node
			salir = true
		}
		}
		if node.fe == 2{
			if node.left.fe== -1{
				rdi a, node

			}else{
				rsi a,node
				salir = true
			}
			}
			if node.root{
				if node.root.right == nodo{
					rama = right
				}else{
					rama= left
					node = node.root
				}
			}

}
}
func rsd (tree *t, pNode node){
	pNode root= nodo.root
	pNode P =nodep
	pNode Q= P.left
	pNode B =Q.right
	if root{
		if root.right == P {
			root.right =Q

			}else{
				root.left=Q
			}
			}else{
				*t =Q
				P.left = B
				Q.rigth= P
				P.root =Q
			}
				if b{
					B.root=P
					Q.root = root
					P.Fe=0
					P.Fe=0

				}
			}
			func rdd (tree *root, tree node){
				pNode root= nodo.root
				pNode P =node
				pNode Q= P.left
				pNode R= Q.right
				pNode B =R.left
				pNode C= R.right
				if root{
					if root.right == R {
						root.right =R

						}else{
							root.left=R
						}
						}else{
							*t =R
							Q.right =B
							P.left = C
							R.rigth= Q
							R.right =Q
							R.root= root
							P.root=Q.root=R
						}
							if b{
								B.root=Q
								if c{
									c.root= P
								}

							}
						}
}

	return new(tree)
}


func (t *tree) Insert(x int) {
	if t.root == nil {
		t.root = &node{value: x}
	} else {
		t.root = t.root.insert(x)
	}
}

func (n *node) insert(x int) *node {
	if n == nil {
		return &node{value: x}
	}
	if x <= n.value {
		n.left = n.left.insert(x)
		return n
	}
	n.right = n.right.insert(x)
	return n
}


func (t *tree) Search(x int) bool {
	return t.root.search(x)
}

func (n *node) search(x int) bool {
	if n == nil {
		return false
	}
	if n.value == x {
		return true
	}
	if n.value < x {
		return n.right.search(x)
	}

	return n.left.search(x)
  }
