# Cartucho 4 em 1 🕹️

Quatro jogos de arcada num só site: dois a solo, um competitivo e um cooperativo, para jogar no mesmo teclado.

**▶ Jogar:** https://danianecrissouza99-creator.github.io/Projeto_Cartucho/

---

## Sobre o projeto

Projeto da UC **Testes e Qualidade de Software**, ISTEC.

O Cartucho foi feito para ser **testado por um colega**. O trabalho do testador é comparar o que cada jogo **faz** com o que **devia fazer**, segundo as regras abaixo (requisitos). Cada diferença é um defeito a registar no relatório.

- Funciona no browser, sem instalar nada. Os jogos a dois jogam-se no mesmo teclado.
- O ranking e as definições ficam gravados no próprio browser.

| Jogo | Modo |
|---|---|
| **Nebula Strike** | Solo: nave espacial contra ondas de inimigos |
| **Tank Duel** | Competitivo: dois tanques numa arena, ganha quem vencer 3 rondas |
| **Guardiões** | Cooperativo: dois jogadores defendem o reator |
| **Demolição** | Solo: partir blocos com a bola e a raquete |

No menu escolhe-se o jogo com o rato ou com as teclas 1 a 4.

---

## Requisitos de cada jogo

Isto é o que cada jogo **deve** fazer. Os IDs começam pelas iniciais do jogo (NS, TD, GU, DM).

### Nebula Strike — Solo · 1 jogador

**Controlos**

| Tecla | Ação |
|---|---|
| Setas ou W A S D | Mover a nave |
| Automático | A nave dispara sozinha |
| P ou Esc | Pausa |
| M | Ligar / desligar som |

**Regras**

| ID | Regra |
|---|---|
| NS-R1 | A nave nunca sai do ecrã, em nenhum dos lados. |
| NS-R2 | Vidas no início: Fácil = 5, Normal = 3, Difícil = 2. As vidas são as navezinhas no canto inferior esquerdo. |
| NS-R3 | Nunca se pode ter mais de 5 vidas. |
| NS-R4 | Depois de perder uma vida, a nave pisca 2 segundos e não pode ser atingida. |
| NS-R5 | Pontos: rocha = 100, caça (nave vermelha) = 200, kamikaze = 150, sentinela = 300, rocha divisora = 250, enxame = 50 cada, nave-mãe = 2 000. |
| NS-R6 | Cada inimigo destruído mostra os pontos que deu (ex.: "+100"). |
| NS-R7 | As ondas aparecem por ordem: Onda 1, Onda 2, Onda 3… sem saltar nenhuma. |
| NS-R8 | A nave-mãe aparece nas ondas 5, 10, 15… |
| NS-R9 | 2x = tiro duplo durante 10 segundos. |
| NS-R10 | E = escudo. Protege de 1 impacto de qualquer tipo: rocha, caça ou tiro. |
| NS-R11 | ♥ = +1 vida (sem passar das 5). |
| NS-R12 | Em pausa tudo para. |
| NS-R13 | Com o som desligado não se ouve nada. |
| NS-R14 | Para guardar no ranking, o nome tem de ter entre 3 e 10 letras. Se ficar vazio ou for curto, aparece um erro e não guarda. |
| NS-R15 | O ranking mostra os 10 melhores, do maior para o menor. |
| NS-R16 | "Jogar de novo" começa do zero: 0 pontos e onda 1. |
| NS-R17 | Todos os textos estão em português correto. |
| NS-R18 | Os inimigos novos aparecem aos poucos: Kamikaze (onda 3), Sentinela (onda 4), Rocha divisora (onda 6) e Enxame (onda 8). Na primeira vez aparece o aviso "Novo inimigo". |
| NS-R19 | O Kamikaze para, aponta à nave e mergulha. A Sentinela fica no topo e dispara 3 tiros apontados. A Rocha divisora parte-se em 2 rochas pequenas. |
| NS-R20 | Cada onda é mais difícil: inimigos mais rápidos e mais frequentes. A nave-mãe fica mais forte de cada vez que volta. |

### Tank Duel — Competitivo · 2 jogadores

**Controlos**

| Tecla | Ação |
|---|---|
| J1: W A S D | Mover |
| J1: Espaço | Disparar |
| J2: Setas | Mover |
| J2: Enter | Disparar |
| P ou Esc | Pausa |
| M | Ligar / desligar som |

**Regras**

| ID | Regra |
|---|---|
| TD-R1 | Cada jogador pode escrever o nome (até 12 letras). Se ficar vazio, aparece "Jogador 1" ou "Jogador 2". |
| TD-R2 | Os dois tanques andam exatamente à mesma velocidade. |
| TD-R3 | Os tanques não atravessam paredes e não saem da arena por nenhum lado. |
| TD-R4 | Cada tanque tem 3 de vida por ronda (as barrinhas). Nunca pode ter mais de 3. |
| TD-R5 | Cada tiro que acerta tira 1 de vida. |
| TD-R6 | Os tiros ressaltam 1 vez nas paredes. Nenhuma parede deixa passar tiros. |
| TD-R7 | O teu próprio tiro, depois de ressaltar, pode acertar-te. Se morreres assim, a ronda é do adversário. |
| TD-R8 | Ganha a partida quem chegar primeiro a 3 rondas ganhas (os losangos no painel). Vale para os dois jogadores. |
| TD-R9 | E = escudo: aguenta o próximo tiro. |
| TD-R10 | V = mais velocidade durante 5 segundos. |
| TD-R11 | + = reparação: +1 de vida, sem passar de 3. |
| TD-R12 | Em pausa nada se mexe e ninguém pode disparar. |
| TD-R13 | Aparece uma tabela com vitórias, tiros, acertos e precisão (%). Quem não disparou tem 0% de precisão. |
| TD-R14 | "Nova partida" começa com tudo a zero, incluindo tiros e acertos. |
| TD-R15 | Todos os textos estão em português correto. |

### Guardiões — Cooperativo · 2 jogadores

**Controlos**

| Tecla | Ação |
|---|---|
| J1: W A S D | Mover |
| J2: Setas | Mover |
| Automático | Os dois disparam sozinhos |
| P ou Esc | Pausa |
| M | Ligar / desligar som |

**Regras**

| ID | Regra |
|---|---|
| GU-R1 | Os jogadores não saem do mapa e não atravessam o reator (o círculo amarelo no meio). |
| GU-R2 | Cada jogador tem 3 corações. Quando um inimigo lhe toca, perde 1 e pisca durante 1,5 segundos (nesse tempo não perde mais). Vale para os dois. |
| GU-R3 | Com 0 corações o jogador fica caído: não se mexe e não dispara. |
| GU-R4 | Para reanimar, o parceiro fica ao lado do caído durante 2 segundos. O reanimado volta com 2 corações. |
| GU-R5 | O reator tem no máximo 100 de energia (topo do ecrã, ex.: "100 / 100"). Nunca passa de 100. |
| GU-R6 | No início de cada onda, a partir da 2.ª, o reator recupera +10, sem passar de 100. |
| GU-R7 | Os inimigos entram pelos 4 lados do mapa. |
| GU-R8 | Pontos: drone = 50, couraçado = 150, corredor = 75, atirador = 120, ninho = 300, colosso = 1 000. Os pontos são da equipa e valem o mesmo para os dois jogadores. Cada inimigo destruído mostra os pontos ("+50"). |
| GU-R9 | O contador "Inimigos restantes" desce sempre que um inimigo desaparece e chega a 0 no fim da onda. |
| GU-R10 | O jogo acaba quando o reator chega a 0 ou quando os dois jogadores estão caídos. |
| GU-R11 | Todos os textos estão em português correto. |
| GU-R12 | Em pausa tudo para. |
| GU-R13 | Inimigos novos: Corredor (onda 3), Atirador (onda 4) e Ninho (onda 6). O Colosso (boss) aparece a cada 5 ondas. Na primeira vez aparece o aviso "Novo inimigo". |
| GU-R14 | O Atirador para longe e dispara contra o reator (5 de dano por tiro). Um jogador pode bloquear esses tiros pondo-se à frente, sem perder corações. |
| GU-R15 | Quando um Ninho é destruído saem 3 drones, e o contador "Inimigos restantes" sobe 3. |

### Demolição — Solo · 1 jogador

**Controlos**

| Tecla | Ação |
|---|---|
| Setas, A / D ou rato | Mover a raquete |
| Espaço ou clique | Lançar a bola |
| P ou Esc | Pausa |
| M | Ligar / desligar som |

**Regras**

| ID | Regra |
|---|---|
| DM-R1 | A raquete anda à mesma velocidade com as setas e com A / D. |
| DM-R2 | A raquete nunca sai do ecrã, em nenhum dos lados. |
| DM-R3 | No início e depois de perder uma vida, a bola fica parada em cima da raquete até carregares em Espaço. |
| DM-R4 | Se a bola bater no lado esquerdo da raquete vai para a esquerda; no lado direito vai para a direita. |
| DM-R5 | Bloco bege = 10 pontos. Bloco amarelo = 30 pontos (precisa de 2 toques). Bloco cinzento (metal) nunca parte. Cada bloco partido mostra os seus pontos ("+10"). |
| DM-R6 | Combo: blocos partidos seguidos dão pontos extra. Quando a bola toca na raquete, o combo acaba e o aviso COMBO desaparece. |
| DM-R7 | O nível só acaba quando já não sobra nenhum bloco bege ou amarelo. Aparece "Nível concluído!". |
| DM-R8 | Começas com 3 vidas. Cada vida é uma barrinha no canto inferior esquerdo. |
| DM-R9 | ↔ = raquete larga durante 10 s. L = bola lenta durante 8 s. ♥ = +1 vida (máximo 5). |
| DM-R10 | Em pausa tudo para. |
| DM-R11 | Há 5 níveis com desenhos diferentes. Depois do 5.º recomeçam, mais rápidos. |
| DM-R12 | A partir do nível 2 aparecem morcegos (50 pontos, 1 toque) e a partir do nível 3 aranhas (100 pontos, 2 toques). A bola ressalta neles. |

---

## Como registar um defeito

Para cada defeito encontrado, sugere-se registar:

| Campo | O que escrever |
|---|---|
| **ID** | D-01, D-02… |
| **Jogo** | Nebula Strike, Tank Duel, Guardiões ou Demolição |
| **Título** | Frase curta com o problema |
| **Requisito** | A regra que não é cumprida (ex.: NS-R2) |
| **Passos para reproduzir** | 1. Abrir… 2. Carregar em… 3. … |
| **Resultado esperado** | O que a regra diz |
| **Resultado obtido** | O que aconteceu |
| **Severidade** | Alta, Média ou Baixa |
| **Evidência** | Captura de ecrã ou vídeo |

**Dica:** para limpar o ranking e recomeçar do zero, apague os dados do site (F12 → Application → Local Storage).

---

## Tecnologias

HTML, CSS e JavaScript, sem bibliotecas. Os jogos são desenhados com a Canvas API e os sons gerados com a Web Audio API.

---

Daniane Christyni Souza da Silva · Desenvolvimento de Software, 2.º ano · ISTEC
