local OrionLib = loadstring(game:HttpGet(('https://pastebin.com/raw/qqT4Ek4t')))()

local Window = OrionLib:MakeWindow({Name = "NASA中心", HidePremium = false, SaveConfig = true,IntroText = "NASA中心", ConfigFolder = "NASA中心"})
game:GetService("StarterGui"):SetCore("SendNotification",{ Title = "NASA中心"; Text ="NASA中心"; Duration = 4; })

local about = Window:MakeTab({
    Name = "坤制作",
    Icon = "rbxassetid://11312",
    PremiumOnly = false
})

about:AddParagraph("云端更新")
about:AddParagraph("更新什么我也不知道")


local Tab =Window:MakeTab({
	Name = "公告",
	Icon = "rbxassetid://11312",
	PremiumOnly = false
})

Tab:AddButton({
	Name = "复制作者QQ",
	Callback = function()
     setclipboard("你妈死了😋")
  	end
})

Tab:AddButton({
	Name = "复制QQ群",
	Callback = function()
     setclipboard("521471687")
  	end
})

OrionLib:MakeNotification({
	Name = "坤脚本",
	Content = "欢迎使用",
	Image = "rbxassetid://394647608",
	Time = 2

})

local Tab = Window:MakeTab({

    Name = "玩家",

    Icon = "rbxassetid://394647608",

    PremiumOnly = false

})

local Section = Tab:AddSection({

	Name = "欢迎玩家"

})

Tab:AddSlider({

	Name = "速度",

	Min = 16,

	Max = 200,

	Default = 16,

	Color = Color3.fromRGB(255,255,255),

	Increment = 1,

	ValueName = "数值",

	Callback = function(Value)

		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value

	end    

})

Tab:AddSlider({

	Name = "跳跃高度",

	Min = 50,

	Max = 200,

	Default = 50,

	Color = Color3.fromRGB(255,255,255),

	Increment = 1,

	ValueName = "数值",

	Callback = function(Value)

		game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value

	end    

})

Tab:AddTextbox({

	Name = "跳跃高度设置",

	Default = "",

	TextDisappear = true,

	Callback = function(Value)

		game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value

	end

})

Tab:AddTextbox({

	Name = "移动速度设置",

	Default = "",

	TextDisappear = true,

	Callback = function(Value)

		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value

	end

})

Tab:AddTextbox({

	Name = "重力设置",

	Default = "",

	TextDisappear = true,

	Callback = function(Value)

		game.Workspace.Gravity = Value

	end

})

Tab:AddToggle({

	Name = "夜视",

	Default = false,

	Callback = function(Value)

		if Value then

		    game.Lighting.Ambient = Color3.new(1, 1, 1)

		else

		    game.Lighting.Ambient = Color3.new(0, 0, 0)

		end

	end

})

Tab:AddButton({

	Name = "跟踪玩家",

	Callback = function()

     loadstring(game:HttpGet("https://pastebin.com/raw/KCrLyTz2"))()

  	end    

})

Tab:AddButton({

  Name = "自瞄",

  Callback = function ()

loadstring(game:HttpGet("https://pastebin.com/raw/1Gp9c57U"))()

  end

})

Tab:AddButton({

	Name = "林飞行",

	Callback = function()

     loadstring(game:HttpGet("https://pastebin.com/raw/gEd1QwJE"))()

  	end    

})

Tab:AddLabel("火速用范围")

Tab:AddButton({

  Name = "普通范围",

  Callback = function ()

loadstring(game:HttpGet("https://pastebin.com/raw/jiNwDbCN"))()

  end

})

Tab:AddButton({

  Name = "中等范围😱",

  Callback = function ()

loadstring(game:HttpGet("https://pastebin.com/raw/x13bwrFb"))()

  end

})

Tab:AddButton({

    Name="全图范围😰",

    Callback=function()

loadstring(game:HttpGet("https://pastebin.com/raw/KKY9EpZU"))()

    end

})

Tab:AddButton({

    Name="终极范围😨",

    Callback=function()

loadstring(game:HttpGet("https://pastebin.com/raw/CAQ9x4A7"))()

    end

})

Tab:AddButton({

  Name = "无限跳",

  Callback = function ()

loadstring(game:HttpGet("https://pastebin.com/raw/V5PQy3y0", true))()

  end

})

Tab:AddButton({

	Name = "替身",

	Callback = function()

loadstring(game:HttpGet(('https://raw.githubusercontent.com/SkrillexMe/SkrillexLoader/main/SkrillexLoadMain')))()

    end

})

Tab:AddButton({

	Name = "爬墙",

	Callback = function()

loadstring(game:HttpGet("https://pastebin.com/raw/zXk4Rq2r"))()

end

})

Tab:AddButton({

	Name = "最好看光影",

	Callback = function()

loadstring(game:HttpGet("https://pastebin.com/raw/Bkf0BJb3"))()

end

})

Tab:AddButton({

	Name = "点击传送工具",

	Callback = function()

mouse = game.Players.LocalPlayer:GetMouse() tool = Instance.new("Tool") tool.RequiresHandle = false tool.Name = "[FE] TELEPORT TOOL" tool.Activated:connect(function() local pos = mouse.Hit+Vector3.new(0,2.5,0) pos = CFrame.new(pos.X,pos.Y,pos.Z) game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = pos end) tool.Parent = game.Players.LocalPlayer.Backpack

	end

})

Tab:AddButton({

  Name = "肘人",

  Callback = function ()

loadstring(game:HttpGet(('https://raw.githubusercontent.com/0Ben1/fe/main/obf_5wpM7bBcOPspmX7lQ3m75SrYNWqxZ858ai3tJdEAId6jSI05IOUB224FQ0VSAswH.lua.txt'),true))()

  end

})

Tab:AddButton({

	Name = "甩飞别人",

	Callback = function()

     loadstring(game:HttpGet("https://pastebin.com/raw/GnvPVBEi"))()

  	end    

})

Tab:AddButton({

	Name = "防止掉线（反挂机）",

	Callback = function()

	print("Anti Afk On")

		local vu = game:GetService("VirtualUser")

		game:GetService("Players").LocalPlayer.Idled:connect(function()

		   vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)

		
