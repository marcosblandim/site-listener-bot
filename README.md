# site-listener-bot
a telegram bot that listens to changes on a website

## TODO
- ver como qual seria o chat_id default (todos, ou o ultimo que falou com o bot?)

## regras de negócio
- é feito um schedular do mesmo tipo do crontab, programaticamente
- a cada iteração do schedular, o bot
  - pega a página
  - processa a página gerando uma mensagem ou não
  - caso tenha sido gerada uma mensagem, a envia pelo telegram
- o que pode ser modularizado?
    - a pagina (yaml)
    - as informações do bot (yaml)
    - o metodo que recebe o objeto do beautiful soup da pagina e retorna uma mensagem (ou não) (um arquivo python customizavel)