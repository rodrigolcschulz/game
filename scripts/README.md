# Scripts

Esta pasta contém todos os scripts GDScript (.gd) do projeto.

## Estrutura

### player/
Lógica do personagem jogável:
- `player_controller.gd` - Controle de movimento
- `player_stats.gd` - Atributos e progressão
- `sanity_system.gd` - Sistema de sanidade

### battle/
Sistema de combate:
- `battle_manager.gd` - Gerencia batalhas por turnos
- `combatant.gd` - Classe base para entidades em batalha
- `skills.gd` - Habilidades e ataques

### dialogue/
Sistema de diálogos:
- `dialogue_manager.gd` - Gerencia fluxo de diálogos
- `dialogue_data.gd` - Resource para dados de diálogo
- `choice_handler.gd` - Gerencia escolhas do jogador

### utils/
Utilitários e helpers:
- `save_system.gd` - Sistema de save/load
- `game_state.gd` - Estado global do jogo (Autoload)
- `audio_manager.gd` - Gerenciador de áudio (Autoload)
- `scene_transition.gd` - Transições entre cenas

## Convenções

- Use snake_case para nomes de arquivos
- Uma classe por arquivo
- Documente funções com comentários ##
- Use type hints sempre que possível

