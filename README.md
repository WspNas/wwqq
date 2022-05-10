local Target = nil
   for i,v in pairs(game.Players:GetChildren()) do
       if v.TeamColor == BrickColor.new("Navy blue") then
           Target = v.Name
       end
   end
   for i,v in pairs(game.Players[Target].Backpack:GetChildren()) do
       if v.Name == "Radio" then
           v:Clone().Parent = game.Players.LocalPlayer.Backpack
       end
   end
