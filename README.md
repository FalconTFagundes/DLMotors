# DL Motors — Estética Automotiva & Personalização de Motos

Website institucional responsivo para a **DL Motors**, com páginas de **Início**, **Serviços** e **Contato**, integração com **WhatsApp** e uso de bibliotecas front‑end populares (AOS, Bootstrap Icons, Font Awesome, GLightbox, PureCounter e Swiper).

> **Stack:** HTML5, CSS3, JavaScript, Google Fonts, Bootstrap Icons (sem build, sem dependências de Node).

---

## 📂 Estrutura do projeto

```
DLMOTORS/
├── assets/
│   ├── img/                # Imagens do site
│   ├── js/                 # Scripts específicos do projeto
│   └── scss/               # (Opcional) Estilos em SCSS/SASS, se utilizados
├── vendor/                 # Bibliotecas de terceiros
│   ├── aos/                # Animações ao rolar
│   ├── bootstrap/          # Bootstrap (CSS/JS)
│   ├── bootstrap-icons/    # Ícones do Bootstrap
│   ├── fontawesome-free/   # Ícones Font Awesome
│   ├── glightbox/          # Lightbox/Galeria
│   ├── php-email-form/     # Validação/cliente para formulário (requer backend)
│   ├── purecounter/        # Contadores animados
│   └── swiper/             # Carrosséis/Sliders
├── contact.html            # Página de Contato
├── index.html              # Página Inicial
├── services.html           # Página de Serviços
└── README.md               # Este arquivo
```

> **Observação:** alguns *vendors* podem estar presentes para futuras features. O projeto funciona como site estático (sem compilação).

---

## ✨ Funcionalidades

- **Hero** com chamada para ação e destaque da marca.
- **Serviços por tipo de veículo** (Carro/Moto) com cartões, texto e faixas de preço.
- **Abas de imagem** (Exemplo | Antes | Depois) nos cards de serviço.
- **Botões flutuantes e CTAs de WhatsApp** para contato rápido.
- **Menu responsivo** com *toggle* no mobile.
- Otimizações visuais: animações, sombras, gradientes e tipografia com **Poppins/Roboto**.

---

## 🚀 Como executar localmente

1. **Clone** o repositório:
   ```bash
   git clone https://github.com/<seu-usuario>/<seu-repo>.git
   cd <seu-repo>
   ```

2. **Abra** o `index.html` diretamente no navegador **ou** use um servidor estático (recomendado):
   - VS Code + extensão **Live Server** (clique em *Go Live*).
   - Ou via Python:
     ```bash
     # Python 3
     python -m http.server 5500
     # depois acesse: http://localhost:5500
     ```

> Não há dependências de Node ou build. É só abrir e usar.

---

## 🛠️ Customização rápida

### 1) WhatsApp (número e mensagem)
- Procure nos arquivos por `wa.me/` e ajuste o número/mensagem, por exemplo:
  ```html
  https://wa.me/5527998810245?text=Olá! Gostaria de conhecer os serviços da DL Motors.
  ```

### 2) Imagens
- Coloque seus arquivos em `assets/img/` e atualize os `src=""` das `<img>` conforme necessário.

### 3) Ícones
- O projeto usa **Bootstrap Icons** e **Font Awesome** (pasta `vendor/`). Exemplos de classe:
  ```html
  <i class="bi bi-whatsapp"></i>
  <i class="fa-solid fa-car"></i>
  ```

### 4) Formulário de contato
- O diretório `vendor/php-email-form/` fornece validação no cliente, **mas o envio real requer backend**.
- Opções:
  - **PHP** (hospedagem com PHP): aponte a `action` do formulário para um script que envia e-mail.
  - **Serviços externos** (ex.: Formspree, Getform): substitua a `action` pelo endpoint do serviço.
- Se a hospedagem for **GitHub Pages**, não há PHP — use um serviço externo de formulários.

### 5) SEO básico
- Ajuste `<title>`, `meta name="description"` e `meta name="keywords"` em cada página.
- Adicione um `favicon` em `assets/img/` e referencie com:
  ```html
  <link rel="icon" href="assets/img/icon.ico">
  ```

---

## 🌐 Publicação no GitHub Pages

1. **Commit & push** para a branch `main` (ou `master`).
2. No GitHub, vá em **Settings › Pages**.
3. Em **Build and deployment**, escolha **Source: Deploy from a branch**.
4. Selecione a branch (ex.: `main`) e o diretório `/root`.
5. Salve. O link será algo como:  
   `https://<seu-usuario>.github.io/<seu-repo>/`

> Se suas páginas estiverem dentro de uma pasta, lembre-se de ajustar os **paths relativos** (`href`, `src`) conforme a raiz do Pages.

---

## 📦 Bibliotecas de terceiros

- **AOS** (animações ao rolar)
- **Bootstrap** e **Bootstrap Icons**
- **Font Awesome Free**
- **GLightbox**
- **PureCounter**
- **Swiper**
- **php-email-form** (validação no front; envio requer backend)

Cada biblioteca mantém **sua própria licença**. Verifique os arquivos dentro de `vendor/` para detalhes.

---

## 🧩 Roadmap (ideias)

- Trocar imagens de exemplo por portfólio real (antes/depois).
- Ativar GLightbox nas galerias.
- Carrosséis de depoimentos com Swiper.
- Integração real do formulário de contato (endpoint).
- Minificação/organização de CSS/JS em `assets/`.

---

## 👤 Autor

Projeto desenvolvido por **Rafael Fagundes**.  
Contato rápido: [WhatsApp](https://wa.me/5533991414767)

---

## 📝 Licença

Defina a licença que preferir para o **código do projeto** (ex.: MIT).  
As **bibliotecas em `vendor/`** seguem as licenças de seus respectivos autores.
