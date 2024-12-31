--carregar biblioteca
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

local Window = Fluent:CreateWindow({
Title = "Krscripts " .. Fluent.Version,
TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

local Tabs = {
Main = Window:AddTab({ Title = "Scripts/-/all" }),
myscripts = Window:AddTab({ Title = "misc", Icon = "misc" }),
bloxfruits = Window:AddTab({ Title = "Blox fruits", Icon = "Blox fruits" }),
adustytrip = Window:AddTab({ Title = "A Dusty Trip", Icon = "A Dusty Trip" }) ,
Settings = Window:AddTab({ Title = "Settings", Icon = "settings" }) 
}
-- parágrafos
Tabs.Main:AddParagraph({ Title = "Scripts", Content = "credits:Krscripts.\nSecond line!" })

-- botões
Tabs.Main:AddButton({ Title = "Genesis/-/universal", Callback = function() 
loadstring(game:HttpGet('https://raw.githubusercontent.com/raw-scriptpastebin/raw/main/B_Genesis'))()
end })

Tabs.Main:AddButton({ Title = "prison life/-/admin", Callback = function() 
loadstring(game:HttpGet("https://rawscripts.net/raw/Prison-Life-Prizz-Admin-14511"))()
end })

Tabs.Main:AddButton({ Title = "Arceus x/-/script", Callback = function() 
loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/chillz-workshop/main/Arceus%20X%20V3"))()
end })

Tabs.Main:AddButton({ Title = "", Callback = function()

end }) 

Tabs.Main:AddButton({ Title = "", Callback = function()

end }) 

Tabs.Main:AddButton({ Title = "", Callback = function()

end }) 

-- blox fruits botões:
Tabs.Settings:AddButton({ Title = "texto", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "Tsuo Hub❌", Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Tsuo7/TsuoHub/main/Tsuoscripts"))()

end})

Tabs.bloxfruits:AddButton({ Title = "Speed hub❌", Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/ahmadsgamer2/Speed-Hub-X/main/SpeedHubX"))()

end})

Tabs.bloxfruits:AddButton({ Title = "Thunder Z hub✅", Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/ThunderZ-05/HUB/main/Mobile-Loader"))()

end})

Tabs.bloxfruits:AddButton({ Title = "Fai Fao❌/-/desatualizado", Callback = function()
loadstring(game:HttpGet"https://raw.githubusercontent.com/PNguyen0199/Script/main/Fai-Fao-Ver2.lua")()

end})

Tabs.bloxfruits:AddButton({ Title = "OMG hub✅", Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/Omgshit/Scripts/main/MainLoader.lua"))()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

Tabs.bloxfruits:AddButton({ Title = "tex", Callback = function()

end})

-- misc botões:

Tabs.myscripts:AddButton({ Title = "infinite jump", Callback = function()
loadstring(game:HttpGet("https://raw.githubusercontent.com/HeyGyt/infjump/main/main"))()
end})

local Slider = Tabs.myscripts:AddSlider("pulo", 
{
    Title = "ajusta pulo",
    Description = "irar mudar pulo jogador",
    Default = 2,
    Min = 0,
    Max = 5,
    Rounding = 1,
    Callback = function(Value)
        print("pulo mudou pra:", Value)
    end
})

local Slider = Tabs.myscripts:AddSlider("velocidade", 
{
    Title = "Velocidade",
    Description = "Ajusta a velocidade do jogador",
    Default = 2,
    Min = 0,
    Max = 5,
    Rounding = 1,
    Callback = function(Value)
        local player = game.Players.LocalPlayer
        local character = player.Character or player.CharacterAdded:Wait()
        local humanoid = character:WaitForChild("Humanoid")
        
        -- Define a velocidade de caminhada
        humanoid.WalkSpeed = Value * 10  -- Multiplica o valor para aumentar o impacto
    end
})

Tabs.myscripts:AddButton({ Title = "", Callback = function()

end})

Tabs.myscripts:AddButton({ Title = "", Callback = function()

end})

Tabs.myscripts:AddButton({ Title = "", Callback = function()

end})

Tabs.myscripts:AddButton({ Title = "", Callback = function()

end})

Tabs.myscripts:AddButton({ Title = "", Callback = function()

end})

Tabs.myscripts:AddButton({ Title = "", Callback = function()

end})

Window:SelectTab(1)
Fluent:Notify({ Title = "Krscript", Content = "The script has been loaded." })
