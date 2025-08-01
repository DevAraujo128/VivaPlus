# VivaPlus - Sistema de Gestão Farmacêutica

## 📋 Descrição

O **VivaPlus** é um sistema de gestão farmacêutica desenvolvido em Java com interface gráfica Swing. O sistema permite o gerenciamento de produtos farmacêuticos, controle de usuários com diferentes níveis de acesso e operações de catálogo de medicamentos.

## 🚀 Funcionalidades

### 👥 Gestão de Usuários
- **Sistema de Login**: Autenticação segura com CIP e senha
- **Múltiplos Níveis de Acesso**:
  - **ADMIN**: Acesso completo ao sistema
  - **MANAGER**: Gestão de produtos e relatórios
  - **EDITOR**: Edição de produtos
  - **BASIC**: Visualização básica

### 💊 Gestão de Produtos Farmacêuticos
- Cadastro de medicamentos com informações completas:
  - Nome do produto
  - Quantidade em estoque
  - Preço
  - Tipo de prescrição (Com prescrição / Sem prescrição)
  - Lote
  - Data de validade
  - Controle de modificações

### 📊 Catálogo de Produtos
- Visualização organizada de todos os produtos
- Filtros e busca por produtos
- Interface intuitiva para navegação

## 🛠️ Tecnologias Utilizadas

- **Java 21**: Linguagem principal
- **Swing**: Interface gráfica
- **MySQL**: Banco de dados
- **Maven**: Gerenciamento de dependências
- **FlatLaf**: Biblioteca para interface moderna
- **Cucumber**: Testes de comportamento (BDD)
- **JUnit**: Framework de testes unitários

## 📦 Dependências Principais

```xml
- MySQL Connector Java 8.0.33
- FlatLaf 3.1.1 (Interface moderna)
- Cucumber Java 7.14.0 (Testes BDD)
- JUnit 4.13.2 (Testes unitários)
- SVG Salamander 1.1.4 (Suporte a SVG)
```

## 🏗️ Estrutura do Projeto

```
VivaPlus/
├── src/
│   ├── main/java/org/vivaplus/
│   │   ├── database/
│   │   │   └── DatabaseConnection.java
│   │   ├── model/
│   │   │   ├── bean/
│   │   │   │   ├── Drug.java
│   │   │   │   └── User.java
│   │   │   ├── dao/
│   │   │   │   ├── DrugDAO.java
│   │   │   │   ├── LoginDAO.java
│   │   │   │   └── UserDAO.java
│   │   │   └── enums/
│   │   │       ├── Prescription.java
│   │   │       └── Roles.java
│   │   └── view/
│   │       ├── catalog/
│   │       ├── dashboard/
│   │       └── LoginScreen.java
│   └── test/
│       ├── java/
│       │   └── steps/
│       └── resources/
│           └── features/
└── pom.xml
```

## 🚀 Como Executar

### Pré-requisitos
- Java 21 ou superior
- Maven 3.6+
- MySQL 8.0+

### Instalação

1. **Clone o repositório**
   ```bash
   git clone [URL_DO_REPOSITORIO]
   cd VivaPlus
   ```

2. **Configure o banco de dados**
   - Crie um banco MySQL
   - Configure as credenciais em `DatabaseConnection.java`

3. **Compile o projeto**
   ```bash
   mvn clean compile
   ```

4. **Execute a aplicação**
   ```bash
   mvn exec:java -Dexec.mainClass="org.vivaplus.Main"
   ```

## 🧪 Testes

### Testes Unitários
```bash
mvn test
```

### Testes de Comportamento (BDD)
O projeto inclui testes Cucumber para cenários de:
- Login de usuários
- Registro de novos usuários
- Gestão de catálogo
- Atualização de produtos
- Mudança de roles

## 📱 Telas do Sistema

### Tela de Login
- Interface moderna com design FlatLaf
- Autenticação por CIP e senha
- Validação de credenciais

### Dashboard Administrativo
- Visão geral do sistema
- Controles de gestão
- Relatórios e estatísticas

### Catálogo de Produtos
- Listagem organizada de medicamentos
- Filtros e busca
- Interface responsiva

## 🔐 Segurança

- Autenticação baseada em roles
- Controle de acesso por nível de usuário
- Validação de dados de entrada
- Logs de modificações

## 📈 Funcionalidades Futuras

- [ ] Relatórios avançados
- [ ] Integração com sistemas externos
- [ ] Backup automático
- [ ] Notificações de produtos vencendo
- [ ] API REST para integração

## 🤝 Contribuição

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).

## 👨‍💻 Desenvolvedor

**João Rodrigues**

---

## 📞 Suporte

Para dúvidas ou suporte, entre em contato através dos canais disponibilizados no projeto.

---

*VivaPlus - Sistema de Gestão Farmacêutica* 🏥💊 