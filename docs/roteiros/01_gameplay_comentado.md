# Roteiro 1: Gameplay comentado

**Duração planejada: 14 min 30 s** (mínimo exigido: 10 min) · **Exibição em aula: 03/12**

Como usar: **TELA** é o que fazer no jogo; as citações são a fala-guia. É para soar como live: não leia palavra por palavra. Preencha tudo que está entre `[colchetes]`.

| # | Bloco | Início | Duração | Quem fala |
|---|---|---|---|---|
| 1 | Grupo e jogo | 0:00 | 0:50 | `[pessoa 1]` |
| 2 | Proposta, história e objetivo | 0:50 | 1:30 | `[pessoa 1]` |
| 3 | Menu e aprendizado dos controles | 2:20 | 2:00 | `[pessoa 2]` |
| 4 | Setor Alpha | 4:20 | 3:00 | `[pessoa 3]` |
| 5 | Setor Beta | 7:20 | 2:00 | `[pessoa 3]` |
| 6 | Setor Gamma e final | 9:20 | 2:00 | `[pessoa 4]` |
| 7 | Devolutivas, antes e depois | 11:20 | 2:30 | `[pessoa 2]` |
| 8 | Encerramento | 13:50 | 0:40 | todos |

## 1. Grupo e jogo (0:00)
**TELA:** tela inicial, sem apertar nada. Na edição, sobrepor os nomes.

> Fala, pessoal! Nós somos o grupo `[nome do grupo]`, do curso de Engenharia de Software da Católica de Santa Catarina, e este é o Geometry Survival: O Cálculo Final. O grupo é formado por `[nomes completos]`. Eu sou `[nome]` e vou começar. Hoje a gente vai jogar com vocês desde a primeira tela, explicar como tudo funciona e mostrar o que mudou desde as versões anteriores. O jogo foi feito em Godot 4. Todos os desenhos e sons são gerados por código: a gente não usou nenhuma imagem nem áudio pronto. As únicas coisas externas são as fontes.

## 2. Proposta, história e objetivo (0:50)
**TELA:** continuar na tela inicial; apertar uma tecla e deixar o menu com Axi-01 e a fenda.

> A proposta é um jogo sério para o Ensino Médio, para praticar área de figuras planas. Em vez de resolver uma lista de exercícios, o cálculo vira a ação do jogo: a sua arma é a geometria.
>
> A história se passa no Arquipélago Dimensional, um conjunto de ilhas flutuantes. Uma força chamada Entropia está abrindo fendas nesse lugar, e de cada fenda sai uma Forma Caótica. Essa personagem na tela é Axi-01, a Arquiteta Dimensional. Quem joga assume o papel dela. Com ela está Geo, uma inteligência artificial em forma de drone, que analisa o perigo de cada fenda.
>
> Para fechar uma fenda, Axi precisa calcular a área exata da forma que saiu dela. Acertou, a fenda é selada. Errou, ela resiste, e se for uma fenda instável, se expande e Axi perde uma vida. O objetivo é atravessar três setores, com três fendas cada, sem perder as três vidas, e restaurar o arquipélago.
>
> Percebam que a matemática e a história são a mesma coisa aqui: não existe combate separado do cálculo.

## 3. Menu e aprendizado dos controles (2:20)
**TELA:** navegar por todas as opções com ↑ e ↓, sem usar o mouse.

> Vamos fingir que eu nunca joguei. O menu já mostra, no canto inferior direito, as setas para navegar e Enter para selecionar. Também dá para usar o mouse. Continuar está apagado porque ainda não existe partida salva. Quem está perdido vai em Como Jogar.

**TELA:** abrir **Como Jogar**; ficar cerca de 15 s por página, avançando com →.

> São quatro páginas ilustradas com os próprios elementos do jogo. A primeira ensina a olhar as medidas na forma. A segunda explica o risco: até setenta por cento a fenda é estável e errar não custa vida; acima disso, acertar dá bônus, mas errar custa uma vida. A terceira mostra como responder: digitar a área, com vírgula ou ponto, e apertar Enter. E a quarta apresenta os setores e as três vidas.

**TELA:** fechar em **Entendi**; abrir **Configurações** e mover o volume da música.

> Em Configurações a gente separa música e efeitos, e tem opções de acessibilidade: dá para desligar o tremor de tela e reduzir o movimento. Vou abaixar a música para vocês me ouvirem bem.

**TELA:** voltar e escolher **Jogar**.

## 4. Setor Alpha (4:20)
**TELA:** no mapa, passar por Beta e Gamma bloqueados; entrar em Alpha.

> Esse é o mapa. Beta e Gamma estão com cadeado: precisa concluir um para abrir o próximo. Vamos no Alpha, as Planícies Euclidianas, com quadrado, retângulo e triângulo.

**TELA:** onda 1. Antes de responder, apontar cada área da tela com o mouse.

> A fenda abriu e a forma foi construída na nossa frente. Em cima ficam pontuação, setor, onda e vidas. Embaixo, Geo conversa comigo; no meio está a fórmula e o campo da resposta; e à direita o medidor de risco. Não tem relógio: a ideia é pensar, não correr.

**TELA:** deixar vazio e apertar Enter; depois digitar `abc` e Enter.

> Olha que legal: se eu confirmo vazio ou digito letras, Geo me orienta e eu não perco a onda. É erro de digitação, não de matemática.

**TELA:** resolver **em voz alta** e acertar.

> Aqui a forma é `[quadrado/retângulo]`, com `[medidas]`. Então a área é `[conta]`, que dá `[resultado]`. Enter… e a fenda foi selada! Cem pontos.

**TELA:** onda 2. Se o risco for até 70%, **errar de propósito** (ex.: digitar o dobro do resultado). Se passar de 70%, acertar e deixar o erro para a onda 3 ou para o Beta.

> Agora vou errar de propósito, para vocês verem. O risco está em `[x]` por cento, então é estável. A fenda resistiu, mas não perdi vida, e apareceu a resolução passo a passo. O jogo nunca diz simplesmente "errado": ele mostra como chegar ao resultado. Errar também avança a onda.

**TELA:** onda 3, acertar; apertar **Esc**, mostrar a pausa e continuar; depois **Concluir setor**.

> A terceira onda já é mais difícil: normalmente um triângulo, às vezes com resultado quebrado. No triângulo o esquecimento clássico é dividir por dois. E se eu precisar parar, Esc abre a pausa, com o Como Jogar de novo. Fim de setor: as estrelas mostram quantas fendas eu selei, e o Beta foi liberado.

## 5. Setor Beta (7:20)
**TELA:** mostrar o desbloqueio no mapa e entrar no Beta.

> Câmara dos Arcos: aqui é tudo círculo. Cor e música mudaram. A área é pi vezes raio ao quadrado, e usando três vírgula catorze está ótimo. O jogo aceita uma margem de cinco por cento, e até pi igual a três passa. Mas se a pessoa confundir área com comprimento da circunferência, em geral não passa.

**TELA:** resolver as ondas 1 e 2 em voz alta. Na onda 2, o raio termina em ,5.

> Raio `[x]`, ao quadrado dá `[y]`, vezes três vírgula catorze, dá `[resultado]`.

**TELA:** onda 3; não responder até ler o aviso.

> Agora a pegadinha: Geo avisa que informou o diâmetro. Quem usar direto erra feio. O raio é a metade, `[valor]`. Só então eu faço a conta. Selada! O risco aqui pode chegar a noventa por cento, e numa fenda instável cada acerto vale cento e cinquenta.

## 6. Setor Gamma e final (9:20)
**TELA:** entrar no Gamma.

> Último setor: Nexo da Entropia. Tudo ficou vermelho e a música acelerou. Agora as formas são compostas. O segredo é separar: aqui tem um retângulo e um triângulo, com cores diferentes para ajudar. Calculo um, calculo o outro e somo. Retângulo `[conta]`, triângulo `[conta]`, total `[resultado]`.

**TELA:** onda 2, retângulo + semicírculo.

> Agora é um semicírculo: o raio é metade da largura, e a área do círculo é dividida por dois.

**TELA:** onda 3, "Fenda do Líder Aleatório". Pausar a fala para criar tensão.

> Essa é a Fenda do Líder Aleatório: pode ser qualquer composta, e maior. Vou conferir duas vezes… e foi!

**TELA:** tela de vitória, sem cortar a contagem da pontuação.

> Arquipélago restaurado! Aparecem a pontuação, a precisão e o desempenho por setor. Se eu tivesse perdido as três vidas, a Entropia avançaria, e o jogo mostraria a resolução da última fenda antes de convidar para tentar de novo.

*Se perder durante a gravação, aproveite: mostre a tela de derrota e siga para o bloco 7.*

## 7. Devolutivas: antes e depois (11:20)

> **Confirmem antes de gravar:** o repositório registra as mudanças, mas **não registra as devolutivas do professor, da turma ou dos testadores**. Preencham quem apontou cada coisa e o que disse. Se um item veio da revisão da própria equipe, digam isso. Removam os que não vieram de devolutiva e incluam os que faltarem.

**TELA:** imagens lado a lado (pasta `docs/evidencias/`), cerca de 25 s por item.

| Devolutiva recebida (preencher) | Antes | Depois | Imagens |
|---|---|---|---|
| `[quem / o que disse]` | Formas do Gamma cobriam a interface | Escala automática | `v1.3/baseline_gamma_overflow.png` → `v1.4/19_gamma.png` |
| `[quem / o que disse]` | Visual simples, sem a fenda | Fenda, Axi-01, Geo, cenário e áudio | `v1.3/02_alpha_triangulo.png` → `v1.4/10_encounter.png` |
| `[quem / o que disse]` | Texto "ERRADO!" e erro de alto risco sem a área correta | Feedback narrativo e resolução | sem print do antes; `v1.4/13_expand.png` |
| `[quem / o que disse]` | Tolerância de ±10%; Beta e Gamma abertos desde o início | ±2% / ±5%; desbloqueio em sequência | sem print do antes; `v1.4/08_map.png` |
| `[quem / o que disse]` | Abria direto no mapa, sem tutorial | Menu, Como Jogar e Configurações | `v1.3/01_mapa_inicio.png` → `v1.4/03_menu.png` |

> Agora, o que mudou. `[Origem]` nos apontou que `[devolutiva]`. Antes, no Gamma, a forma cobria o risco, o campo e até o botão. Hoje a escala é automática e cada medida fica ao lado da sua aresta.
>
> Depois, `[devolutiva]`. Esse era o visual da versão um ponto três: o cálculo já funcionava, mas a fenda, que é o centro da história, não aparecia. Na um ponto quatro entraram a fenda, Axi, Geo, os cenários e todo o áudio.
>
> O terceiro ponto foi `[devolutiva]`. O jogo escrevia "errado" e, com risco alto, a pessoa perdia a vida sem saber a resposta. Hoje a fenda reage na história e todo erro traz a resolução.
>
> Em `[devolutiva]`, a tolerância era de dez por cento: num quadrado de área quarenta e nove, quarenta e cinco era aceito. Baixamos para dois por cento no Alpha e cinco nos outros. E os setores, que abriam todos de uma vez, agora são liberados em ordem.
>
> Por último, `[devolutiva]`: quem abria o jogo caía direto no mapa. Agora tem menu, tutorial e configurações, como vocês viram no começo.

## 8. Encerramento (13:50)
**TELA:** voltar ao menu.

> Esse foi o Geometry Survival: O Cálculo Final. O que mais gostamos de fazer foi `[resposta]`, e o maior desafio foi `[resposta]`. Se fôssemos continuar, o próximo passo seria `[resposta]`. Obrigado por assistir, e lembrem: a geometria é a sua arma!

---

## Checklist de gravação
- [ ] Gravar 1080p a 30 ou 60 fps (OBS), com **microfone e jogo em faixas separadas**.
- [ ] No jogo, música em cerca de 20% e efeitos em 40%; na edição, jogo uns 15 a 20 dB abaixo da voz.
- [ ] Gravar 30 s de teste e ouvir no celular e em caixa de som: todas as falas devem ser entendidas.
- [ ] Ter calculadora à mão e um ensaio completo antes.
- [ ] Os desafios são sorteados: calcular ao vivo, sem decorar resultados.
- [ ] Para mostrar **Continuar** apagado, gravar sem partida salva. Se já houver uma, adaptar essa frase do bloco 3 e confirmar "Nova partida" (isso substitui o salvamento).
- [ ] Conferir que o vídeo final tem **mais de 10:00**. Se ficar curto, resolver também um erro em fenda instável e mostrar a vida perdida.
- [ ] Testar o arquivo no computador da sala antes de 03/12.
