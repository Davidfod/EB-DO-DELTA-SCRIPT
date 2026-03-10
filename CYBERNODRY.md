
local scriptURL = "https://raw.githubusercontent.com/Davidfod/CyberScript/refs/heads/main/CYBER.md"

local success, result = pcall(function()
    return loadstring(game:HttpGet(scriptURL))()
end)

if not success then
    warn("Erro ao carregar o script: " .. tostring(result))
end
