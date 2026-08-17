# 🍽️ Sistema de Gerenciamento e Reservas para Restaurantes

Um sistema Full Stack completo, responsivo e modular desenvolvido para a automação de serviços, gerenciamento de cardápios, reservas de mesas e administração interna de um estabelecimento gastronômico.

⚡ **Link do Projeto (Demonstração):** [Acesse o Deploy](https://vercel.app)

---

## 🛠️ Engenharia e Arquitetura do Sistema

O projeto foi estruturado seguindo boas práticas de separação de conceitos (Separation of Concerns), integrando uma interface rica para o usuário final a um painel de controle administrativo seguro.

### 1. Camada de Persistência e Modelagem de Dados (`MySQL`)
A arquitetura de dados utiliza o modelo relacional para garantir a integridade referencial das informações do restaurante.
* **Mapeamento de Entidades:** O arquivo estrutural `mysql.sql` gerencia tabelas cruciais como usuários, agendamentos de reservas, itens do cardápio e mensagens de contato.
* **Segurança e Consistência:** Modelagem focada em chaves primárias e estrangeiras para evitar concorrência ou duplicidade no agendamento de mesas.

### 2. Painel Administrativo (`/admin`)
O sistema conta com um módulo exclusivo de administração isolado da interface pública do cliente.
* **Controle Operacional:** Permite aos administradores gerenciar o fluxo de reservas ativas, atualizar os itens e preços do menu (`menu.html`) e auditar dados sem a necessidade de interagir diretamente com o banco de dados.

### 3. Experiência do Usuário e Otimização Visual
* **Acessibilidade e SEO:** Páginas estruturadas de forma estritamente semântica (`services.html`, `contact.html`, `reservation.html`) com metadados otimizados para mecanismos de busca.
* **Estilização Modular:** Folhas de estilo segregadas e otimizadas para garantir responsividade fluida em smartphones, tablets e desktops, mantendo uma identidade visual sofisticada e de alto contraste.

---

## 🚀 Tecnologias Utilizadas

* **Frontend:** HTML5 Semântico, CSS3 Moderno, JavaScript Avançado (manipulação do DOM e validação de requisições de formulários).
* **Backend & Infraestrutura:** Estrutura de scripts para integração de rotas e processamento de regras de negócio.
* **Banco de Dados:** MySQL (Modelagem relacional e scripts estruturais).
* **Fontes & Ícones:** Google Fonts e pacotes de ícones otimizados para web.

---

## 📁 Estrutura de Diretórios Principal

* `/admin`: Páginas e controle do painel de administração interna.
* `/css`: Arquivos de estilo e arquitetura visual estruturada.
* `/db`: Configurações de conexão e persistência de dados.
* `mysql.sql`: Script de criação e inicialização do banco de dados relacional.
* `reservation.html`: Módulo de captura e processamento de reservas de clientes.

---

## 🧠 Como Executar o Projeto Localmente

1. Clone o repositório em sua máquina:
   ```bash
   git clone [https://github.com](https://github.com/leo-gomes-dev/restaurante-leogom.git)
   ```
2. **Configuração do Banco de Dados:**
   * Importe o arquivo `mysql.sql` no seu gerenciador MySQL local (como phpMyAdmin, MySQL Workbench ou Docker).
3. Execute o arquivo `index.html` utilizando a extensão **Live Server** do VS Code ou seu servidor local de preferência (XAMPP/WampServer).

---

Desenvolvido com foco em escalabilidade e regras de negócio reais por **Leo Gomes** 🚀
