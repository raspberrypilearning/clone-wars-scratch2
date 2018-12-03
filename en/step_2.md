## Make a spaceship

First make a spaceship that can defend the Earth!

--- task ---

Open the 'Clone wars' Scratch starter project.

**Online:** open the starter project at [rpf.io/clone-wars-on](http://rpf.io/clone-wars-on). 

**Offline:** download the starter project from [rpf.io/clone-wars-off](http://rpf.io/clone-wars-off), and then open it using the offline editor.

If you need to download and install the Scratch offline editor, you can find it at rpf.io/scratchoff.

--- /task ---

![starter project](images/starter-project.png)

--- task ---

Add this code to the spaceship sprite to make the spaceship move left if the <kbd>left</kbd> arrow is pressed:

![rocket sprite](images/rocket-sprite.png)

```blocks
	when flag clicked
	forever
		if <key [left arrow v] pressed?> then
			change x by (-4)
		end
	end
```

The x-axis goes from the left side of the Stage to the right side. This means that the spaceship moves to the left when you subtract from the value of the spaceship sprite's `x` position. So this code block is the part that makes your spaceship move left:

```blocks
change x by (-4)
```

--- /task ---

--- task ---

Add some more code inside the `forever`{:class="blockcontrol"} block to make your spaceship move to the right if the <kbd>right</kbd> arrow key is pressed.

--- hints ---

--- hint ---

Subtracting `4` from the spaceship's `x` position made it move left, so how could you make the spaceship move right by `4` instead?

--- /hint ---

--- hint ---

You need the same code block, but with a different number:

```blocks
change x by ( )
```

--- /hint ---

--- hint ---

Here is the code you need to add below the other code inside the `forever`{:class="blockcontrol"} block:

![rocket sprite](images/rocket-sprite.png)

```blocks
if <key [right arrow v] pressed?> then
	change x by (4)
end
```
--- /hint ---

--- /hints ---

--- /task ---

--- task ---

Test your project by clicking the green flag. Can you press the arrow keys to make your spaceship move left and right?

--- /task ---

