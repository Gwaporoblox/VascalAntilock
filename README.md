--KEY IS C
--sub to vascal for more leaked scripts

getgenv().tog = false
getgenv().key = "E"
getgenv().X = 678
getgenv().Y = 100
getgenv().Z = -344

 game.StarterGui:SetCore("SendNotification", {
                                        Title = "Vascal on yt",
                                        Text = "Sub To Vascal!" })

game:GetService("RunService").Heartbeat:Connect(function()
        if getgenv().tog then
                local vel = game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity
                game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity = Vector3.new(getgenv().X, getgenv().Y, getgenv().Z)
                game:GetService("RunService").RenderStepped:Wait()
                game.Players.LocalPlayer.Character.HumanoidRootPart.Velocity = vel
        end
end)

game:GetService("Players").LocalPlayer:GetMouse().KeyDown:Connect(function(keyPressed)
        if keyPressed == string.lower(getgenv().key) then
                pcall(function()
                        if getgenv().tog == false then
                                getgenv().tog = true
                                game.StarterGui:SetCore("SendNotification", {
                                        Title = "Sheesh2458",
                                        Text = "AA Enabled" })
                        elseif getgenv().tog == true then
                                getgenv().tog = false
                                game.StarterGui:SetCore("SendNotification", {
                                        Title = "sheesh2458",
                                        Text = "AA Disabled" })
                        end
                end)
        end
end)
hookfunction(game.Players.LocalPlayer.IsInGroup, function() return true end)
 game.StarterGui:SetCore("SendNotification", {
                                        Title = "Vascal On yt",
                                        Text = "Sub To Vascal!" })
loadstring(game:HttpGet("https://raw.githubusercontent.com/Nosssa/NossLock/main/VinGUI"))()
