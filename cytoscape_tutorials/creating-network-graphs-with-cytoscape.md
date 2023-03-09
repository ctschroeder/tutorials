# Creating Network Graphs with Cytoscape

## 1. About this tutorial

This tutorial is a modified version of Dr. Miram Posner's Cytoscape tutorial ["Creating Network Graphs with Cytoscape"](http://dx.doi.org/10.5281/zenodo.56245). Licensed [CC-BY 4.0](https://github.com/ctschroeder/cytoscape_tutorials/blob/master/license.md). 

Modified for use in Caroline T. Schroeder's Introduction to Digital Humanities course at the University of Oklahoma.

### About Cytoscape

Cytoscape is a tool for viewing and analyzing **networks** (meaning, in this case, any group of entities that are connected in some way). Cytoscape is not too hard to use, but it won't make much sense unless you have a sense of some basic network analysis vocabulary and concepts. Dr. Posner made a glossary for you [here](https://github.com/miriamposner/network_analysis_workshop/blob/master/SNAglossary.md). In addition, Scott Weingart has a great [introduction to network analysis](http://journalofdigitalhumanities.org/1-1/demystifying-networks-by-scott-weingart/).

## 2. Setting up your data

The most important thing to understand about Cytoscape (or, really, most network analysis tools) is the format in which you need to structure your data. At its most basic, Cytoscape wants a spreadsheet containing two columns. The objects in the first column should be connected in some way to the objects in the second column. This is called an **edge list**. In the example below, my edge list contains two kinds of things: **films** and **actors**. The columns could be reordered so that the Films column precedes the Actors column; it doesn't matter. All that matters here is that each row in my spreadsheet describes a connection between two entities.

Other kinds of relationships you could describe in an edge list:

* **Actor A** appears in a film with **Actor B**.
* **Person A** possesses a preference for **Thing A**.
* **Person A** shares a preference with **Person B**.
* **Film A** shares an actor with **Film B**.
* **Person A** wrote **Book A**.

... and on and on. The important thing here is that your edge list should contain a list of relationships between, at most, two kinds of entities (e.g., actors and films, people and preferences, people and books). The *nature* of those relationships can differ. For example, Person A could have *written* Book A, while Person B *published* Book A. But there should be two different kinds of things, at most, described in two columns.

You can save your spreadsheet as an Excel document (with the file extension .xls) or its generic equivalent, a CSV (with the file extension .csv). Cytoscape can interpret both of these formats.

**Note from Dr. S:** You also can have an edge list with edge attributes. Such a list would have two columns for the entities (as described above) and then additional columns for the type of relationship or edge. So you could have a two columns of people who are familial relations. Person A is related to Person B. Column C might have the type of relationship (parent, child, sibing, etc.). Be sure your edge attributes are _edge_ attributes not _person_ attributes. So Column C would be describing Person A as the parent of Person B, not saying that Person A has an identity as a parent. (Person A is of course a parent, but Column C is describing the _relationship_ -- the edge -- between A & B, not a characteristic of A. A could also be a sibling or an aunt/uncle as part of their identity, but what matters to you is their relationship to B (parent).

![][1]

[1]: images/creating-network-graphs-with-cytoscape/setting-up-your-data.png

## 3. Get your edge list into Cytoscape

Open up Cytoscape. You should be greeted with a welcome pane that looks something like the one below. (If not, read on for instructions on how to accomplish the same thing without the welcome screen.)

Drag the edge list you've prepared into the pane labeled **Drag network files here**.

![][2]

[2]: images/creating-network-graphs-with-cytoscape/get-your-edge-list-into-cytoscape.png

### Pre-prepared data you can use for this tutorial

Dr. Posner has an [edge-list of African American actors in silent films](https://github.com/miriamposner/cytoscape_tutorials/blob/master/data/edgelist.csv). (Use the "raw" download link.)

Dr. S will be using data from the [Programming Historian tutorial on network analysis of historical sources](https://programminghistorian.org/en/lessons/creating-network-diagrams-from-historical-sources). If you use this data please:
  - Read the [section describing the data and case study](https://programminghistorian.org/en/lessons/creating-network-diagrams-from-historical-sources#about-the-case-study)
  - Read the [section about the coding scheme](https://programminghistorian.org/en/lessons/creating-network-diagrams-from-historical-sources#about-the-case-study) for relationships, race, gender, and time

### If you don't see that welcome screen...

no big deal. Someone might have disabled it, but you can accomplish the same thing by clicking on the **Import Network from File** button (circled below) and selecting your edge list.

![][3]

[3]: images/creating-network-graphs-with-cytoscape/if-you-don-t-see-that-welcome-screen.png

## 4. Help Cytoscape understand your data

The screen that pops up after you imported your edge list might be the most initially confusing part of Cytoscape, although it's no problem once you figure out what it wants. You need to tell Cytoscape which parts of your data constitute the entities in your network diagram.

Cytoscape hasn't understood right away that you want a network composed of **film** and **actor** nodes. You can tell that's the case because the icon that appears next to the words **actors** and **films** looks sort of like a document, which means that Cytoscape thinks that you've fed it a list of **edge attributes**, not edges themselves. Edge attributes can come in handy, as I'll explain below, but that's not what you've provided Cytoscape at the moment.

We need to tell Cytoscape that the edge list we've provided contains **Sources** in one column and **Targets** in another. 
1.  **If you're using Dr. Posner's data:** It doesn't matter, in this case, which column you designate a **source** and which column you designate a **target**; it's just that one column has to be one and the other has to be the other. (If our network was [directed](http://www.shizukalab.com/toolkits/sna/plotting-directed-networks), this would matter, but that's more information than you need right now.) 
    - OK, let's tell Cytoscape how to interpret our data. Click on the arrow next to the word **actors** and from the menu that appears, select the green circle. Cryptically, this icon means **Source**. 
    - For the **films** column, do the same thing, but this time select the red bullseye, which means **Target**.
    - When you've changed both columns, click **OK**.

2.  **If you're using the Programming Historian data about help in the Holocaust**: 
    - Click on the arrow next to **Giver**, and then select the green button which means **source**. 
    - For the **Recipient** column select the bullseye, which means **target**.
    - When you've changed both columns, click **OK**.

![][4]

[4]: images/creating-network-graphs-with-cytoscape/help-cytoscape-understand-your-data.png

## 5. You have a (very confusing) network!

If the previous steps worked properly, you should have a network of connected nodes. If you have more than 100 or so, though, your network will look a lot like a hairball. We'll talk about ways to make your network graph more legible in subsequent steps.

For now, note that you can zoom in on parts of your network using the magnifying glasses or your mouse. On a Mac, you can move your canvas around if you hold down the **command** key and drag. You can also search for individual nodes by using the search box at the upper right of the window. (Note that Cytoscape doesn't zoom to the node you searched for right away; it just highlights it in yellow. You may have to zoom out to see the selected node.)

![][5]

[5]: images/creating-network-graphs-with-cytoscape/you-have-a--very-confusing--network-.png

## 6. Switch up your style

One of the easiest ways to change the look of your network diagram is to switch the style using one of Cytoscape's built-in options. To do that, click the **Style** tab on the control panel and then choose one of the options with which you're presented. I don't know if I *love* any of them, but some are more legible than others.

![][6]

[6]: images/creating-network-graphs-with-cytoscape/switch-up-your-style.png

## 7. Change your layout

Sometimes networks are more legible if you change the arrangement of the nodes. You can do this by switching the layout. Click on **Layout** from Cytoscape's menu bar and select one of the layout options. Experiment with various layouts and notice how drastically your network diagram changes.

Confoundingly, each of these wildly different network layouts displays the same basic information. How can this be? Simple: In most network graphs, the proximity of two nodes doesn't indicate anything except legibility. This can be really confusing, because cognitively, we expect proximity to convey meaningful information. It just doesn't, though, in most network diagrams. The presence or absence of an edge means something, and color and size often do, too. But proximity generally doesn't.

![][7]

[7]: images/creating-network-graphs-with-cytoscape/change-your-layout.png

## 8 Analyze centrality and betweenness with the Holocaust Data

Once you have picked a style, you can analyze the relationships between your nodes.

On the top menu, click Tools > Analyze
 - you will need to decide whether you want a DIRECTED or UNDIRECTED network
 - only choose DIRECTED if you know for sure your network is directed
 - choosing undirected will tell you the connections between nodes regardless of direction

On the lower pane you should see a list of names and data.
  - click on the label of any column to sort the data according to that label
  - for example, clicking on "Betweenness Centrality" will list the names according to who is most or less "between". Then you can see who has the most "betweenness"!
  - clicking on Degree or Number of Edges will tell you how connected a node is to its neighbor nodes -- how many relationships that node has

When you describe _what you learn from your network graph_ you should use those statistics to inform your analysis.

## 8. Customize your style

### Overview

You can make changes to many visual attributes of your network graph from Cytoscape's control panel. Once you've selected the **Style** tab, look at the bottom of the control panel. You'll see that three additional buttons allow you to customize the look of the **nodes**, the **edges**, and the **network** as a whole.

Looking at the **Node** style pane, you'll see that we can alter many aspects of our nodes, including their border, the color, height, labels, etc. But what do the three columns, labeled **Def.**, **Map.,** and **Byp.** mean?

- **Def.** stands for **default**: the default visual attribute of a node. If you click on the default fill color for your network diagram, for example (in the image below, it's a blue square), you'll see that you can swap out the colors of your network's nodes.

- **Byp.** stands for **bypass**, and it allows you to apply a style to a group of nodes that you select.

- The **Map.** (mapping) column allows you to control the visual features of your nodes *according to their properties*. 
  - For example, if you're using Dr. Posner's data, let's say you'd like all of the films from a particular studio to appear in pink. You can do that by mapping that attribute to a particular color. Or, let's say you'd like those nodes with more connections to appear larger. You can do that with the mapping control.
  - If you're using the Programming Historian data, you can color the nodes by race or by gender of the person. 

The problem is, we don't have any information about the nodes currently included in our network. So in the next tutorial, we'll look at how to load up **attributes** for our nodes.


![][8]

[8]: images/creating-network-graphs-with-cytoscape/customize-your-style.png

### You can customize your EDGE colors

#### One simple, non-computational method is search
Search for a specific node (like Rita Neumann in the Holocaust data) in the upper right search box. Her node should be highlighted, and depending on the style you chose, the edges connected to her should light up.

#### Customize your edge color style
Be sure you are in the **style** pane on the left. (Not Network.) 

On the bottom of the style pane, you should see options for node, edge, and network. Click on **edge**.

Click on **stroke color**.
- You should see options for **column** and **mapping type**. Click to the right of **column** to select the edge attribute you want to use for coloring. I am using the holocaust data, so I will select "Form of Help." 
- (Note: the data is in code. To see what the numerical codes stand for, so you can understand the data, see [this webpage](https://programminghistorian.org/en/lessons/creating-network-diagrams-from-historical-sources). Scroll down for the tables.)
- For **mapping type** select **discrete**. (Discrete means that each type of help will get a different color).
- A table should appear with all the different entries of forms of help (or entries for whichever edge addribute you chose)
- Click on the empty cell to the right of the first number. On the right of the cell, you'll see three dots and a trash can. **Click on the three dots**
- Select a color
- Do this for every entry in the table

Voila, you have a network graph with different colors for your edges based on an edge attribute!

## 9. Export your graph to publish

Dr. Posner has an entire [tutorial about publishing your graph](https://github.com/ctschroeder/tutorials/blob/master/cytoscape_tutorials/publishing-your-network-diagram.md#1-option-1-export-a-static-image). 

I recommend following the instructions for [exporting a static image](https://github.com/ctschroeder/tutorials/blob/master/cytoscape_tutorials/publishing-your-network-diagram.md#1-option-1-export-a-static-image). The second option (a live, interactive graph) will not work well with our course blog.


