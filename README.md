本地OrionLib=loadstring(游戏：HttpGet(('https://pastebin.com/raw/qqT4Ek4t')))()

本地窗口=OrionLib:MakeWindow({Name="NASA中心"，HidePremium=false，saveconfig=true，introtext="NASA中心"，ConfigFolder="NASA中心"})
游戏：GetService("StarterGuui")：SetCore("SendNotification"，{title="NASA中心"；Text="NASA中心"；持续时间=4；})

本地关于=窗口：MakeTab({
name="坤制作"，
icon="rbxassetid://11312"，
PremiumOnly=false
})

关于：addParagraph("云端更新")
关于：addParagraph("更新什么我也不知道")


本地选项卡=窗口：MakeTab({
name="公告"，
icon="rbxassetid://11312"，
PremiumOnly=false
})

选项卡：AddButton({
name="复制作者QQ"，
callback=函数()
setclipboard("你妈死了😋")
结束
})

选项卡：AddButton({
name="复制QQ群"，
callback=函数()
固定夹板(“521471687”)
结束
})

OrionLib:MakeNotification({
name="坤脚本"，
content="欢迎使用"，
image="rbxassetid://394647608"，
时间=2

})

本地选项卡=窗口：MakeTab({

    name="玩家"，

    icon="rbxassetid://394647608"，

    PremiumOnly=false

})

本地节=制表符：AddSection({

	name="欢迎玩家"

})

选项卡：AddSlider({

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

		
