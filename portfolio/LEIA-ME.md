# Portfólio · Elian Leite

Página única (`index.html`), responsiva, com tema claro/escuro.
Endereço depois de publicada: `https://SEU-USUARIO.github.io/aulas-elian-leite/portfolio/`

## 1. Colocar os links das redes

Abra `index.html`, vá até o **final do arquivo**, no bloco marcado
`▼▼▼ 1) LINKS — EDITE APENAS ESTE BLOCO ▼▼▼` e cole as URLs:

```js
const LINKS = {
  linkedin : "https://www.linkedin.com/in/elian-santos-leite-41a936124/",
  lattes   : "http://lattes.cnpq.br/4053214001115674",
  instagram: "https://www.instagram.com/prof_elianleite",
  email    : "prof.eliansantos@gmail.com"   // e-mail do ícone no topo
};
```

> Link deixado como `""` faz o ícone correspondente sumir da página — nada quebra.

Os e-mails que aparecem na seção **Contato** ficam logo abaixo, na lista `EMAILS`
(o primeiro é o principal). Para incluir mais um, basta acrescentar uma linha:

```js
const EMAILS = [
  { rotulo:"Profissional", end:"prof.eliansantos@gmail.com" },
  { rotulo:"Institucional · NEES/UFAL", end:"elian.santos@nees.ufal.br" }
];
```

## 2. Colocar as imagens

Salve os arquivos dentro da pasta `img/` com **exatamente** estes nomes:

| Arquivo | Onde aparece | Observação |
|---|---|---|
| `img/perfil.jpg` | foto de perfil no topo | quadrada (o corte circular é feito pelo CSS) |
| `img/galeria-1.jpg` … `galeria-5.jpg` | mosaico da galeria | qualquer proporção — a página respeita a original |

**Como as imagens atuais foram preparadas.** Os arquivos originais estão guardados em
`img/originais/`. As versões usadas na página são recortes/reduções otimizadas
(lado maior ≤ 1400 px), para o site carregar rápido:

- `perfil.jpg` — quadrado 900×900, rosto e ombros. Também existe
  `perfil-vertical.jpg` (retrato 900×1200, corpo até os joelhos) como alternativa,
  caso queira trocar o círculo do topo por um retângulo.
- `galeria-1..5.jpg` — reduzidas a partir dos originais, ~100–250 KB cada.

Para **acrescentar** uma foto: salve o arquivo em `img/` e adicione uma linha no
array `GALERIA` (ver item 3). Não é preciso recortar — o mosaico aceita retrato,
quadrado e paisagem juntos, e a foto abre em tela cheia ao ser clicada
(setas ← → e Esc funcionam).

Enquanto o arquivo não existe, a página mostra um quadro tracejado com o nome esperado —
é só substituir. Para trocar as legendas (ou mudar a quantidade de fotos), edite o array
`GALERIA` no final do `index.html`.

## 3. Editar os textos

Tudo que muda com frequência está em arrays no final do `index.html`:

- `FORMACAO` — linha do tempo da formação acadêmica
- `EXPERIENCIA` — cards de experiência profissional (ícone, cargo, instituição, período, bullets e tags)
- `GALERIA` — fotos e legendas (a ordem da lista é a ordem no mosaico)

Os textos de apresentação (hero, "Sobre", "Contato") ficam no HTML, cada um dentro de um
bloco comentado com o nome da seção.

## 4. Publicar

A pasta já está dentro do repositório `aulas-elian-leite`. Basta commitar e enviar:

```bash
git add portfolio
git commit -m "Adiciona página de portfólio"
git push
```
