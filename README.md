# Exercise-01b-Twine-Project

Exercise for MSCH-C220

A demonstration of this exercise is available at [https://youtu.be/VVd_8dvao9E](https://youtu.be/VVd_8dvao9E).

This exercise is an opportunity for you to create your first project in Twine, the open-source tool for creating non-linear interactive stories (interactive fiction). You should have installed [Twine 2.4.1](http://twinery.org/)  as part of your last exercise; if not, please do so now.

Fork this repository. When that process has completed, make sure that the top of the repository reads [your username]/Exercise-01b-Twine-Project. Edit the LICENSE and replace BL-MSCH-C220-F22 with your full name.  Commit your changes.

Press the green "Code" button and select "Open in GitHub Desktop". Allow the browser to open (or install) GitHub Desktop. Once GitHub Desktop has loaded, you should see a window labeled "Clone a Repository" asking you for a Local Path on your computer where the project should be copied. Choose a location where you will keep the repositories for this class (a C220 folder off your Desktop would be fine). Make sure the Local Path ends with "Exercise-01b-Twine-Project" and then press the "Clone" button. GitHub Desktop will now download a copy of the repository to the location you indicated.

Open Twine, and press the "+ Story" button in the right side bar. When you are asked what your story should be named, enter "Zork". Press the "+Add" button to get started.

You should now see a window with a blue grid background. There should be a node in the middle of the window labeled "Untitled Passage". Double click on the node to open it.

On the top line of the resulting window, change "Untitled Passage" to "West of House". Then replace the description ("Double-click this passage to edit it.") with the following:

```
This is an open field west of a white house, with a boarded front door.

[[NORTH->North of House]]
[[SOUTH->South of House]]
[[WEST->Forest]]
```

Close that window, and you should now see that the node is now labeled "West of House" and that there are three arrows pointing to newly created passages: North of House, South of House, and Forest.

Follow that same process with each of the newly created passages. When you are done, you should have eight locations:

 * Passage: North of House
   * Description: You are facing the north side of a white house.  There is no door here, and all the windows are barred.
   * Exits:
     * WEST->West of House
     * EAST->East of House
     * NORTH->Forest
 * Passage: South of House
   * Description: You are facing the south side of a white house. There is no door here, and all the windows are barred.
   * Exits:
     * WEST->West of House
     * EAST->East of House
     * SOUTH->Forest
 * Passage: Forest
   * Description: This is a forest, with trees in all directions around you.
   * Exits:
     * NORTH->Sunlit Forest
     * EAST->Forest
     * SOUTH->Forest
     * WEST->Forest
 * Passage: East of House
   * Description: You are behind the white house. A path leads into the forest to the east. In one corner of the house there is a small window which is slightly ajar.
   * Exits:
     * NORTH->North of House
     * SOUTH->South of House
     * EAST->Sunlit Forest
     * WEST->Kitchen
     * ENTER->Kitchen
 * Passage: Sunlit Forest
   * Description: This is a dimly lit forest, with large trees all around.  One particularly large tree with some low branches stands here.
   * Exits:
     * NORTH->Forest
     * SOUTH->Forest
     * EAST->Forest
     * WEST->East of House
     * UP->Tree
 * Passage: Tree
   * Description: You are about 10 feet above the ground nestled among some large branches. The nearest branch above you is above your reach. Beside you on the branch is a small bird's nest.
   * Exits:
     * DOWN->Sunlit Forest
 * Passage: Kitchen
   * Description: You are in the kitchen of the white house. A table seems to have been used recently for the preparation of food. A passage leads to the west and a dark staircase can be seen leading upward. A dark chimney leads down and to the east is a small window which is open.
   * Exits:
     * EAST->East of House

Once you have added each of these passages, close the passage edit window. Down in the bottom right corner of the workspace is a button labeled "Play". Press that now.

The game should load in your browser. You should be able to press the links to take you from one location to another.

When you are done, return to Twine. On the bottom bar press the "Zork" label. In the resulting menu, select "Publish to File".

Navigate to the location of your repository in your file system. Save the file as Zork.html in the repository (Exercise-01b-Twine-Project) folder.

Quit Twine. In GitHub desktop, you should now see Zork.html listed in the left panel. In the bottom of that panel, type a Summary message (something like "Adds a simple version of the Zork Interactive Fiction game") and press the "Commit to master" button. On the right side of the top, black panel, you should see a button labeled "Push to origin". Press that now.

If you return to and refresh your GitHub repository page, you should now see Zork.html listed among the files.

Now edit the README.md file. When you have finished editing, commit your changes, and then turn in the URL of the main repository page (https://github.com/[username]/Exercise-01b-Twine-Project) on Canvas.

The final state of the file should be as follows (replacing my information with yours):
```
# Exercise-01b-Twine-Project

Exercise for MSCH-C220

An Interactive Fiction game loosely based on the great Interactive Fiction game, Zork. Load Zork.html in a browser to play it.

## Implementation
Built using Twine 2.4.1

## References
[Zork, Infocom, 1977](https://www.pcjs.org/software/pcx86/game/infocom/zork1/)

## Future Development
None

## Created by 
Jason Francis
```
