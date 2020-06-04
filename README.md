# DEMtoMinecraft
Scripts to Convert a DEM to a Minecraft world


##Requirements
Requires Python 3 (tested on Python 3.8.3)

Python Packages
	anvil (pip install anvil-parser)
	numpy (pip install numpy)
	pandas (pip install pandas)
	matplotlib (pip install matplotlib)
	sys (pip install sys)
	PySide2 (pip install PySide2)

##Settings
Horizontal Scale (default: 1): reduction factor in x and z directions. For example, with a horizontal scale of 4, for every 4 cells in the input DEM, the output Minecraft world will have 1 block.
Vertical Scale (default: 1): as for horizontal scale, but in the vertical direction.
Water Level (default: 1): DEM value below which to add water instead of solid blocks.
Skirt Height (default: 5): height above the bottom of the Minecraft World to make the zero point of the DEM

Main Block: the block used fpr all blocks, with the exception of the top block, in a stack.
Top Block: the block used as the top block in a stack, except where that stack is a half integer tall.
Use Half Blocks: determines whether the nearest half integer or nearest integer is used as the stack height.
Half Block Type: the block to be used as the half block, when "Use half blocks" is checked.