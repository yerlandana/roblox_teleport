local StartPoint = script.Parent.Part1
local EndPoint = script.Parent.Part2
function TouchedFunc(touched)
	if touched.Parent:FindFirstChild("Humanoid") then
		local human = touched.Parent.HumanoidRootPart
		human.Position = EndPoint.Position +Vector3.new(0,10,0)
	end
end
StartPoint.Touched:Connect(TouchedFunc
