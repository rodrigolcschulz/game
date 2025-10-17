# 🌑 Void Whispers - Quick Reference

## 📖 Documentos Importantes

| Leia Isto | Para Fazer Isso |
|-----------|-----------------|
| **START_HERE.md** | Começar o projeto pela primeira vez |
| **docs/TAREFAS_INICIAIS.md** | Ver tarefas práticas para começar |
| **docs/DESENVOLVIMENTO.md** | Aprender convenções e boas práticas |
| **docs/ROADMAP.md** | Ver planejamento completo |
| **docs/escopo.md** | Entender objetivo e visão do jogo |
| **CONTRIBUTING.md** | Contribuir para o projeto |

## 🎮 Comandos Rápidos Godot

| Atalho | Ação |
|--------|------|
| `F5` | Rodar projeto |
| `F6` | Rodar cena atual |
| `F7` | Step (debug) |
| `Ctrl+S` | Salvar |
| `Ctrl+D` | Duplicar nó |
| `Ctrl+Shift+D` | Descolar nó |

## 📁 Onde Colocar Cada Coisa

### Cenas (.tscn)
- **Personagens** → `scenes/player/`
- **Inimigos** → `scenes/enemies/`
- **Mapas** → `scenes/maps/`
- **UI** → `scenes/ui/`

### Scripts (.gd)
- **Controle do Player** → `scripts/player/`
- **Sistema de Batalha** → `scripts/battle/`
- **Diálogos** → `scripts/dialogue/`
- **Utilitários** → `scripts/utils/`

### Assets
- **Sprites** → `assets/sprites/`
- **Tilesets** → `assets/tilesets/`
- **Música** → `assets/music/`
- **SFX** → `assets/sfx/`

## 🎯 Checklist Rápido

### Setup Inicial
- [x] Estrutura de pastas
- [x] Configuração do Godot
- [x] Documentação
- [ ] Abrir no Godot
- [ ] Testar cena principal

### Primeiro Dia
- [ ] Criar sprite do personagem (placeholder)
- [ ] Implementar movimento WASD
- [ ] Criar mapa de teste
- [ ] Adicionar colisão

### Primeira Semana
- [ ] Sistema de animação
- [ ] Camera seguindo player
- [ ] Primeiro NPC
- [ ] Diálogo básico

## 💡 Dicas Rápidas

1. **Use placeholders**: Quadrados coloridos são suficientes no início
2. **Teste frequente**: F5 após cada mudança pequena
3. **Commits regulares**: Save your progress!
4. **Leia a doc**: Tudo está documentado aqui
5. **Divirta-se**: É um projeto de paixão! 🎮

## 🆘 Problemas Comuns

### "Cena não carrega"
→ Use `res://` no caminho, ex: `res://scenes/player/Player.tscn`

### "Colisão não funciona"
→ Verifique se CollisionShape2D tem uma shape definida

### "Erro de syntax"
→ GDScript é sensível à indentação (use tabs)

### "Não sei por onde começar"
→ Leia `docs/TAREFAS_INICIAIS.md` passo a passo

## 📚 Links Úteis

- **Godot Docs**: https://docs.godotengine.org/
- **GDScript Basics**: https://gdquest.github.io/learn-gdscript/
- **Heartbeast RPG**: https://youtube.com/playlist?list=PL9FzW-m48fn2SlrW0KoLT4n5egNdX-W9a
- **Assets Grátis**: https://opengameart.org/

## 🎨 Paleta de Cores do Jogo

```
Background Dark:  #1a1a2e
Primary Dark:     #16213e
Secondary Dark:   #0f3460
Purple (Mystic):  #533483
Red (Alert):      #e94560
```

## 🎵 Tom do Jogo

- **Gênero**: RPG 2D, Lovecraftiano
- **Atmosfera**: Misteriosa, sombria, intrigante
- **Inspiração**: Chrono Trigger + Cthulhu
- **Diferencial**: Sistema de sanidade

---

**Use este arquivo como referência rápida durante o desenvolvimento!**

*Save this file in your bookmarks!* 🔖

