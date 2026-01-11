local plr=game.Players.LocalPlayer
local uis=game:GetService("UserInputService")
uis.InputBegan:Connect(function(input,gp)
 if input.UserInputType==Enum.UserInputType.Keyboard and input.KeyCode==Enum.KeyCode.Space then
  if plr.Character and plr.Character:FindFirstChild("Humanoid") then
   plr.Character.Humanoid:ChangeState(Enum.HumanoidStateType.Jumping)
  end
 end
end)
