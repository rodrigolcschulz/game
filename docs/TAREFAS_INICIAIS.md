# 📋 Tarefas Iniciais - Primeiros Passos

Este documento lista as primeiras tarefas práticas para começar o desenvolvimento.

## ✅ Setup Concluído
- [x] Estrutura de pastas criada
- [x] Arquivo `project.godot` configurado
- [x] Documentação inicial
- [x] `.gitignore` configurado
- [x] Ícone placeholder criado
- [x] Cena principal básica

## 🎯 Próximas Tarefas (em ordem de prioridade)

### 1. Abrir o Projeto no Godot
```
1. Abra o Godot Engine
2. Clique em "Import"
3. Navegue até a pasta do projeto
4. Selecione o arquivo project.godot
5. Clique em "Import & Edit"
```

### 2. Testar a Cena Principal
- [ ] Pressione F5 para rodar o projeto
- [ ] Você deve ver "Void Whispers" na tela
- [ ] Confirme que não há erros no console

### 3. Criar o Personagem Básico

#### 3.1. Criar Sprite Placeholder
```
1. No Godot, crie um novo recurso de imagem 32x32
2. Pinte um quadrado colorido simples
3. Salve em: assets/sprites/player_placeholder.png
```

#### 3.2. Criar Cena do Player
```
1. Crie nova cena (Scene > New Scene)
2. Root node: CharacterBody2D
3. Renomeie para "Player"
4. Adicione nós filhos:
   - Sprite2D (textura: player_placeholder.png)
   - CollisionShape2D (shape: RectangleShape2D)
5. Salve em: scenes/player/Player.tscn
```

#### 3.3. Script de Movimento
- [ ] Crie script `player_controller.gd`
- [ ] Implemente movimento básico WASD
- [ ] Adicione suavização de movimento
- [ ] Salve em: scripts/player/player_controller.gd

### 4. Criar Primeiro Mapa de Teste

#### 4.1. Criar Tileset Placeholder
```
1. Crie imagem 32x32 com alguns tiles simples:
   - Verde = grama
   - Cinza = pedra
   - Marrom = terra
2. Salve em: assets/tilesets/test_tileset.png
3. No Godot, crie TileSet a partir da imagem
```

#### 4.2. Criar Mapa
```
1. Nova cena com Node2D como root
2. Adicione TileMap
3. Configure o tileset
4. Desenhe um mapa pequeno (20x20 tiles)
5. Adicione instância do Player
6. Salve em: scenes/maps/TestMap.tscn
```

### 5. Configurar Camera
- [ ] Adicione Camera2D ao Player
- [ ] Configure para seguir o personagem
- [ ] Ajuste limites se necessário

### 6. Teste Completo
- [ ] Player se move em 4 direções
- [ ] Colide com borders do mapa
- [ ] Camera segue suavemente
- [ ] Sem erros no console

## 🎓 Tutoriais Recomendados

### Para Iniciantes em Godot:
1. [Godot Docs - Your First 2D Game](https://docs.godotengine.org/en/stable/getting_started/first_2d_game/index.html)
2. [GDQuest - Learn GDScript](https://gdquest.github.io/learn-gdscript/)
3. [Heartbeast - Action RPG Tutorial](https://www.youtube.com/playlist?list=PL9FzW-m48fn2SlrW0KoLT4n5egNdX-W9a)

### Para Sistema de RPG:
1. Sistema de stats e progressão
2. Inventário e itens
3. Combate por turnos
4. Sistema de save/load

## 💡 Dicas Importantes

1. **Comece Simples**: Use placeholders coloridos, não se preocupe com arte agora
2. **Teste Frequente**: Rode o jogo a cada pequena mudança
3. **Commits Regulares**: Faça commit a cada feature funcional
4. **Não Pule Etapas**: Movimento básico deve funcionar antes de adicionar combate
5. **Use a Documentação**: Godot Docs é excelente, consulte sempre

## 🆘 Precisa de Ajuda?

- **Godot Community**: https://godotengine.org/community
- **Discord Godot**: https://discord.gg/godotengine
- **Reddit r/godot**: https://reddit.com/r/godot
- **Stack Overflow**: Tag [godot]

---

**Depois de completar estas tarefas**, você terá um personagem funcional que pode andar em um mapa básico. A partir daí, seguir o ROADMAP.md para adicionar mais features!

Boa sorte! 🚀

