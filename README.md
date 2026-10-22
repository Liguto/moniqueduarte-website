# 🌿 Monique | Massoterapia & Doulagem Hospitalar

Site institucional e landing page profissional desenvolvido para a **Monique**, unindo suas duas frentes de atuação com uma experiência acolhedora, sensível e focada em conversão:
1. **Massoterapia & Bem-Estar** ([@monique.massoterapia](https://instagram.com/monique.massoterapia))
2. **Doula & Acompanhante Hospitalar** ([@parto.commoni](https://instagram.com/parto.commoni))

Pronto para publicação gratuita e automática via **GitHub + Vercel**.

---

## ✨ Tecnologias Utilizadas

- **HTML5 Semântico:** Estrutura limpa, acessível e otimizada para motores de busca (SEO).
- **Tailwind CSS (CDN):** Estilização moderna e responsiva com paleta personalizada (tons terrosos, nude, bege, rosa queimado e verde oliva suave).
- **Google Fonts:**
  - *Cormorant Garamond:* Títulos elegantes, orgânicos e sofisticados.
  - *Plus Jakarta Sans:* Tipografia de corpo limpa, moderna e altamente legível.
- **Lucide Icons & SVGs inline:** Ícones leves e elegantes para cada técnica, benefício e redes sociais.
- **JavaScript Inline Vanilla:**
  - Menu hambúrguer mobile responsivo e acessível.
  - Scroll suave nos links de navegação com fechamento automático no mobile.
  - Accordion interativo de Perguntas Frequentes (FAQ) com transição suave.
  - Botão flutuante do WhatsApp com animação pulsante e tooltip.

---

## 🎨 Como Customizar os Dados da Monique

Antes de enviar para a Vercel ou após clonar, você pode abrir o arquivo `index.html` e substituir facilmente:

1. **Número de WhatsApp:**
   - Procure no arquivo por `55SEUNUMERO` e substitua pelo número real da Monique com DDD e código do país (ex: `5511999998888`).
   - Há mensagens personalizadas já configuradas para cada botão de ação (geral, massagem relaxante, drenagem, massagem para dores e acompanhamento de doula).

2. **Perfis do Instagram:**
   - Já estão pré-configurados com:
     - `https://instagram.com/monique.massoterapia`
     - `https://instagram.com/parto.commoni`

3. **Fotos da Monique:**
   - O site já vem com imagens profissionais e acolhedoras de alta qualidade do Unsplash.
   - Para colocar as fotos reais da Monique, basta salvar as fotos dela na mesma pasta (ex: `foto-monique.jpg`) e alterar o atributo `src=""` das tags `<img>` no `index.html`.

4. **Cidade / Região de Atendimento:**
   - No rodapé (`footer`), altere o texto *"Atendimento em consultório, domiciliar e hospitais/maternidades da região"* para especificar a cidade ou bairros atendidos.

---

## 🚀 Passo a Passo de Deploy (GitHub + Vercel)

### Parte 1: Enviar o código para o GitHub

#### 1. Criar o repositório no GitHub:
1. Acesse [github.com](https://github.com/) e faça login na sua conta.
2. No canto superior direito, clique no botão **`+`** e selecione **"New repository"** (Novo repositório).
3. Em **Repository name**, digite um nome (exemplo: `site-monique`).
4. Escolha **Public** (Público) ou **Private** (Privado) e deixe as outras opções desmarcadas (não adicione README nem .gitignore por lá).
5. Clique em **"Create repository"**.
6. Copie a URL do seu repositório (exemplo: `https://github.com/SEU-USUARIO/site-monique.git`).

#### 2. Comandos no Terminal (PowerShell / Git Bash / CMD):
Abra o terminal na pasta deste projeto (`C:\Users\Liguto\Documents\Site_Monique`) e execute os seguintes comandos:

```bash
# 1. Inicializa o repositório Git local
git init

# 2. Adiciona todos os arquivos ao controle de versão
git add .

# 3. Cria o primeiro commit com uma mensagem descritiva
git commit -m "feat: site profissional da Monique (Massoterapia e Doulagem)"

# 4. Define o branch principal como main
git branch -M main

# 5. Conecta seu repositório local ao repositório criado no GitHub
# (Substitua a URL abaixo pela URL que você copiou do seu GitHub)
git remote add origin https://github.com/SEU-USUARIO/site-monique.git

# 6. Envia os arquivos para o GitHub
git push -u origin main
```

---

### Parte 2: Publicar Gratuitamente na Vercel

1. Acesse [vercel.com](https://vercel.com/) e faça login (recomendado: clique em **"Continue with GitHub"** para conectar diretamente sua conta).
2. No painel principal (Dashboard), clique no botão **"Add New..."** > **"Project"**.
3. Na lista **"Import Git Repository"**, localize o repositório recém-criado (ex: `site-monique`) e clique em **"Import"**.
4. Nas configurações do projeto:
   - **Project Name:** Pode manter `site-monique` (ou personalizar o nome).
   - **Framework Preset:** Selecione **"Other"** (é um site HTML/JS estático puro).
   - **Root Directory:** `./` (deixe o padrão).
5. Clique no botão azul **"Deploy"**.
6. Em cerca de 10 a 20 segundos, a Vercel finalizará o processo e exibirá uma tela de parabéns com confetes! 🎉
7. O site já estará no ar com link público seguro HTTPS (exemplo: `https://site-monique.vercel.app`).

---

### 🔄 Atualizações Automáticas (CI/CD)

Sempre que você alterar qualquer detalhe no `index.html` e fizer:
```bash
git add .
git commit -m "atualizacao: ajustando numero de telefone"
git push
```
A **Vercel detecta a mudança instantaneamente** e atualiza o site no ar em poucos segundos, sem que você precise fazer nada manual.

---

### 🌐 Adicionar Domínio Personalizado (Opcional)

Se a Monique tiver ou comprar um domínio próprio (ex: `moniquecuidado.com.br` ou `moniquedoula.com.br`):
1. No painel do projeto na Vercel, vá em **Settings** > **Domains**.
2. Digite o domínio desejado e clique em **Add**.
3. A Vercel mostrará os apontamentos de DNS (Tipo `A` ou `CNAME`) para configurar onde o domínio foi comprado (Registro.br, Hostinger, GoDaddy, etc.).
4. A Vercel gera o certificado SSL (cadeado verde HTTPS) de forma 100% gratuita e automática!
