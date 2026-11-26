# Geometry Survival: O Cálculo Final

Jogo sério 2D em Godot 4.3 (GDScript) para praticar o cálculo de áreas de figuras planas no Ensino Médio.
Axi-01, a Arquiteta Dimensional, sela as **fendas** abertas pela Entropia calculando a área das Formas Caóticas que saem delas.

Versão **v1.4** — Vertical Slice (EAP 1.4): apresentação visual, interface e áudio completos. Veja `docs/CHANGELOG.md`.

## Como executar

1. Instale o [Godot 4.3](https://godotengine.org/download) (versão padrão, não a .NET).
2. No Godot, clique em **Importar**, selecione `project.godot` e pressione **F5**.

Renderer **Compatibility**: exporta para Web (HTML5) e roda em máquinas modestas.

## Controles

| Ação | Teclado / mouse |
|---|---|
| Navegar nos menus | ↑ ↓ ← → ou mouse |
| Selecionar / confirmar resposta / próxima onda | Enter ou clique |
| Pausar (durante o encontro) / voltar | Esc |
| Resposta decimal | vírgula ou ponto (ex.: 12,5) |

## Fluxo do jogo

Tela inicial → Menu principal → Arquipélago (seleção de setor) → cartão do setor → 3 ondas (a fenda abre, a forma surge, o jogador calcula, a fenda é selada ou se expande) → fim de setor com estrelas → próximo setor liberado → Vitória ou Derrota.
O progresso é salvo automaticamente ao voltar ao mapa ("Continuar" no menu).

## Testes automatizados

```bash
godot --headless --import .              # apenas na primeira vez
godot --headless -s tests/test_runner.gd # código de saída 0 = tudo OK
```

Cobrem validação de entrada, tolerância, geração de formas, risco, pontuação e vidas, desbloqueio, vitória, derrota, reinício, sequência de acertos, abandono de setor, salvamento/restauração, áudio procedural e um teste de fumaça da interface inteira (menu → mapa → encontro → pausa → fim de setor).

## Checklist manual (1.5.1)

1. Tela inicial: o logotipo se monta e "Pressione qualquer tecla" abre o menu.
2. Menu: hover/teclado destacam as opções; "Continuar" só fica ativo com partida salva.
3. Configurações: sliders alteram o volume na hora; "Movimento reduzido" congela o parallax.
4. Encontro: a fenda abre, a forma é traçada, o risco sobe no medidor; Enter confirma e depois avança.
5. Acerto: feixe da Axi, fenda selada, pontos voando e contagem no HUD.
6. Erro com risco > 70%: fenda vermelha se expande, tela treme, um coração se parte, resolução aparece.
7. Esc pausa; "Voltar ao mapa" desfaz só o setor atual.
8. Fim de setor mostra estrelas; o mapa anima o desbloqueio do próximo setor.
9. Vitória e Derrota exibem desempenho por setor e o recorde.

## Onde ajustar

- Balanceamento: `scripts/GameRules.gd`.
- Cores de setores e interface: `scripts/ui/Palette.gd`.
- Sons e trilhas: `scripts/AudioManager.gd`.

## Estrutura

| Pasta / arquivo | Responsabilidade |
|---|---|
| `scripts/GameRules.gd`, `AnswerValidator.gd`, `ShapeGenerator.gd` | Regras, validação e geração de desafios |
| `scripts/GameManager.gd` | Estado global, progressão, FSM do Geo, sequência, abandono/restauração (autoload) |
| `scripts/Settings.gd`, `SaveGame.gd`, `AudioManager.gd` | Configurações, salvamento e áudio procedural (autoloads) |
| `scripts/Main.gd` | Orquestra telas, transições, pausa, música e tremor de tela |
| `scripts/ShapeEncounter.gd`, `ShapeDisplay.gd` | Encontro com a fenda e desenho animado das formas |
| `scripts/SectorMap.gd`, `HUD.gd`, `ResultScreen.gd` | Arquipélago, HUD e telas de vitória/derrota |
| `scripts/screens/` | Menu, logotipo, pausa, configurações, como jogar, diálogo, fim de setor |
| `scripts/fx/` | Fenda, Axi-01, Geo, cenário em camadas e efeitos (partículas, onda de choque) |
| `scripts/ui/` | Paleta, tema e tipografia, ícones, botões, medidor de risco, transição |
| `shaders/` | Nebulosa, transição em fenda e desfoque da pausa |
| `assets/fonts/` | Orbitron e Exo 2 (SIL OFL 1.1) |
| `docs/evidencias/v1.4/` | Capturas de todas as telas |

Nenhum sprite ou áudio externo é usado (Pilar 5 do GDD): tudo é desenhado e sintetizado por código.
