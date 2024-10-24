# konsole
A custom developer console for Roblox, and Roblox Studio, for all your needs.

-----------------------------------------------------------------------------

# How to import:

1. Download the .rbxm file from the git release page on our repo
2. Then drag drop it into your Roblox Studio place
3. Drag the GUI to StarterGui
4. And then done!

# _G API

This developer console consists of using the _G variable to make it so that all scripts can access parts of the Konsole such as logging something to the Konsole, clearing the output or input Konsole, and so much more.

# How to access the _G API:

Go into your script type in _G.konsole, and then your done ;) now you can access all that it brings.

Functions:

_G.konsole.log(any, Enum.MessageType?)

_G.konsole.clear(string) // example: _G.konsole.clear('Input'), _G.konsole.clear('Output')

_G.konsole.execute(string) // runs a loadstring function

Signals:

_G.konsole.onlog:Connect(function()
  -- code here
end)

_G.konsole.onlog:Once(function()
  -- code here
end)

_G.konsole.oncleared:Connect(function()
  -- code here
end)

_G.konsole.oncleared:Once(function()
  -- code here
end)

_G.konsole.onexecute:Connect(function()
  -- code here
end)

_G.konsole.onexecute:Once(function()
  -- code here
end)
