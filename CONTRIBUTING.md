# Como Contribuir para Void Whispers

Obrigado por considerar contribuir para o projeto! 🎮

## 🤝 Como Posso Ajudar?

Existem várias formas de contribuir:

- **Código**: Implementar features, corrigir bugs
- **Arte**: Criar sprites, tilesets, animações
- **Áudio**: Compor músicas, criar efeitos sonoros
- **Design**: Criar puzzles, balancear combate, design de níveis
- **Escrita**: Escrever diálogos, lore, história
- **Testes**: Jogar e reportar bugs
- **Documentação**: Melhorar docs, tutoriais

## 🚀 Começando

1. **Fork** o repositório
2. **Clone** seu fork localmente
3. **Crie uma branch** para sua feature: `git checkout -b feature/minha-feature`
4. **Faça suas alterações**
5. **Commit** suas mudanças: `git commit -m "Add: nova feature"`
6. **Push** para o GitHub: `git push origin feature/minha-feature`
7. Abra um **Pull Request**

## 📝 Convenções de Commit

Use prefixos claros nos commits:

- `Add:` - Nova feature ou arquivo
- `Fix:` - Correção de bug
- `Update:` - Atualização de código existente
- `Remove:` - Remoção de código/arquivo
- `Refactor:` - Refatoração de código
- `Docs:` - Mudanças em documentação
- `Style:` - Formatação, estilo de código
- `Test:` - Adição ou correção de testes

Exemplos:
```
Add: player movement system
Fix: collision bug in village map
Update: dialogue system to support choices
Docs: add tutorial for creating NPCs
```

## 🎨 Estilo de Código

### GDScript
- Use **snake_case** para variáveis e funções
- Use **PascalCase** para classes
- Use **UPPER_SNAKE_CASE** para constantes
- Sempre use **type hints**
- Comente código complexo
- Siga o [GDScript Style Guide oficial](https://docs.godotengine.org/en/stable/tutorials/scripting/gdscript/gdscript_styleguide.html)

### Exemplo:
```gdscript
extends CharacterBody2D
class_name Player

const MAX_SPEED: float = 200.0

@export var health: int = 100

var _is_moving: bool = false

func take_damage(amount: int) -> void:
    health -= amount
    if health <= 0:
        die()

func _ready() -> void:
    print("Player initialized")
```

## 🐛 Reportando Bugs

Ao reportar um bug, inclua:

1. **Descrição clara** do problema
2. **Passos para reproduzir**
3. **Comportamento esperado** vs **comportamento atual**
4. **Screenshots/vídeos** se aplicável
5. **Versão do Godot** que está usando
6. **Sistema operacional**

## 💡 Sugerindo Features

Ao sugerir uma feature:

1. **Verifique o ROADMAP** para ver se já está planejada
2. **Descreva claramente** o que você quer
3. **Explique por que** seria útil
4. **Sugira como** poderia ser implementado

## ✅ Checklist para Pull Requests

Antes de enviar seu PR, confirme:

- [ ] O código segue as convenções do projeto
- [ ] Testei as mudanças no Godot
- [ ] Não quebrei funcionalidades existentes
- [ ] Adicionei comentários em código complexo
- [ ] Atualizei a documentação se necessário
- [ ] O commit message é claro e descritivo

## 🎯 Áreas que Precisam de Ajuda

Confira as issues marcadas com:
- `good first issue` - Bom para iniciantes
- `help wanted` - Precisamos de ajuda aqui
- `art needed` - Precisamos de arte
- `music needed` - Precisamos de música

## 📚 Recursos para Aprender

- [Godot Docs](https://docs.godotengine.org/)
- [GDQuest Tutorials](https://www.gdquest.com/)
- [Heartbeast RPG Tutorial](https://www.youtube.com/playlist?list=PL9FzW-m48fn2SlrW0KoLT4n5egNdX-W9a)

## 💬 Comunicação

- **Issues**: Para bugs e sugestões
- **Pull Requests**: Para contribuições de código
- **Discussions**: Para discussões gerais

## 📜 Código de Conduta

- Seja respeitoso e inclusivo
- Aceite críticas construtivas
- Foque no que é melhor para o projeto
- Ajude outros contribuidores

## 🙏 Obrigado!

Toda contribuição, por menor que seja, é muito apreciada! Juntos vamos criar um jogo incrível! 🌑✨

