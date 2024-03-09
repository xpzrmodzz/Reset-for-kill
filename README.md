-- This script was made for you to be able to kill/"reset" your character if resetting your character is not an option, or has 
-- been taken out. This script will also work as a suicide command.

-- Function to handle player's death
local function forceResetAction()
    local player = game.Players.LocalPlayer
    if player.Character and player.Character:FindFirstChild("Humanoid") then
        player.Character.Humanoid.Health = 0
    end
end

-- Boucle pour répéter l'action de réinitialisation
while true do
    -- Appeler la fonction de réinitialisation
    forceResetAction()
    -- Attendre quelques secondes avant de répéter l'action (par exemple, 5 secondes)
    wait(3.7)
end
