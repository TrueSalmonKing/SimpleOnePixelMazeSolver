# Simple Maze Solver

a java program capable of reading maze images and solving them, granted that the maze's borders are made out of a one pixel block  using djikstra's algorithm, we solve the maze through 3 basic steps listed in the process of execution section

## Getting started

To run this program optimally, it is necessary to note that the image to be used must adhere to appropriate format of which is an image representing a maze made out of 1 pixel black blocks, a sample image is provided along with the software.
Run the software, and choose the maze and the result will be printed in the same directory as the source maze

# Process of execution
### Step 1

The pixels are read and nodes are defined as to ease the computational overhead in the case of a large maze, we do so following 2 rules: if a pixel is surronded 2 pixels on oppsing sides ( left and right or up and down ), then said pixel is not a node. Otherwise it's a node. This two rules seperate a path ( the first case ) from a node.

### Step two

Each node is added to linked list that will later be treated using djikstra's algorith to define the shortest path from source to end, such is done using the defined list of nodes along with a sublist of sources and exits, which chooses the optimal path between them.

### Step three

The node list is treated and we return a list of nodes with the exit node as a head of the list, and with a previous pointer, pointing to the previous node in the shortest path leading to the source node. Finally the path from the source to the exit.

### Prerequisites

JDK 12.0

## Built With

* [Eclipse](https://www.eclipse.org/documentation/) - The java IDE used.

## Note

program not optimzed for large scale mazes.
