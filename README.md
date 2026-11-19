# Danielle Esteves, nutricionista clínica

Página da nutricionista clínica Danielle Esteves (CRN-3 31011, @daniesteves_nutricionista), com consultório em Indaiatuba, SP, e atendimento on-line. Ela não tinha site (usava Linktree); esta é a primeira versão, feita do zero.

Versão 1 (19/11/2026), conceito "feche uma consulta", página dinâmica e imersiva:
- abertura com o ensaio em preto e branco ocupando a tela, monograma "D" ao fundo e o traço champanhe do "E" do logo se desenhando;
- "Mito ou verdade?": baralho de 5 cartas com dúvidas que ela responde nos reels; a carta vira com a resposta e o tema vai para a mensagem do WhatsApp;
- áreas de atendimento (adultos de 18 a 65 anos), passeio horizontal pelo consultório, formas de acompanhamento com traço que se preenche, avaliações do Google em esteira, sobre e na mídia, final escuro.

Textos em linguagem profissional. HTML, CSS e JavaScript puros, sem build. Todos os botões de agendamento abrem o WhatsApp.

## Estrutura

```
index.html                      página completa (estilos, scripts e monograma dentro do arquivo)
img/danielle-terraco.jpg        abertura (ensaio P&B, Instagram)
img/consultorio-recepcao.jpg    passeio: recepção (Google Maps)
img/consultorio-sala.jpg        passeio: sala de atendimento (Google Maps)
img/consultorio-espera.jpg      passeio: sala de espera (Google Maps)
img/danielle-avaliacao.jpg      passeio: avaliação física (Google Maps)
img/danielle-poltrona.jpg       sobre (Google Maps)
img/favicon.png                 ícone da aba (recorte do logo)
img/apple-touch-icon.png        ícone ao salvar na tela do celular
vercel.json                     configuração da Vercel (URLs limpas)
```

Todas as fotos são da Danielle (Instagram e perfil do Google). Nenhuma foi gerada por IA.

## Publicar

1. Crie um repositório no GitHub (ex.: `Danielle_Esteves`) e envie os arquivos desta pasta para a raiz dele.
   Importante: **arraste a pasta `img` inteira** para a área de upload. O botão "choose your files" não envia pastas.
2. Na Vercel, clique em **Add New → Project**, importe o repositório e mantenha:
   - Project Name: `nutri-danielleesteves`
   - Framework Preset: **Other**
   - Build Command: vazio
   - Output Directory: vazio (raiz)
3. Clique em **Deploy**. O site fica em https://nutri-danielleesteves.vercel.app/ e cada novo commit publica a atualização sozinho.

Se usar outro nome de projeto, troque o endereço em `canonical`, `og:url` e `og:image` no `<head>` do `index.html`.

## Atualizar o site já publicado

Envie o `index.html` novo para o repositório. A pasta `img` só precisa subir de novo quando alguma imagem mudar. Ao trocar uma imagem mantendo o mesmo nome, aumente o `?v=1` nos links.

## Editar conteúdo

- WhatsApp: variável `numero` no fim do `index.html` (hoje 5511966132166) e o número exibido no rodapé.
- Mito ou verdade: lista `mitos` no script (afirmação, resposta certa, texto da resposta e tema da mensagem).
- Áreas: lista `.lista-areas`. Horário: painel final do passeio e rodapé.
- Cores: variáveis no início do `<style>` (`--grafite`, `--carvao`, `--greige`, `--areia`, `--creme`, `--champ`).

## A confirmar com a cliente

- WhatsApp: a página usa (11) 96613-2166 (briefing); o perfil do Google mostra (19) 99509-7055.
- Horários: o Google publica só quinta-feira, 13h às 19h; a página diz "demais dias e horários pelo WhatsApp".
- Se trabalha com consulta, acompanhamento de 90 e 180 dias.
- Se pode citar a Rádio Cultura Brasil (Chat MPB) e a palestra na SIPAT da CPFL Energia.
- Tempo de experiência: o Instagram diz 17 anos; a arte do Google, 14 anos de formada (a página usa 17).
- O monograma DE foi redesenhado em SVG a partir do logo; receber o arquivo original.
- Fotos da recepção e da sala de espera em alta resolução (as do Google têm cerca de 750 px).
