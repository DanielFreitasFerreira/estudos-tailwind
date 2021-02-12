<div style="text-align: center;">
  <img src="https://o.remove.bg/downloads/58da447f-0775-4ea9-b15c-52fe27e0e957/tailwind-css-logo-removebg-preview.png"/>
</div>

# Iniciando com Tailwind

Acesse o site oficial do tailwind css, para mais informações: 
[tailwindcss.com]('https://tailwindcss.com/')

## Por que Tailwind ?

- Foco em utility e não componentes.
- Pouco ou nenhum CSS para atingir resultados excelentes.
- Pouca sobreposição de CSS, ao contrário de frameworks.
- Foco em responsividade.
- Podemos criar componentes no tailwind.
- Facilidade em customização.

## Propósito do tailwindcss

- Diminuir o tempo que passamos codificando CSS.
- Permitir ampla liberdade entre os componentes que criamos.
- Facilidade em entender e customizar.
- Acoplagem em diversos ambientes, com ou sem framework front-end.
- Dificuldade zero para começar com mobile first.

## Instale o Tailwind via npm

- Precisamos instalar ele no projeto via npm.
- Para instalar tailwind, execute esse comando:  
```
npm install tailwindcss@latest postcss@latest autoprefixer@latest
```
O CSS do Tailwind requer Node.js 12.13.0 ou superior.

Na documentação eles recomenda instalar o tailwind como um plugin PostCSS.

Acesse o repositório Post CSS: [PostCSS / Autoprefixer]('https://github.com/postcss/autoprefixer')

Como o Tailwind não adiciona prefixos de fornecedor automaticamente ao CSS que ele gera, instale o autoprefixer para lidar com isso para você.

- Criando um arquivo CSS que vai conter as diretivas do tailwind.
- Precisamos buidar o arquivo baseado no arquivo de configurações criado, apontando para a saida que é o arquivo final de CSS. Acesse o repositório com o link acima.

## Crie seu arquivo de configuração

Se quiser personalizar a instalação do Tailwind, gere um arquivo de configuração para o seu projeto usando o utilitário Tailwind CLI incluído na instalação do tailwindcss pacote npm:

```
npx tailwindcss init
```
Isso criará um tailwind.config.jsarquivo mínimo na raiz do seu projeto:
```
module.exports = {
  purge: [],
  darkMode: false, // or 'media' or 'class'
  theme: {
    extend: {},
  },
  variants: {},
  plugins: [],
}
```
Se quizer saiber mais sobre como configurar o Tailwind acesse [documentação de configuração]("https://tailwindcss.com/docs/configuration")

## Incluir Tailwind em seu CSS

Crie um arquivo CSS se você não tiver um, e usar a @tailwinddirectiva para injetar de Tailwind base, components e utilities estilos:

```
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
```

## Instalação Tailwind Intellisense

- O intellisense é uma extensão excelente para o tailwind.
- Vai ajudar na criação dos projetos, auto completando as classes do framerwork.
- Em alguns casos mostra um preview do que utilizamos.

Para começar criar um projeto com tailwind, têm que ter o node instalado

[Clique para acessar o site do node]('https://nodejs.org/en/')

AS pelo site, recomendo que instale a versão LTS pelo NVM (Node Version Manager), pelo repositório oficial no github. Assim facilita a transição entre versões do node. E por padrão o node vêm com o npm instalado junto.

[Clique para acessar o github do NVM]('https://github.com/nvm-sh/nvm')

# Script para instalação e atualização

Para instalar ou atualizar o nvm, você deve executal o [script de instalação]('https://github.com/nvm-sh/nvm/blob/v0.37.2/install.sh'). Você pode baixar e executar o script manualmente ou usar o seguinte comando CURL ou WGET.

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
```
```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
```
Depois que instalou o script, execute npm install para baixar o nvm.
```
npm install nvm
```

# Verificar versão do nvm

Para verificar se o nvm foi instalado, execulte esse comando abaixo:
```
comando -v nvm
```

# Como usar

Para baixar, compilar e instalar a versão mais recente do node, faça o seguinte: 
```
nvm install node versão recente
```
Para instalar uma versão específica
```
nvm install aqui digite a versão do node -> 9.99.9
```
Ou digite no final (lts), ele vai buscar automáticamente a versão mais atual do node.
```
nvm install lts
```
