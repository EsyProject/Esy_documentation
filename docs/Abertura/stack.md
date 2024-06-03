import { FaReact } from "react-icons/fa";
import { SiVite, SiNpm } from "react-icons/si";
import { FaCss3Alt } from "react-icons/fa";
import { BiLogoSpringBoot, BiLogoPostgresql } from "react-icons/bi";
import { IoLogoDocker } from "react-icons/io5";
import {SiMicrosoftazure} from "react-icons/si";
import { SiDbeaver } from "react-icons/si";
import { FaGitAlt } from "react-icons/fa";
import { SiInsomnia } from "react-icons/si";
import { SiDocusaurus } from "react-icons/si";


# Desenvolvimento

## Tecnologias Utilizadas 🧰:

### Documentação:
- [Docusaurus](https://docusaurus.io/) <SiDocusaurus />: Usamos o Docusaurus para realizar a documentação do Bosch Esy.

### Frontend:
- [React](https://react.dev/)  <FaReact/>: React é uma biblioteca JavaScript para criar interfaces de usuário interativas e dinâmicas. Com React, podemos dividir a interface do usuário do projeto Bosch Esy em componentes reutilizáveis, facilitando o desenvolvimento de um aplicativo web moderno e escalável.
- [Vite](https://vitejs.dev/) <SiVite/>: Vite é uma ferramenta de construção rápida para aplicativos web modernos. Com Vite, podemos iniciar rapidamente o projeto Bosch Esy, aproveitando a compilação instantânea e o recarregamento a quente para um desenvolvimento eficiente e ágil.
- [CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS) <FaCss3Alt />: CSS (Cascading Style Sheets) é uma linguagem de estilo usada para estilizar documentos HTML. Com CSS, podemos adicionar estilos de design ao projeto Bosch Esy, incluindo cores, fontes e layout, para criar uma aparência visual atraente e coesa.
- [NPM](https://www.npmjs.com/) <SiNpm />: NPM (Node Package Manager) é um gerenciador de pacotes para o ecossistema JavaScript. Com o NPM, podemos instalar e gerenciar dependências de projetos no Bosch Esy, facilitando a integração de bibliotecas e ferramentas externas necessárias para o desenvolvimento e a execução do projeto.

### Backend
- [Spring Boot](https://spring.io/projects/spring-boot) <BiLogoSpringBoot />: Spring Boot é um framework Java que simplifica o desenvolvimento de aplicativos web. Com o Spring Boot, podemos criar rapidamente aplicativos Java robustos e escaláveis para o backend do projeto EsyBosch, aproveitando suas convenções e configurações predefinidas. Usamos o Spring Boot para realizar uma API Restful, ou seja, backend do Bosch Esy.
- [PostGreSQL](https://www.postgresql.org/) <BiLogoPostgresql />: PostgreSQL é um sistema de gerenciamento de banco de dados relacional de código aberto. Com o PostgreSQL, podemos armazenar e gerenciar os dados do projeto Bosch Esy de forma confiável e eficiente, garantindo integridade e consistência dos dados.
- [DBeaver](https://dbeaver.io/download/) <SiDbeaver />: DBeaver é uma ferramenta gratuita para gerenciamento de bancos de dados. Com o DBeaver, podemos interagir com o banco de dados PostgreSQL usado no projeto Bosch Esy. Ele facilita a visualização, edição e execução de consultas SQL, ajudando no desenvolvimento e manutenção do banco de dados do projeto.
- [Insomnia](https://insomnia.rest/download) <SiInsomnia />: Utilizamos o Insmonia como cliente para realizar os devidos testes na API do Bosch Esy, podendo acessar (com o token JWT da azure) todos os [endopoints](https://github.com/EsyProject/Esy_backend/blob/fix_dev/endpoints.json) criados com Spring Boot.
- [Docker](https://www.docker.com/) <IoLogoDocker />: Docker é uma plataforma de contêinerização que simplifica o processo de desenvolvimento, implantação e execução de aplicativos. Com o Docker, podemos criar contêineres isolados para o projeto Bosch Esy, garantindo consistência e portabilidade entre diferentes ambientes de desenvolvimento e produção. Usamos no Bosch Esy para facilitar o desenvolvimento, rodando TUDO em contâiner.
- [Azure](https://azure.microsoft.com/pt-br/) <SiMicrosoftazure />:
Azure é uma plataforma de computação em nuvem fornecida pela Microsoft. Com o Azure, podemos hospedar e implantar o projeto Bosch Esy na nuvem de forma escalável e segura, aproveitando os serviços e recursos oferecidos pela plataforma para garantir alta disponibilidade e desempenho do aplicativo. Usamos o SSO (Single Sign-On) para entrar no nosso aplicativo (sistema padrão Bosch).

## Desenvolvimento 💻:

#### Componentes Reutilizáveis (Bosch Esy):

##### Sidebar
- Facilita a navegação do usuário dentro do sistema.
- Componentizada para ser usada em várias páginas, garantindo consistência de navegação.

##### Input
- Componente versátil para entrada de dados em formulários.
- Flexível e reutilizável em diferentes contextos, promovendo consistência e usabilidade.

##### Navbar
- Barra de navegação superior do sistema.
- Componentizada para oferecer uma experiência de navegação coesa e intuitiva em todo o aplicativo.

### Implementação de Autenticação:

#### Frontend
- Desenvolvimento das telas de login e cadastro utilizando React e Vite.
- Integração fluida com a API fornecida pelo backend para autenticação e registro de usuários.

#### Backend
- Implementação robusta das rotas e lógica de autenticação utilizando Spring Boot.
- Criação de endpoints seguros usando o SSO (Bosch) para lidar com solicitações de login e cadastro de usuários de forma eficiente e segura. Com todos os endpoints autenticados com o JWT do SSO da Bosch.

## Estruturação do Projeto:

### Frontend
- Organização do código-fonte em componentes reutilizáveis, páginas e serviços, promovendo a manutenibilidade e a escalabilidade do frontend.

### Backend
- Estruturação consistente seguindo os padrões de projeto do Spring Boot, com classes de controle, serviços e modelos, garantindo a coesão e a clareza do código.

## Fluxo de Trabalho:

### GitFlow <FaGitAlt />
- Utilização do fluxo de trabalho GitFlow para gerenciar as branches do projeto, facilitando o desenvolvimento colaborativo e a integração contínua. [Bosch ESY!](https://github.com/orgs/EsyProject/repositories)

## Ambiente de Desenvolvimento:

### Ferramentas e Integração:
- Utilização do ambiente de desenvolvimento rápido Vite para o frontend, e do Spring Boot para o backend, garantindo eficiência e robustez no desenvolvimento de APIs.
- Integração eficaz entre as partes frontend e backend do projeto para proporcionar uma experiência de usuário contínua e eficaz.
