# Personal docker library used in dev env

```
  alias composer='docker run -it --rm -v `pwd`:/app -w /app composer/composer'
  alias node='docker run -it --rm -v `pwd`:/app -w /app node node'
  alias npm='docker run -it --rm -v `pwd`:/app -w /app node npm'
  alias php-cs-fixer='docker run -it --rm -v `pwd`:/app -w /app ludofleury/php-cs-fixer'
  alias phpspec='docker run -it --rm -v `pwd`:/app -w /app phpspec/phpspec'
```
