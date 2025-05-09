local painel = Instance.new("Frame")
painel.Size = UDim2.new(0, 300, 0, 200)
painel.Position = UDim2.new(0.5, -150, 0.5, -100)
painel.BackgroundColor3 = Color3.fromRGB(128, 0, 128) -- Roxo
painel.BorderSizePixel = 0
painel.Name = "PainelRoxo"
painel.Parent = script.Parent

-- Título
local titulo = Instance.new("TextLabel")
titulo.Size = UDim2.new(1, 0, 0, 40)
titulo.Position = UDim2.new(0, 0, 0, 0)
titulo.BackgroundTransparency = 1
titulo.Text = "Painel Roxo"
titulo.TextColor3 = Color3.new(1, 1, 1)
titulo.TextScaled = true
titulo.Font = Enum.Font.SourceSansBold
titulo.Parent = painel

-- Botão de fechar
local fechar = Instance.new("TextButton")
fechar.Size = UDim2.new(0, 30, 0, 30)
fechar.Position = UDim2.new(1, -35, 0, 5)
fechar.BackgroundColor3 = Color3.fromRGB(200, 0, 0)
fechar.Text = "X"
fechar.TextColor3 = Color3.new(1, 1, 1)
fechar.Font = Enum.Font.SourceSansBold
fechar.TextScaled = true
fechar.Parent = painel

-- Evento de fechar
fechar.MouseButton1Click:Connect(function()
	painel:Destroy()
