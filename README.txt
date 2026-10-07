CHOOSE EVERYTHING! — V3.1 (ANIME IMAGES)
=========================================

NOVIDADES DESTA VERSÃO
- Todos os 100 cards da categoria Anime possuem mapeamento de imagem específico por personagem.
- Tanjiro usa a imagem local enviada pelo usuário: public/assets/tanjiro.png.
- Para os outros personagens de anime, o servidor tenta, nesta ordem:
  1) Jikan / MyAnimeList
  2) AniList
  3) Kitsu
  4) Wikipedia/Wikimedia
- Cada personagem usa um nome canônico próprio para evitar que formas como Ultra Instinct, Gear 5 e GER procurem a pessoa errada.
- As imagens remotas são repassadas pelo próprio servidor para reduzir imagens quebradas por hotlink.
- Se todos os provedores estiverem temporariamente indisponíveis, aparece um fallback visual em vez de uma imagem quebrada.
- O endpoint /api/health mostra animeImageMappings: 100.

MANTIDO DA V3
- 1.500 cartas no total.
- Botão COBRIR +1.
- Botão PASSAR.
- Modos 1v1, 1v1v1, 1v1v1v1, 2v2 e 3v3.
- Leilão por rodadas, sons, salas online e juiz final por IA quando OPENAI_API_KEY estiver configurada.
- O juiz agora é instruído a respeitar a forma/transformação escrita no nome da carta.

ATUALIZAR O RAILWAY
1. Extraia este ZIP.
2. No GitHub, substitua os arquivos do repositório pelos desta versão:
   - server.js
   - cards.json
   - anime-images.json
   - package.json
   - README.txt
   - pasta public/ inteira
3. Faça Commit changes.
4. O Railway deve redeployar automaticamente.

IMPORTANTE SOBRE AS FOTOS
O Tanjiro está embutido no pacote. Os outros 99 personagens de anime têm mapeamento individual,
mas a foto é obtida em tempo de execução de bases públicas. Se uma dessas bases ficar fora do ar,
o jogo tenta as próximas automaticamente.
