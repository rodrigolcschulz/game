# 📁 Estrutura do Projeto

## Organização de Pastas

```
game/
├── scenes/              # Cenas do Godot (.tscn)
│   ├── player/         # Cenas relacionadas ao jogador
│   ├── enemies/        # Cenas de inimigos
│   ├── maps/           # Mapas e áreas do jogo
│   └── ui/             # Interface do usuário
│
├── scripts/            # Scripts GDScript (.gd)
│   ├── player/         # Lógica do personagem
│   ├── battle/         # Sistema de combate
│   ├── dialogue/       # Sistema de diálogos
│   └── utils/          # Utilitários e helpers
│
├── assets/             # Recursos visuais e sonoros
│   ├── sprites/        # Sprites dos personagens e objetos
│   ├── tilesets/       # Tilesets para mapas
│   ├── music/          # Músicas de fundo
│   └── sfx/            # Efeitos sonoros
│
└── docs/               # Documentação do projeto
    ├── escopo.md       # Escopo e planejamento
    └── ESTRUTURA.md    # Este arquivo
```

## Convenções de Nomenclatura

### Arquivos de Cena (.tscn)
- Use PascalCase: `PlayerCharacter.tscn`, `VillageMap.tscn`
- Seja descritivo: `DialogueBox.tscn` em vez de `Box.tscn`

### Scripts (.gd)
- Use snake_case: `player_controller.gd`, `battle_system.gd`
- Nomeie de acordo com a funcionalidade

### Assets
- Use snake_case: `player_idle.png`, `forest_tileset.png`
- Inclua descrição do estado: `enemy_slime_attack.png`

## Boas Práticas

1. **Um script por classe**: Cada classe deve ter seu próprio arquivo
2. **Organização por funcionalidade**: Agrupe arquivos relacionados
3. **Comentários**: Documente funções complexas
4. **Sinais (Signals)**: Use para comunicação entre nós
5. **Autoload**: Use para gerenciadores globais (SaveSystem, GameState, etc.)

## Próximos Passos

1. Implementar Player Character com movimento básico
2. Criar primeiro mapa de teste
3. Implementar sistema de colisão
4. Adicionar sistema de diálogo

