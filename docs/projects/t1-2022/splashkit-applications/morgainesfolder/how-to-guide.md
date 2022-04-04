# Build a Cool Arcade Game		 

Game name: Jump		    Category: Platformer			Creator: Morgaine Barter 

 

## Project Constraints:  

Window size set to 1920 x 1080, this is a standard laptop pixel width and height 

When creating the window use function toggle_window_boarder() 
 to remove the minimize, maximize and exit options from the game window visually 

Also, center the placement of the window and give it a name using the function window_position_named() 


## Creating the player and movement: 

 

## Using Collisions: 

 

## Scene Set up: 

Create_window(1920,1080); 		//width by height 

clear_screen(Background.png); 

 

## Sprite Sheet Integration: the text file matrix refers to the cell’s index number, starting at 0, like an array 
so at the top left of the screen, the matrix says to print cell number (index) when working with a sprite sheet/page of Png's it can be helpful to create a reference with grid overlay of cell numbers to make this a faster process when drawing the scene using the matrix for the level. See below. 

This Png of game elements starts at cell 0 and goes to 76, meaning this cell sheet has 77 total cells 
if you zoom in and count the individual pixels, each cell is 16 by 16 pixels, the sheet has 11 rows, and 7 columns. The way we let the program know this information is by using the following function: bitmap_set_cell(cell_map, 16,16, 11, 7, 77); 
<image here> C:\Users\User\Documents\Code\ThothTech Handbook\handbook-1\docs\projects\t1-2022\splashkit-applications\PlatformerCellCount.png "PlatformerCellCount.png"