game.Players.PlayerAdded:Connect(function(player)
    player.CharacterAdded:Connect(function(character)
        local humanoid = character:FindFirstChild("Humanoid")
        if humanoid then
            humanoid.WalkSpeed = 30 -- Define a velocidade do jogador (padrão é 16)
            print("Velocidade aumentada para o jogador: " .. player.Name)
        end
    end)
end)
