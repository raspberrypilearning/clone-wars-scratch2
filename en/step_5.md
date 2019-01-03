## Space-hippos

Now you're going to add lots of flying hippos that try to destroy your spaceship.

--- task ---

Create a new sprite with the 'Hippo1' image in the Scratch library. Use the **shrink** tool to make the `Hippo` sprite a similar size to the `Spaceship` sprite.

![screenshot](images/invaders-hippo.png)

--- /task ---

--- task ---

Set the `Hippo` sprite's rotation style to **left-right**.

[[[generic-scratch-sprite-rotation-style]]]

--- /task ---

--- task ---

Add some code to hide the `Hippo` sprite when the game starts.

![hippo sprite](images/hippo-sprite.png)

![blocks_1546523027_3088238](images/blocks_1546523027_3088238.png)
--- /task ---

--- task ---

Add some code to the Stage to create a new `Hippo` clone every few seconds.

--- hints ---

--- hint ---

When the `green flag is clicked`{:class="blockevents"}, `repeatedly`{:class="blockcontrol"} `wait`{:class="blockcontrol"} `between 2 and 4 seconds`{:class="blockoperators"} and then `create a clone of the Hippo sprite`{:class="blockcontrol"}.

--- /hint ---

--- hint ---

Here are the blocks you need:

![blocks_1546523028_9276502](images/blocks_1546523028_9276502.png)

--- /hint ---

--- hint ---

This is what your code should look like:

![stage sprite](images/stage-sprite.png)

![blocks_1546523030_5624168](images/blocks_1546523030_5624168.png)

--- /hint ---

--- /hints ---

--- /task ---

Each new hippo clone should appear at a random `x` position, and every clone should have a random speed.

--- task ---

Create a new variable called `speed`{:class="blockdata"} that is for the `Hippo` sprite only.

[[[generic-scratch-add-variable]]]

When you've done this correctly, the variable has the name of the sprite next to it, like this:

![screenshot](images/invaders-var-test.png)

--- /task ---

--- task ---

When each `Hippo` clone starts, pick a random speed and starting place for it. Then show the clone on the screen.

![blocks_1546523032_157261](images/blocks_1546523032_157261.png)

--- /task ---

--- task ---

Test your code. Does a new hippo appear every few seconds?

--- /task ---

At the moment the hippos don't move.

--- task ---

Each hippo should move around randomly until it gets hit by a lightning bolt. To make that happen, attach this code below the blocks that are already in the `Hippo` sprite's code script:

![blocks_1546523033_7609413](images/blocks_1546523033_7609413.png)

--- /task ---

--- task ---

Test your code again. You should see a new hippo clone appear every few seconds, and each clone should move at a different speed.

![screenshot](images/hippo-clones.gif)

--- /task ---

--- task ---

Now test the spaceship's laser cannon. If a lightning bolt hits a hippo, does the hippo vanish?

--- /task ---

