# JF Construções — Site de Portfólio

Site de portfólio profissional para marceneiro e pedreiro, hospedado via GitHub Pages.

## Tecnologias

- HTML5, CSS3 e JavaScript puro (sem frameworks)
- Google Fonts (Playfair Display + Inter)
- Totalmente responsivo (mobile, tablet e desktop)

## Estrutura

```
├── index.html   # Página principal
├── style.css    # Estilos
└── main.js      # Animações e interatividade
```

## Funcionalidades

- Animações de scroll (Intersection Observer)
- Contador animado de estatísticas
- Filtro de portfólio por categoria
- Formulário que abre conversa no WhatsApp com os dados preenchidos
- Menu mobile com hamburguer
- Navbar que muda ao fazer scroll

## Como publicar no GitHub Pages

1. Crie um repositório no GitHub (pode ser público)
2. Faça o upload dos arquivos ou use git:

```bash
git init
git add .
git commit -m "primeiro commit"
git branch -M main
git remote add origin https://github.com/seu-usuario/seu-repositorio.git
git push -u origin main
```

3. No repositório, vá em **Settings → Pages**
4. Em **Source**, selecione a branch `main` e clique em **Save**
5. Aguarde alguns segundos — o site estará disponível em `https://seu-usuario.github.io/seu-repositorio`

## Personalização

### Dados do cliente
Edite `index.html` e substitua:
- `João Ferreira` → nome real do cliente
- `JF Construções` → nome da empresa
- `(11) 99999-9999` → telefone real
- `joao@jfconstrucoes.com.br` → e-mail real
- `Grande São Paulo` → região de atendimento

### Número do WhatsApp
Em `main.js` (linha 99) e em `index.html` (botão "Chamar no WhatsApp"), troque o número:
```
wa.me/5511988582495
```
O formato é: `55` (Brasil) + DDD + número, sem espaços ou traços.

### Fotos do portfólio
Nos cards de portfólio em `index.html`, substitua os blocos `<div class="img-placeholder">` por:
```html
<img src="fotos/nome-da-foto.jpg" alt="Descrição do trabalho" />
```

### Estatísticas do Hero
Em `index.html`, ajuste os valores `data-target` conforme a realidade do cliente:
```html
<span class="stat-num" data-target="350">0</span>
```
