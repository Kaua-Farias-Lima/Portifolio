# Portfólio | Kauã Farias de Lima

Portfólio pessoal de **Kauã Farias de Lima**, estudante de Engenharia de Software e técnico em informática, com experiência em suporte técnico N1 / Service Desk e desenvolvimento web.

![Prévia do portfólio](docs/preview.png)

## O que tem no site

- **Sobre mim** e destaque da **experiência** profissional (Digisystem, Suporte Técnico N1 / Service Desk)
- **Habilidades** técnicas e de ambiente corporativo
- **Projeto** Cosmetic Store (TCC)
- **Formação** acadêmica
- **Certificados** organizados por área, com visualizador ampliado e navegação por setas ou teclado
- **Contato** por e-mail, WhatsApp, LinkedIn e GitHub, além de botão para baixar o currículo em PDF

## Tecnologias

HTML5, CSS3 e um pouco de JavaScript puro. Não usa framework, build nem dependências: as fontes (Inter) ficam dentro do próprio projeto, então o site funciona offline.

## Estrutura

```text
.
├── index.html                 # conteúdo da página
├── style.css                  # visual e responsividade
├── README.md
├── docs/
│   └── preview.png            # imagem usada neste README
└── assets/
    ├── foto-kaua.jpg          # foto da abertura (proporção 4:5)
    ├── icon.png               # ícone da aba do navegador
    ├── curriculo-kaua-farias.pdf
    ├── fonts/                 # fontes Inter
    └── certificados/          # imagens dos certificados
```

## Como ver no seu computador

Basta abrir o `index.html` com um clique duplo. Se preferir um servidor local:

```bash
python3 -m http.server 8000
```

Depois acesse `http://localhost:8000`.

## Como publicar no GitHub (GitHub Pages)

### Opção A: substituir o portfólio que já está no seu repositório

1. Clone o repositório atual (troque `SEU-USUARIO` pelo seu usuário do GitHub):

   ```bash
   git clone https://github.com/SEU-USUARIO/Portifolio.git
   cd Portifolio
   ```

2. Apague os arquivos antigos (`index.html`, `style.css`, `avatar.png`, `banner.jpg`, `icon.png`, `certifiado.PNG`) e copie para dentro da pasta **todo o conteúdo** da pasta `Portifolio` deste zip, incluindo `assets/` e `docs/`.

3. Envie as mudanças:

   ```bash
   git add -A
   git commit -m "Reformula portfólio com novo design, certificados e currículo"
   git push origin main
   ```

   Se o seu repositório usa outro nome de branch (por exemplo `master`), troque `main` por ele.

### Opção B: criar um repositório novo

1. No GitHub, clique em **New repository** e dê um nome (por exemplo `Portifolio`). Deixe como **Public**.
2. Na pasta do projeto, rode:

   ```bash
   git init
   git add -A
   git commit -m "Primeira versão do portfólio"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/Portifolio.git
   git push -u origin main
   ```

### Ativar o GitHub Pages

1. No repositório, abra **Settings** e depois **Pages**.
2. Em **Build and deployment**, escolha **Deploy from a branch**.
3. Selecione a branch `main` e a pasta `/ (root)`, e clique em **Save**.
4. Em 1 a 2 minutos o site aparece em:
   - `https://SEU-USUARIO.github.io/Portifolio/`

   Se você nomear o repositório como `SEU-USUARIO.github.io`, o endereço fica só `https://SEU-USUARIO.github.io/`.

Depois de publicar, coloque o link do site na descrição do repositório (ícone de engrenagem ao lado de **About**) e no seu LinkedIn.

## Como personalizar

- **Textos:** edite o `index.html`. Cada seção tem um comentário (`<!-- Sobre -->`, `<!-- Experiência -->` etc.).
- **Cores:** estão no começo do `style.css`, no bloco `:root` (`--tinta`, `--papel`, `--cabo`, `--led`).
- **Foto:** troque `assets/foto-kaua.jpg`. Use proporção 4:5, de preferência com 640 × 800 px ou mais.
- **Currículo:** substitua `assets/curriculo-kaua-farias.pdf` mantendo o mesmo nome.
- **Novo certificado:**
  1. Salve a imagem em `assets/certificados/` como `nome.jpg` (cerca de 1400 px de largura) e uma miniatura `nome-mini.jpg` (640 px de largura).
  2. Na seção `<!-- Certificados -->` do `index.html`, copie um bloco `<li>...</li>` dentro do grupo certo e troque o nome do arquivo, o título e os textos.
  3. O visualizador reconhece o novo item sozinho.
- **Novo projeto:** na seção `<!-- Projetos -->`, copie o bloco `<article class="projeto">` e edite.

## Cuidados antes de publicar

- Em certificados e documentos, cubra dados pessoais como RG, CPF e data de nascimento (o certificado da ETB já está com esses trechos tapados).
- O telefone e o e-mail do site são públicos. Remova os que você não quiser expor na seção de contato.

## Contato

- E-mail: kaualima10cp@gmail.com
- LinkedIn: [linkedin.com/in/kauã-farias-253435196](https://www.linkedin.com/in/kau%C3%A3-farias-253435196)
- GitHub: [github.com/Kaua-Farias-Lima](https://github.com/Kaua-Farias-Lima)
