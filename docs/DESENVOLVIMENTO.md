# 🛠️ Guia de Desenvolvimento

## Começando a Desenvolver

### Pré-requisitos
- Godot 4.3 ou superior
- Editor de código (VS Code recomendado com extensão Godot)
- Git para controle de versão

### Configuração Inicial
1. Abra o projeto no Godot
2. Familiarize-se com a estrutura de pastas
3. Leia o `docs/escopo.md` para entender o objetivo
4. Consulte o `docs/ROADMAP.md` para ver o que precisa ser feito

## Workflow de Desenvolvimento

### 1. Antes de Começar uma Feature
- [ ] Verifique o roadmap e escolha uma task
- [ ] Crie uma branch: `git checkout -b feature/nome-da-feature`
- [ ] Leia a documentação relacionada

### 2. Durante o Desenvolvimento
- [ ] Escreva código limpo e comentado
- [ ] Teste frequentemente no editor
- [ ] Faça commits pequenos e descritivos
- [ ] Use a convenção de nomenclatura do projeto

### 3. Após Completar
- [ ] Teste a feature completamente
- [ ] Verifique se não quebrou nada existente
- [ ] Atualize a documentação se necessário
- [ ] Faça merge na branch main

## Convenções de Código

### GDScript Style Guide

```gdscript
# Bom exemplo de classe
extends CharacterBody2D
class_name Player

## Constantes em UPPER_SNAKE_CASE
const MAX_SPEED = 200.0
const ACCELERATION = 800.0

## Variáveis exportadas (aparecem no Inspector)
@export var health: int = 100
@export var sanity: int = 100

## Variáveis privadas começam com _
var _velocity: Vector2 = Vector2.ZERO

## Sinais no topo, após variáveis
signal health_changed(new_health: int)
signal died()

## Função _ready sempre primeiro
func _ready() -> void:
    print("Player ready!")

## Funções públicas
func take_damage(amount: int) -> void:
    health -= amount
    health_changed.emit(health)
    
    if health <= 0:
        die()

## Funções privadas começam com _
func _update_animation() -> void:
    # Lógica de animação
    pass

func die() -> void:
    died.emit()
    queue_free()
```

### Organização de Nodes
```
Player (CharacterBody2D)
├── Sprite2D
├── CollisionShape2D
├── AnimationPlayer
├── Camera2D
└── Components/
    ├── HealthComponent
    ├── SanityComponent
    └── InventoryComponent
```

## Sistemas Principais

### 1. Sistema de Movimento
- Usar `CharacterBody2D` para o player
- Input com `Input.get_vector()`
- Suavização com lerp/acceleration

### 2. Sistema de Diálogo
- Usar Resource para dados de diálogo
- Singleton para gerenciar estado
- Sinais para eventos de diálogo

### 3. Sistema de Combate
- Estado de batalha separado
- Turnos gerenciados por queue
- Animações e feedback visual

### 4. Sistema de Sanidade (Único!)
- Decresce em eventos específicos
- Efeitos visuais progressivos
- Altera gameplay em sanidade baixa

## Debugging

### Comandos Úteis
```gdscript
# Print simples
print("Debug: ", variable)

# Print com informações
print_debug("Erro em: ", get_stack())

# Breakpoint
breakpoint # Pausa execução aqui
```

### Atalhos do Godot
- `F5`: Rodar projeto
- `F6`: Rodar cena atual
- `F7`: Step (debug)
- `Ctrl+S`: Salvar
- `Ctrl+D`: Duplicar nós

## Recursos Úteis

### Documentação
- [Godot Docs](https://docs.godotengine.org/)
- [GDScript Reference](https://docs.godotengine.org/en/stable/tutorials/scripting/gdscript/index.html)
- [Godot Tutorials](https://www.gdquest.com/)

### Assets
- [OpenGameArt](https://opengameart.org/)
- [itch.io Assets](https://itch.io/game-assets)
- [Kenney Assets](https://kenney.nl/assets)

### Música
- [FreePD](https://freepd.com/)
- [Incompetech](https://incompetech.com/)

## Troubleshooting

### Problema: Colisão não funciona
- Verifique se o CollisionShape2D tem uma shape definida
- Confirme que as layers de colisão estão corretas
- Use debug shapes (Debug > Visible Collision Shapes)

### Problema: Cena não carrega
- Verifique o caminho do arquivo
- Use `res://` sempre para caminhos
- Confirme que o arquivo .tscn existe

### Problema: Performance ruim
- Use `call_deferred()` para operações pesadas
- Reduza chamadas em `_process()` e `_physics_process()`
- Use Object Pooling para objetos frequentes

## Dicas Pro

1. **Use Autoloads para sistemas globais**: SaveSystem, AudioManager, GameState
2. **Sinais > Chamadas diretas**: Melhor para desacoplamento
3. **Teste no editor**: Use `@tool` para testar scripts no editor
4. **Version control**: Commit frequente, messages descritivas
5. **Backup**: Sempre faça backup antes de mudanças grandes

---

**Dúvidas?** Consulte a documentação ou abra uma issue no repositório!

