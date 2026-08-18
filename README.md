# Aulas · Elian Leite

Repositório de aulas e apresentações interativas. A página inicial (`index.html`) lista as **disciplinas** e permite abrir cada **aula**.

🔗 **Site (após publicar):** `https://SEU-USUARIO.github.io/aulas-elian-leite/`

## 📁 Estrutura

```
aulas-elian-leite/
├── index.html                      ← home: índice de disciplinas e aulas
├── .nojekyll                       ← evita processamento Jekyll no GitHub Pages
├── README.md
├── saberes-metodologia-lp/         ← uma pasta por disciplina
│   └── bncc-lingua-portuguesa/     ← uma pasta por aula
│       ├── index.html              ← a apresentação interativa
│       ├── Aula_BNCC_Lingua_Portuguesa.md
│       └── BNCC_LP_Anos_Iniciais.md
└── didatica/
    └── metodologias-ativas/
        └── index.html
```

Cada aula vive em sua própria pasta com um `index.html`, então o endereço fica limpo, por exemplo:
`https://SEU-USUARIO.github.io/aulas-elian-leite/saberes-metodologia-lp/bncc-lingua-portuguesa/`

## ➕ Como adicionar uma nova aula

1. Crie uma pasta dentro da disciplina (ex.: `saberes-metodologia-lp/nova-aula/`) e coloque nela o `index.html` da apresentação.
2. Abra o `index.html` da raiz e, no bloco `CURSOS` (dentro do `<script>`), adicione um item em `aulas`:

```js
{ n:"Aula 02", titulo:"Título da aula", desc:"Resumo curto.",
  badge:"2h · interativa", link:"saberes-metodologia-lp/nova-aula/" }
```

Para uma **nova disciplina**, adicione um novo objeto ao array `CURSOS` com seu próprio `icone`, `nivel` e lista de `aulas`.

## 🚀 Publicar no GitHub Pages

1. Crie um repositório **público** chamado `aulas-elian-leite`.
2. Envie todos os arquivos desta pasta (inclusive o `.nojekyll`, que é oculto).
3. Em **Settings → Pages**, escolha **Deploy from a branch**, branch **main**, pasta **/ (root)** e salve.
4. Aguarde 1–2 min e acesse o link gerado.

## 📝 Créditos

Material de apoio à docência. Fonte da aula de LP: BRASIL. MEC. **Base Nacional Comum Curricular (BNCC)**, 2018.
