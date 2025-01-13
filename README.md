local Player = game.Players.LocalPlayer


local animation = Instance.new("Animation")
animation.AnimationId = "rbxassetid://110137167847351"
wait()


for i,v in pairs(game.Workspace:GetDescendants()) do
	if v.Name == Player.Character.Name then
		
	local Human = v:FindFirstChild("Humanoid")
	local LoadAnim = Human:LoadAnimation(animation)
		
    LoadAnim.Priority = Enum.AnimationPriority.Action
    LoadAnim:Play()

	end
end
