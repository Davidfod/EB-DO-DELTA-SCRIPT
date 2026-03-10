
local scriptURL = "https://raw.githubusercontent.com/Davidfod/CyberScript/refs/heads/main/CYBER.md"

local success, result = pcall(function()
    return loadstring(game:HttpGet(scriptURL))()
end)

if not success then
    warn("Não foi possível carregar o script: " .. tostring(result))
else
    print("Script CyberNoDry carregado com sucesso!")
end
