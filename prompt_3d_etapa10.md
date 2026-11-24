# Prompt detalhado — Maquete 3D do Templo (Etapa 10)

Objetivo: maquete 3D visual (apresentação, nada técnico) em **um único index.html** com Three.js r128 (unpkg) + OrbitControls, gerada a partir da planta baixa 2D da Etapa 8 (SVG em px; 50 px = 1 unidade ≈ 1 m; X=(px-370)*0,02; Z=(py-900)*0,02).

## Alturas padrão
- Muro à esquerda, Muro à direita, Parede das salas do anexo, Parede do templo externo e paredes das salas do anexo/externas: 3 m.
- Muro frontal: 1 m de base + grade de 2 m; Portão principal (vão x520..640) com pilares de 3 m.
- Portas simples 0,90 x 2,10 m; porta dupla da nave 1,80 x 2,10 m; janelas 1,20 x 1,20 m com peitoril 1,10 m.

## Planta (px)
- Anexo (y40..230): Cozinha (Sala 1), Sala 2, Sala 3 (x50..255, 265..470, 480..685; y50..160); portas à esquerda de cada sala (centros 95, 310, 525); janelas só nas Salas 2 e 3, voltadas ao corredor (x≈410 e 625, y=160). Corredor y170..220; porta de acesso ao anexo em x≈665 (y=225).
- Altar (y230..320): Plataforma 2 a 1,0 m (y230..274); Plataforma 1 a 0,5 m (y274..320); 1/4 de pizza (r=46 px) nos dois extremos, altura da Plataforma 2, unificados; sobre a Plataforma 2 (topo a 1,0 m, olhando da nave para o altar): Bateria no lado direito (x≈560), Teclado no lado esquerdo (x≈110), Guitarra e Baixo em suportes com amplificadores (x≈235 e 305) e local dos Microfones com 3 pedestais (x≈345..405, na frente).
- Nave (y320..720), chamada "Piso": 4 fileiras x 10 bancos (numeração da porta ao altar); Banco 1 da Fileira 1 substituído por Mesa de som. Parede do templo externo (y=720): porta dupla x300..390 e janela x≈520.
- Banheiros (x50..255): Feminino y730..805, Masculino y805..880; 2 box com vaso cada (divisão horizontal), pia (Fem. em cima, Masc. embaixo), parede + corredor de acesso (x=224); portas na parede x=255 (Fem. extremo superior, Masc. extremo inferior). Bebedouro vertical (x645..685, y730..830).
- Cobertura em telhado sobre os 2 banheiros e o bebedouro (x46..700, y722..884), abrigo antes da nave.
- Varanda externa de acesso às salas externas 1 e 2 (x205..255, y880..1180, telhas); Sala 1 externo (y880..1030) e Sala 2 externo (y1030..1180) em x50..205; portas na parede x=205; janela da Sala 2 externo voltada à varanda.
- Estacionamento 1: 5 vagas (x50..250, a partir de y1200). Estacionamento 2: 4 fileiras x 2 vagas em x450..690, começando em y=900 (veículos mais para trás).
- Entorno: calçada com pedrinhas (y≈1763..1870), Rua Elizeu de Alvarenga (larga, y1870..2050, faixa tracejada).

## Cores e acabamentos dos limites
- Grades externas (portão/frente): BRANCAS.
- Muros (esquerda, direita e base frontal de 1 m): metade de cima AZUL, metade de baixo com ladrilhinhos (pequenos ladrilhos bege).
- Paredes das salas externas 1 e 2 e dos banheiros (externas, divisórias dos box e parede do corredor de acesso), nas duas faces: metade de cima AZUL MAIS CLARO (#9cc8ee) e metade de baixo com ladrilhinhos.
- Parede do templo externo (nave x pátio): face EXTERNA (lado do pátio) com a mesma cor do muro (azul em cima, ladrilhinhos embaixo); face interna (nave) inalterada.

## Forros e luzes (somem junto com o Telhado)
- Nave e altar (sob o telhado), salas externas 1 e 2 e banheiros: forro de ISOPOR em placas (padrão de placas ~0,6 m) a ~2,95 m, com luminárias retangulares/redondas no forro.
- Salas do anexo (Cozinha, Sala 2, Sala 3): laje emboçada BRANCA lisa com luzes redondas.
- Vista "Forro e luzes": câmera dentro da nave olhando para cima.

## Telhados
- Todos os telhados (principal, cobertura dos banheiros/bebedouro e varanda): CINZA (#8d9299).

## Formas
- Carros: carroceria arredondada (perfil com capô, para-brisa, teto e porta-malas curvos, bordas chanfradas), vidros escuros, faróis/lanternas e rodas com calota — nada em caixa reta.
- Instrumentos: amplificadores e teclado com cantos arredondados; guitarra/baixo com corpo curvo (lóbulos), braço e cabeça; bateria e pedestais com peças cilíndricas.

## Interface
Botões Telhado / Nomes / Girar; vistas: Visão geral, Entrada, Pátio, Banheiros e varanda, Dentro da nave, Forro e luzes, Altar, Anexo, Vista de cima. Rótulos flutuantes com os nomes oficiais (Cozinha, Sala 2, Sala 3, Altar, Plataforma 1/2, Piso da nave, Mesa de som, Banheiro Feminino/Masculino, Sala 1/2 externo, Varanda, Cobertura, Bebedouro, Estacionamento 1/2, Pátio, Portão principal, Calçada, Rua Elizeu de Alvarenga, Muro à esquerda/direita, Parede do templo externo).

## Regras permanentes
Não alterar o que não foi pedido (especialmente as fileiras de bancos); escopo literal; ao fim de cada etapa entregar este prompt em MD.


## Cobertura do pátio
- A cobertura sobre os banheiros e o bebedouro fica SEM colunas (removidas a pedido). Os postes da varanda (x252) permanecem.

## Portas e janelas das salas (anexo e externas)
- Portas de madeira (folha 0,86 x 2,08 m, cor #8b5e3c, almofadas mais escuras, maçaneta dourada, batente marrom escuro), fechadas, nas aberturas já existentes: Cozinha (x95), Sala 2 (x310), Sala 3 (x525) na parede y=160; Sala 1 externa (y955) e Sala 2 externa (y1090) na parede x=205.
- Janelas (1,20 x 1,20 m, peitoril 1,10 m, vidro azul claro translúcido, esquadria e peitoril brancos, montante central): anexo – Cozinha (x200, nova), Sala 2 (x410), Sala 3 (x625); salas externas – Sala 2 externa (y1146 na parede x=205), (as 2 janelas que existiam na parede do fundo x=50 das salas externas foram EXCLUÍDAS a pedido; a parede do fundo fica sem janelas).
- Helpers no código: doorLeaf(horiz, fixed, c) e winFrame(horiz, fixed, c).
- Não mexer nas portas dos banheiros, na porta dupla da nave nem em nada fora do pedido.

## Porta dupla da nave e janela (parede nave x pátio, y=720)
- Porta dupla (x300..390, 1,80 m de vão) em VIDRO TEMPERADO: duas folhas de vidro verde-claro translúcido (opacidade ~0,32), ferragens/perfis metálicos cinza (#6b7075) em cima, embaixo e nas laterais, dois puxadores verticais inox no centro do vão e verga superior metálica.
- A janela da nave (x520) segue o MESMO modelo das janelas das salas (1,20 x 1,20 m, peitoril 1,10 m, vidro azul claro, esquadria e peitoril brancos, montante central): winFrame(true, 720, 520).

## Portas de madeira dos banheiros
- Porta de entrada de cada banheiro (acesso à pia), na parede x=255: Feminino (y730..774,5) e Masculino (y837,5..880) — folha de madeira #8b5e3c 0,86 x 2,08 m, fechada, com almofadas, maçaneta e batente marrom escuro.
- Portas dos boxes (acesso aos vasos), na divisória x=154: 2 por banheiro, centradas nos vasos (y0+20,5 e y0+53,5, com y0 = 730 Feminino / 805 Masculino) — folha de madeira 0,40 x 1,68 m, fechadas, mesmo acabamento.
- Helper: doorLeaf(horiz, fixed, c, largura, altura, espessuraBatente).

## Piso do pátio
- Piso do pátio (x40..700, y720..1760) em CIMENTO QUEIMADO: cinza médio (#9a9a96) com manchas suaves claras/escuras e granulação, textura em canvas repetida em placas de 3 x 3 m com junta de dilatação fina. Roughness 0,9. Faixas das vagas continuam verdes por cima. Substituiu a cor verde-clara anterior (#dfeedd).

## Piso da nave e tapete das plataformas
- Piso da nave (x40..700, y320..720): cor CLARA — porcelanato bege claro (#f0ebdf) com placas de 0,6 m e juntas suaves (substituiu o verde-água #bfe6dc).
- Tapete MARROM (#6a4326, textura felpuda, espessura 2,5 cm) sobre as plataformas: Plataforma 2 (x48..622, y238..266, topo 1,00 m), Plataforma 1 (x94..576, y280..314, topo 0,50 m) e sobre os dois 1/4 de círculo dos extremos (topo 1,00 m). Margem de ~8 px de borda sem tapete para mostrar o acabamento amarelo das plataformas.

## Paredes internas da nave e do altar
- Paredes INTERNAS da nave e do altar em cinza claro (#d2d4d7), aplicadas como revestimento fino (1,2 cm) só na face interna: lateral esquerda (x40, y225..720), lateral direita da nave (x700, y320..720), lateral direita do altar (x630, y225..320), fundo do altar (y225, x40..630) e a parede do pátio pelo lado de dentro (y720), com recortes na porta dupla (x300..390) e na janela (x520). As faces externas e as paredes das salas do anexo NÃO mudam de cor.

## Muretas das plataformas (50 cm)
- Os corpos/muretas das Plataforma 1 (0,50 m) e Plataforma 2 (1,00 m), incluindo os 1/4 de círculo dos extremos, ficam em cinza claro #d2d4d7 (C.plat1 = C.plat2 = 0xd2d4d7), no mesmo tom das paredes internas da nave. O tapete marrom continua por cima. Substituiu o amarelo (#f8e0a0 / #f1c25d).

## Altura da Plataforma 2
- O degrau da Plataforma 2 passa de 50 cm para 20 cm acima da Plataforma 1: Plataforma 1 continua com topo a 0,50 m; Plataforma 2 agora tem topo a 0,70 m (antes 1,00 m). Ajustados juntos: 1/4 de círculo dos extremos (altura 0,2 m, topo 0,70 m), tapete da Plataforma 2 (topo 0,70 m) e todos os instrumentos/microfones (base P = 0,70 m). Os valores de 1,00 m citados nas seções anteriores valem agora 0,70 m.

## Altura da Plataforma 1
- Plataforma 1 passa de 50 cm para 20 cm de altura (topo a 0,20 m). Mantido o degrau de 20 cm da Plataforma 2 sobre a Plataforma 1, então a Plataforma 2 passa a ter topo a 0,40 m (antes 0,70 m). Ajustados juntos: 1/4 de círculo dos extremos (de 0,20 a 0,40 m), tapetes (Plataforma 1 topo 0,20 m; Plataforma 2 e quarto de círculo topo 0,40 m) e instrumentos/microfones (P = 0,40 m). Esta seção substitui os valores das seções anteriores sobre alturas das plataformas.

## Parede removida ao lado da bateria
- EXCLUÍDA a parede x=630 (y225..320) que ficava entre o altar (ao lado da bateria) e o corredor de acesso ao anexo (x630..700, y220..320), junto com o revestimento cinza dela. O corredor passa a ficar aberto para o altar. O restante (parede divisória y=225 com a porta do anexo em x665, parede x=700) não muda. Na planta 2D não alterei nada.

## Porta de acesso ao anexo
- Porta de madeira (0,86 x 2,08 m, #8b5e3c, almofadas, maçaneta, batente marrom escuro, fechada) na abertura de acesso ao anexo: parede divisória y=225, centro x=665 (corredor ao lado da bateria). doorLeaf(true, 225, 665, 0.86, 2.08, 0.2).

## Painel de MDF amadeirado (parede divisória nave x anexo, lado interno)
- Na face INTERNA (voltada para a nave/altar) da parede divisória y=225 foi aplicado painel de MDF com acabamento de madeira (tom #a87649–#b98557, veios verticais, juntas escuras entre chapas de ~1,2 m), do chão ao topo (3 m), x40..642,5 e x687,5..700 (deixando livre o vão da porta de acesso ao anexo em x665). Substituiu o revestimento cinza claro nesse trecho; as demais paredes internas da nave continuam cinza claro (#d2d4d7). Espessura 2 cm.

## MDF sobre a porta de acesso ao anexo
- O painel de MDF amadeirado agora é contínuo em toda a parede y=225 (x40..700), cobrindo também a porta de acesso ao anexo (x665) pelo lado da nave/altar. A porta de madeira continua atrás (fecha o vão); na face do MDF há só um contorno discreto escuro da porta (0,92 x 2,10 m) e um puxador dourado pequeno em x≈665+0,34 m, altura 1,0 m. Isto substitui o recorte do vão descrito na seção anterior ("deixando livre o vão da porta").

## Parede do altar (divisória nave x anexo, lado da nave) inspirada nas fotos de referência
Referência: fotos do próprio templo (parede de fundo do altar). Pessoas das fotos foram ignoradas. Elementos reproduzidos de forma simples/estilizada na face interna da parede y=225 (x40..700), de z = Z(225)+0,13:
- Painel de MDF ripado em madeira ESCURA (nogueira/marrom escuro): ripas verticais de ~20 cm com frestas escuras e veios; juntas de chapa a cada ~1,2 m; contínuo, cobrindo também a porta de acesso ao anexo (contorno discreto + puxador).
- Letreiro OVAL vertical centralizado no altar (centro em x=335 px, altura 1,75 m; 1,32 x 1,80 m) em grafite escuro com aro de madeira clara; dentro: cruz AZUL e coração vazado (contorno) VERMELHO/ROSA em LED (materiais sem sombreamento) + arco azul de LED na base.
- Faixa de LED QUENTE (#ffc16b) ao longo do pé da parede, logo acima da plataforma (y≈0,62 m, x48..630) com brilho suave aditivo acima.
- Dois SPLITS (ar-condicionado) brancos altos (1,15 x 0,30 x 0,22 m, y=2,5 m) em x=170 e x=510 px, um de cada lado do letreiro, com friso e LED verde.
- Duas CAIXAS DE SOM pretas penduradas perto do teto nos cantos (x=70 e x=600 px, y≈2,3 m, a 0,4 m da parede, com haste de fixação).
- Não incluído (só nas fotos, não pedido): painéis acústicos cinza das paredes laterais, ventiladores, púlpito de acrílico, telão, banners.

## Pátio, fachada e salas externas inspirados na foto de referência
Referência: foto do pátio com as salas à esquerda e a fachada. Imitados só a arquitetura e os detalhes — NÃO foram usados a cor azul da foto (a maquete mantém as cores já definidas) nem os veículos da foto.
- Telha metálica trapezoidal cinza (#8d9299 com nervuras claras/escuras) na cobertura do pátio (sobre banheiros/bebedouro) e na varanda das salas externas (nervuras no sentido da inclinação). Sem colunas sob a cobertura (continua como pedido antes); postes da varanda mantidos.
- Gradil decorativo quadriculado BRANCO (1,3 x 1,3 m, 6x6 com detalhes nos cruzamentos) nas janelas voltadas ao pátio: janela da nave (x520, y=720, lado do pátio) e janela da Sala 2 externa (lado da varanda).
- Ar-condicionado split brancos na fachada (à esquerda da porta de vidro, x≈262, y=2,4 m) e na parede da Sala 1 externa voltada à varanda (y≈1000, y=2,35 m); condensadora cinza no chão à direita da porta de vidro (x≈448).
- Capacho escuro e soleira de concreto na porta de vidro da nave.
- Canteiro de concreto (0,84 x 1,6 m x 0,5 m) com 3 arbustos, ao lado da varanda (x258..300, y1100..1180).
- Estrutura metálica retangular (grafite #3b3f44, 2,0 x 1,6 m) sobre a cobertura, no centro da fachada (x295..395, sobre y≈803) — some junto com o telhado.
- Caixa d'água cilíndrica cinza claro com tampa e cintas sobre a laje das salas externas (x≈110, y≈1000) — some junto com o telhado.
- Piso do pátio continua em cimento queimado.

## Corredor em frente às salas do anexo mais largo (SUBSTITUI valores anteriores)
- O corredor de acesso em frente às salas do anexo (Cozinha, Sala 2, Sala 3) passa de 1,0 m para 1,5 m de largura (piso do corredor y145..220 em px; antes y170..220).
- O espaço vem da profundidade das salas: a parede frontal das salas passa de y=160 para y=135 (salas y50..135, ~1,7 m de fundo). A parede divisora com a nave (y=225) e o resto do templo não mudam.
- Acompanharam a mudança: paredes laterais das salas (vwall 260 e 475 até y135), portas de madeira e janelas (agora em y=135), laje/forro das salas (profundidade 85 px, centro y92,5), luzes e rótulos das salas (y≈92).
- Planta 2D (gen.py) ajustada igual: salas até y=135, corredor de y=145 a 220, portas/janelas e arcos de porta em y=135.
- Corredor ao lado da bateria (x630..700) NÃO foi alterado.
