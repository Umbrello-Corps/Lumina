# Lumina — Plataforma de Apoio à Pesquisa Científica Feminina

O **Lumina** é um ecossistema digital desenvolvido com o propósito claro de visibilizar, valorizar e financiar a produção científica feita por mulheres no Brasil. A plataforma atua como um repositório científico de acesso aberto e uma rede de financiamento coletivo (crowdfunding), permitindo que a sociedade civil apoie diretamente projetos de pesquisa liderados por mulheres por meio de doações transparentes e acompanhamento de metas estruturadas.

Este repositório contém toda a implementação **Frontend** da plataforma, totalmente otimizada para execução estática e pronta para implantação contínua no Vercel.

---

## Sobre a Umbrello Corps

A **Umbrello Corps** é uma organização de desenvolvimento de software e soluções tecnológicas focada no design de sistemas de alto impacto social, usabilidade refinada e forte fundamentação em Engenharia de Software. Guiada por processos iterativos e metodologias ágeis, a organização busca transformar requisitos complexos em interfaces fluidas, acessíveis e seguras, promovendo soluções inovadoras que conectam comunidades e democratizam o acesso à informação e aos recursos.

---

## Funcionalidades & Casos de Uso Cobertos

O sistema foi inteiramente projetado seguindo a especificação dos Casos de Uso da plataforma, abrangendo os seguintes fluxos:

1. **Repositório Científico Dinâmico:** Feed de buscas avançadas com filtros por área de conhecimento, instituição e status da pesquisa.
2. **Visualização de Artigos Completa:** Exibição do resumo científico, visualizador integrado e acompanhamento em barras de progresso das metas financeiras atreladas.
3. **Mecanismo de Apoio Direto:** Sistema integrado de simulação de doações (via Pix/PayPal) com direcionamento automático para telas de confirmação de sucesso.
4. **Comunidade Acadêmica & Debates:** Seção de comentários em tempo real sob os artigos e ferramentas de moderação (denúncia de abusos).
5. **Login Inteligente (Coringa):** Fluxo dinâmico via `localStorage` que simula um backend real. O nome inserido no login ou cadastro é memorizado e exibido de forma personalizada por todo o cabeçalho e painel do sistema.
6. **Moderação Administrativa:** Painel restrito para que administradores auditem usuários e aprovem ou rejeitem novas submissões de artigos acadêmicos.

---

## Estrutura de Arquivos do Projeto

Para garantir máxima performance, portabilidade e compatibilidade com o roteamento estático do Vercel, todos os estilos (CSS) e interações dinâmicas (JavaScript/DOM) foram embutidos de maneira limpa dentro de cada arquivo `.html` correspondente:

* `index.html` - Página inicial institucional (Landing Page) contendo o banner de conformidade com a LGPD.
* `cadastro.html` - Fluxo de criação de conta com diferenciação dinâmica entre os perfis de Leitora e Pesquisadora (exigência de Currículo Lattes).
* `login.html` - Tela de acesso à plataforma integrada ao sistema de memória do perfil coringa e atalho de acesso ao Admin.
* `pesquisa.html` - Painel geral de exploração de artigos científicos com suporte a filtros ativos.
* `artigo.html` - Página de leitura detalhada do trabalho científico, metas do projeto e módulo de debates técnicos.
* `doacao-sucesso.html` - Tela de confirmação e agradecimento após a conclusão simulada do Pix de apoio.
* `painel.html` - Dashboard privado da pesquisadora, exibindo métricas financeiras acumuladas e lista de artigos próprios.
* `perfil.html` - Página de perfil público da pesquisadora com bio e listagem de trabalhos validados.
* `painel-admin.html` - Painel restrito do administrador para gerenciamento e moderação de submissões pendentes.
* `recuperar-senha.html` - Solicitação de link de redefinição de credenciais via e-mail acadêmico.
* `nova-senha.html` - Tela de inserção e confirmação da nova senha de usuário.
* `quem-somos.html` - Página descritiva detalhando a missão, valores e o propósito do Lumina.
* `contato.html` - Central de atendimento com e-mail corporativo fictício e formulário de contato.

---

## Como Executar o Projeto

Como o projeto é composto estritamente de arquivos frontend estáticos bem estruturados, ele não necessita de instaladores de pacotes (`npm` ou `yarn`) ou servidores pesados.

### Localmente
1. Faça o clone deste repositório ou baixe a pasta com os arquivos.
2. Certifique-se de manter todos os 13 arquivos `.html` na **raiz** da mesma pasta.
3. Abra o arquivo `index.html` diretamente em qualquer navegador moderno ou utilize a extensão **Live Server** no VS Code para uma experiência em tempo real.

### Implantação no Vercel
Este repositório está configurado para publicação imediata no **Vercel**:
1. Conecte sua conta do GitHub ao painel do Vercel.
2. Selecione este repositório para importação.
3. Mantenha as configurações padrão (o Vercel detectará automaticamente o arquivo `index.html` como a página principal).
4. Clique em **Deploy** e o seu link estático `.vercel.app` estará online em segundos!

---

## Tecnologias Utilizadas

* **HTML5:** Estruturação semântica de todas as páginas e modais.
* **CSS3:** Estilização moderna baseada em Design Tokens (variáveis), grids responsivos e tipografia elegante tirada diretamente do manual de identidade visual.
* **JavaScript (Vanilla):** Manipulação de DOM para gerenciamento de modais, alternância de abas de perfil e uso do `localStorage` para a simulação persistente da sessão do usuário.
* **SVG:** Ícones nativos vetorizados em alta resolução e Favicon embutido via Data URI para otimização de requisições.

---

© 2026 Umbrello Corps. Desenvolvido para fins acadêmicos e de impacto científico social.
