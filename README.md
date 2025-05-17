Este repositório foi criado como parte do desafio da DIO (Digital Innovation One), com o objetivo de documentar o processo de configuração de uma instância de banco de dados na plataforma Microsoft Azure. Aqui você encontrará resumos, anotações e dicas práticas que servirão como material de apoio para estudos e futuras implementações.

---

## 🎯 Objetivos do Desafio

- Praticar a criação e configuração de uma instância de banco de dados na Azure.
- Aplicar os conceitos aprendidos durante as aulas teóricas.
- Registrar todo o processo técnico em um repositório público no GitHub.
- Explorar os modelos de serviço (IaaS, PaaS e SaaS) e o modelo de responsabilidade compartilhada.

---

## 🧠 Conceitos Fundamentais

### ☁️ Modelos de Serviço: IaaS, PaaS e SaaS na Azure

| Modelo | Definição | Exemplo na Azure | Responsabilidade |
|--------|-----------|------------------|------------------|
| **IaaS (Infrastructure as a Service)** | Fornece infraestrutura básica (servidores, redes, armazenamento). | Azure Virtual Machines | Alta responsabilidade do usuário (configurar SO, banco, segurança etc.) |
| **PaaS (Platform as a Service)** | Oferece uma plataforma gerenciada para desenvolver e hospedar aplicações. | Azure SQL Database, Azure App Service | Responsabilidade intermediária (usuário foca na aplicação e dados) |
| **SaaS (Software as a Service)** | Serviço completo pronto para uso pelo cliente. | Microsoft 365, Dynamics 365 | Pouca ou nenhuma responsabilidade do usuário (apenas uso do serviço) |

Na configuração de banco de dados, o uso do **Azure SQL Database (PaaS)** é altamente recomendado, pois a Microsoft cuida da manutenção, backups, escalabilidade e segurança da instância.

---

### 🔐 Modelo de Responsabilidade Compartilhada

Na nuvem, a **segurança e a operação dos recursos são divididas** entre o provedor (Microsoft Azure) e o cliente (você):

- **Azure é responsável** pela segurança física dos datacenters, infraestrutura, rede e serviços básicos da plataforma.
- **Você é responsável** pela configuração correta dos seus recursos, gerenciamento de acesso, criptografia dos dados e boas práticas de segurança (como senhas fortes e firewalls).

> ⚠️ Exemplo: se você configurar mal as regras de firewall do seu banco de dados, ele poderá ficar vulnerável — mesmo que a infraestrutura da Azure seja segura.


---

## 💡 Dicas e Boas Práticas

- **Habilite o firewall corretamente** para evitar conexões não autorizadas.
- Utilize **autenticação com Active Directory** para maior controle de usuários.
- Configure **backup automático e alta disponibilidade**, se possível.
- Sempre **use variáveis de ambiente** para senhas e conexões no código.




