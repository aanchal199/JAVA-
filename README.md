# JAVA- TREE
Java Program to built a tree 

import javax.swing.*;
import javax.swing.tree.DefaultMutableTreeNode;
public class Tree1
{
JFrame F;
Tree1()
{
F = new JFrame("TREE");
DefaultMutableTreeNode Style = new DefaultMutableTreeNode("Style");
DefaultMutableTreeNode Color = new DefaultMutableTreeNode("Color");
DefaultMutableTreeNode Font = new DefaultMutableTreeNode("Font");
Style.add(Color);
Style.add(Font);

DefaultMutableTreeNode Blue = new DefaultMutableTreeNode("Blue");
DefaultMutableTreeNode Green = new DefaultMutableTreeNode("Green");
DefaultMutableTreeNode Black = new DefaultMutableTreeNode("Black");
Color.add(Blue);
Color.add(Green);
Color.add(Black);
JTree jt=new JTree(Style);
F.add(jt);
F.setSize(300,300);
F.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
F.setVisible(true);
}
public static void main(String args[])
{ 
new Tree1();
}
}
