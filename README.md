local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
local Window = Library.CreateLib("Ninja Legends Hub - made by @c.o.u.r.t.l.a.n.d", "BloodTheme")
local Tab = Window:NewTab("Main 😎")

local Section = Tab:NewSection("Elements 🌊🔥")

Section:NewButton("Transfer All Elements 🌊🔥", "Gives all the Elements", function()
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Frost")
    wait(2)
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Inferno")
    wait(2)
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Lightning")
    wait(2)
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Electral Chaos")
    wait(2)
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Masterful Wrath")
    wait(2)
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Shadow Charge")
    wait(2)
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Shadowfire")
    wait(2)
    game.ReplicatedStorage.rEvents.elementMasteryEvent:FireServer("Eternity Storm")
end)

local Section = Tab:NewSection("Farm")

Section:NewToggle("Auto Swing ⚔", "force swing", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "swingKatana"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1)
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "swingKatana"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1)
        wait()
        end
    end
end)

Section:NewToggle("Sell 30x 💰", "Sells at the Last Island which has 30x coins multiplier", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(84.2945251, 87069.0391, 123.435143)
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(84.2945251, 87069.0391, 123.435143)
        wait()
        end
    end
end)

local Section = Tab:NewSection("King of the Hill 👑")

Section:NewToggle("King of the hill Farm", "This farm is for chi", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(218.628006, 89.7980728, -306.10614)
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(250.906387, 89.7980728, -267.906158)
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(217.515915, 89.7980728, -271.927338)
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(245.596283, 89.7980728, -291.48761)
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(218.628006, 89.7980728, -306.10614)
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(250.906387, 89.7980728, -267.906158)
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(217.515915, 89.7980728, -271.927338)
        wait(1)
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(245.596283, 89.7980728, -291.48761)
        wait()
        end
    end
end)

local Section = Tab:NewSection("Boss Farms 🤵")

Section:NewToggle("Robot 🤖", "Use with Auto Swing", function(state)
    if state then
        _G.boss = true
        while _G.boss do
        wait()
        if game:GetService("Workspace").bossFolder:FindFirstChild("RobotBoss"):FindFirstChild("HumanoidRootPart") then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.bossFolder.RobotBoss.HumanoidRootPart.CFrame
        end
        wait()
        end
    else
        _G.boss = false
        while _G.boss do
        wait()
        if game:GetService("Workspace").bossFolder:FindFirstChild("RobotBoss"):FindFirstChild("HumanoidRootPart") then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.bossFolder.RobotBoss.HumanoidRootPart.CFrame
        end
        wait()
        end
    end
end)

Section:NewToggle("Magma 🔥", "Also Use with Auto Swing", function(state)
    if state then
        _G.boss = true
        while _G.boss do
        wait()
        if game:GetService("Workspace").bossFolder:FindFirstChild("AncientMagmaBoss"):FindFirstChild("HumanoidRootPart") then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.bossFolder.AncientMagmaBoss.HumanoidRootPart.CFrame
        end
        wait()
        end
    else
        _G.boss = false
        while _G.boss do
        wait()
        if game:GetService("Workspace").bossFolder:FindFirstChild("AncientMagmaBoss"):FindFirstChild("HumanoidRootPart") then
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Workspace.bossFolder.AncientMagmaBoss.HumanoidRootPart.CFrame
        end
        wait()
        end
    end
end)

local Section = Tab:NewSection("Ring autofarm")

Section:NewToggle("Ring Farm ⭕", "Brings all The Hoops in the sky to You", function(state)
    if state then
            _G.cum = true -- set to false and it will stop
            while wait() do
            if _G.cum then
            local plr = game.Players.LocalPlayer
            for i,v in pairs(workspace.Hoops:GetDescendants()) do
            if v.ClassName == "MeshPart" then
            v.touchPart.CFrame = plr.Character.HumanoidRootPart.CFrame
            end
        end
    end
    end
    else
            _G.cum = false -- set to false and it will stop
            while wait() do
            if _G.cum then
            local plr = game.Players.LocalPlayer
            for i,v in pairs(workspace.Hoops:GetDescendants()) do
            if v.ClassName == "MeshPart" then
            v.touchPart.CFrame = plr.Character.HumanoidRootPart.CFrame
            end
        end
    end
end
end
end)

local Tab = Window:NewTab("Auto Purchase 🛒")
local Section = Tab:NewSection("I RECOMMEND USING THEM ALL AT ONCE")

Section:NewToggle("Swords ⚔", "Buys Swords For You", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllSwords"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllSwords"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    end
end)

Section:NewToggle("Belts 👞", "Buys Belts For You", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllBelts"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllBelts"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    end
end)

Section:NewToggle("Ranks 💎🏆", "Buys Ranks For You", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        local oh1 = "buyRank"
        local oh2 = game:GetService("ReplicatedStorage").Ranks.Ground:GetChildren()
        for i = 1,#oh2 do
        game:GetService("Players").LocalPlayer.ninjaEvent:FireServer(oh1, oh2[i].Name)
        end
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        local oh1 = "buyRank"
        local oh2 = game:GetService("ReplicatedStorage").Ranks.Ground:GetChildren()
        for i = 1,#oh2 do
        game:GetService("Players").LocalPlayer.ninjaEvent:FireServer(oh1, oh2[i].Name)
        end
        wait()
        end
    end
end)

Section:NewToggle("Skills 😎", "Buys Skills For You", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllSkills"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllSkills"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    end
end)

Section:NewToggle("Shuriken ⚔", "Buys Shurikens For You", function(state)
    if state then
        _G.Condition = true -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllShurikens"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    else
        _G.Condition = false -- true turns it on, false turns it off
        while _G.Condition == true do
        local A_1 = "buyAllShurikens"
        local A_2 = "Inner Peace Island"
        local Event = game:GetService("Players").LocalPlayer.ninjaEvent
        Event:FireServer(A_1, A_2)
        wait()
        end
    end
end)

local Tab = Window:NewTab("Chest AutoFarm 🧰")

local Section = Tab:NewSection("MORE SCRIPTS COMING SOON BABY")

local Section = Tab:NewSection("Chest Farm")

Section:NewButton("All Chests", "Teleports you to all of the chests", function()
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(44.8091736, 772.892029, -186.113876)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(44.8091736, 772.892029, -186.113876)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(210.977661, 4054.0918, 58.45504)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(210.977661, 4054.0918, 58.45504)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(35.7061806, 5681.10449, 60.3083115)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(35.7061806, 5681.10449, 60.3083115)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(37.7248688, 9309.10352, 60.0999756)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(37.7248688, 9309.10352, 60.0999756)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(38.2728996, 13704.792, 58.9767265)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(38.2728996, 13704.792, 58.9767265)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(36.5750389, 17711.0234, 59.0358429)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(36.5750389, 17711.0234, 59.0358429)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(35.99506, 24094.6055, 59.6758461)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(35.99506, 24094.6055, 59.6758461)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(33.2964478, 28279.1758, 51.1746063)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(33.2964478, 28279.1758, 51.1746063)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-48.8769913, 33382.1094, -180.307999)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-48.8769913, 33382.1094, -180.307999)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-132.883453, 39457.9688, 169.222794)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-132.883453, 39457.9688, 169.222794)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(428.534729, 46137.9648, -45.9690437)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(428.534729, 46137.9648, -45.9690437)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(424.302216, 52741.6719, -50.0839348)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(424.302216, 52741.6719, -50.0839348)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(424.19577, 66800.8047, -46.1431847)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(424.19577, 66800.8047, -46.1431847)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(425.921204, 70414.9063, -44.0284424)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(425.921204, 70414.9063, -44.0284424)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(425.431824, 74579.7031, -45.7830544)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(425.431824, 74579.7031, -45.7830544)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(426.997314, 79884.4297, -48.2278976)
    wait(1)
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(426.997314, 79884.4297, -48.2278976)
end)

local Tab = Window:NewTab("Misc 🥇")
local Section = Tab:NewSection("Miscellaneous")

Section:NewSlider("WS - Walk Speed 🏃️", "Walk Speed", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)

Section:NewSlider("JP - Jump Power 🏢", "Jump Power", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = s
end)

Section:NewButton("Ctrl To Teleport 🕶", "teleport", function()
    local Plr = game:GetService("Players").LocalPlayer
    local Mouse = Plr:GetMouse()
    Mouse.Button1Down:connect(function()
    if not game:GetService("UserInputService"):IsKeyDown(Enum.KeyCode.LeftControl) then return end
    if not Mouse.Target then return end
    Plr.Character:MoveTo(Mouse.Hit.p)
    end)
end)

Section:NewButton("Infinite Jump", "jump with no restriction", function()
    game.Players.LocalPlayer.multiJumpCount.Value = 9999999
end)

local Tab = Window:NewTab("Credits 🏆")
local Section = Tab:NewSection("Credits = cland")
local Section = Tab:NewSection("Kavo UI LIB - Made by xHeptc")
