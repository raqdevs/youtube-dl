# youtube-dl
Estudos de caso do youtube-dl

## Baixar playlist do Youtube Music (em testes para youtube padrão)
Baixar e converter para .mp3 todos os audios das playlists do Youtube Music utilizando as ferramentas youtube-dl e ffmpeg

```
@echo off
set /p url=Enter URL: 
youtube-dl -ciw -o "%%(uploader)s - %%(playlist)s/%%(playlist_index)s - %%(title)s.%%(ext)s" --add-metadata --xattrs -x --audio-format mp3 %url%

pause
```
Nesse caso utilizaremos a configuração folder - playlist / playlist_index - title - ext ou seja Chiclete com Banana - Chiclete Na Caixa, Banana No Cacho / 01 Voa Voa (Ao Vivo).mp3
