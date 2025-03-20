# 🛒 Fake Shop

## 📌 Sobre o Projeto
Fake Shop é uma aplicação web desenvolvida para simular uma loja virtual.  
O projeto foi criado para fins de estudo e demonstração de conceitos de desenvolvimento e implantação de aplicações em ambiente containerizado usando Kubernetes.

## 🛠 Tecnologias Utilizadas
- 🐍 **Python 3.12** - Linguagem de programação principal
- 🌐 **Flask** - Framework para criação da API Web
- 🔥 **Gunicorn** - Servidor WSGI para execução da aplicação Flask
- 🐳 **Docker** - Para containerização da aplicação
- ☸ **Kubernetes** - Para orquestração dos containers
- 🐘 **PostgreSQL** - Banco de dados relacional
- ---  


## 📂 Estrutura do Projeto
```
/fake-shop
│── k8s/                      # Arquivos de configuração do Kubernetes
│   ├── deployment.yaml       # Configuração do Deployment e Services
│── src/                      # Código fonte da aplicação
│   ├── migrations/           # Arquivo principal da API Flask
│   ├── models/               # Modelos do banco de dados
|   ├── static/               # Arquivos de layout web
│   ├── templates/            # Arquivos HTML da aplicação WEB
│── requirements.txt          # Dependências do projeto
│── Dockerfile                # Arquivo para criação da imagem Docker
│── README.md                 # Documentação do projeto
```
---  

## 📦 Como Executar o Projeto

### 🔹 Clonar o Repositório
```sh
git clone https://github.com/pedroar9/fake-shop.git
cd fake-shop
```

### 🔹 Construir a Imagem Docker
```sh
docker build -t fake-shop .
```

### 🔹 Executar o Contêiner
```sh
docker run -p 5000:5000 fake-shop
```

A aplicação estará rodando em:
📍 http://localhost:5000

---  

## ⚙️ Variáveis de Ambiente

Para o funcionamento correto do projeto, defina as seguintes variáveis de ambiente:

| Variável        | Descrição                                   |
|----------------|---------------------------------|
| `DB_HOST`     | Host do banco de dados PostgreSQL |
| `DB_USER`     | Nome do usuário do banco de dados PostgreSQL |
| `DB_PASSWORD` | Senha do usuário do banco de dados PostgreSQL |
| `DB_NAME`     | Nome do banco de dados PostgreSQL |
| `DB_PORT`     | Porta de conexão com o banco de dados PostgreSQL |  

---  


🔄 Como Usar a API

A API do Fake Shop está configurada para oferecer funcionalidades de um e-commerce, como gerenciamento de produtos e pedidos.

---  


🌍 Publicação no DockerHub

A imagem do projeto está disponível no DockerHub e pode ser baixada diretamente com o comando:

```sh
docker pull pedroar9/fake-shop-desafio:v1
```
ou

```sh
docker pull pedroar9/fake-shop-desafio:v2
```

🔗 **Link da imagem:** [DockerHub - pedroar9/fake-shop-desafio](https://hub.docker.com/r/pedroar9/fake-shop-desafio/tags)

---

## 👨‍💻 Autor

**Pedro Assis**

[![Linkedin](https://i.sstatic.net/gVE0j.png) LinkedIn](https://www.linkedin.com/in/pedrocarlos-assis/) | [![GitHub](https://i.sstatic.net/tskMh.png) GitHub](https://github.com/pedroar9) | 📧 [Email](mailto:pedrocarlos.assis@gmail.com)
---

## 📝 Licença

Este projeto está sob a licença MIT - veja o arquivo [LICENSE](https://mit-license.org/) para mais detalhes.

---