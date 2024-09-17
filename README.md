# 🐾 Teste de API REST de Cadastro de Cães

Este projeto implementa uma API REST utilizando Node.js e Express para realizar operações CRUD básicas. A API está conectada a um banco de dados MongoDB através do Mongoose, permitindo a modelagem e manipulação de dados com schemas.

## 🚀 Funcionalidades

- **Cadastro de Cães:** Permite o registro de cães com as seguintes informações:
  - Nome 🐶
  - Tutor 👤
  - Raça 🐕
  - Sexo 🚻
  - Cor do pelo 🎨

- **Consulta por ID:** Endpoint para consultar um cão específico através de seu ID. 🔍

![Captura de tela 2024-09-17 181354](https://github.com/user-attachments/assets/35eea5f9-338c-4727-8fa0-02649023850a)

- **Remoção de Cães:** Endpoint para remover um cão do sistema usando seu ID. 🗑️

 ![Captura de tela 2024-09-17 181523](https://github.com/user-attachments/assets/47a44dfb-dda6-457f-9352-01acb02aed72)

## 🧪 Testes

- **Testes com Cypress:** Testes automatizados foram criados para validar cada endpoint da API, com foco nas operações CRUD. 🔧
- O teste garante que não tem dois cães iguais cadastrados.

![cy op](https://github.com/user-attachments/assets/6ea2b78c-c46c-4929-99cd-544789249183)
![1cy](https://github.com/user-attachments/assets/30960a0f-e251-4121-b110-f4bc70b96464)


- **Validação de Erros com Postman:** Utilizamos Postman para validar o tratamento de erros e garantir que a API lida adequadamente com entradas incorretas e outros cenários de falha. 📬
  

## 🛠️ Ferramentas Utilizadas

- **Git Bash:** Utilizado para validar a operação da porta do Mongoose (porta 5000) e outras operações relacionadas ao desenvolvimento. 💻
- **Nodemon:** Utilizado para reiniciar automaticamente a aplicação Node.js durante o desenvolvimento, facilitando o processo de desenvolvimento e testes contínuos. 🔄
- ![nodemon](https://github.com/user-attachments/assets/c9047c84-601f-4321-bc47-6d5b1ab09a11)


## ⚙️ Boas práticas

-Tentei ao máximo utilizar boas práticas de clean code utilizando Custom Commands no Cypress, criando comandos personalizados que podem ser reutilizados, evitando repetir código e deixando seus testes mais fáceis de entender.

![Captura de tela 2024-09-17 182653](https://github.com/user-attachments/assets/97743936-753a-40ba-9cc3-6d33498c2eb3)

-Realizei o uso de um plugin da NPM para garantir que os testes sejam isolados e executados em um ambiente controlado, evitando que dados anteriores afetem os próximos testes. (repare que na foto do Mongo temos somente 1 documento mesmo quando damos reload, sem isso os documentos ficam consumindo o banco e armazenando dados desnecessários.


![Captura de tela 2024-09-17 183324](https://github.com/user-attachments/assets/3d4c4391-7246-4225-bc12-8df26db19d48)

![Captura de tela 2024-09-17 183140](https://github.com/user-attachments/assets/43de30d7-7460-4e1b-a3f6-28c4a5d7bece)



## ⚙️ Tecnologias Utilizadas

- **Node.js** e **Express** para desenvolvimento da API
- **MongoDB** com **Mongoose** para gerenciamento de dados
- **Cypress** para testes automatizados
- **Postman** para validação de erros e testes manuais

  ## 📁 Estrutura de Pastas

📦 cypress  
 ┣ 📂 downloads  
 ┣ 📂 e2e  
 ┃ ┗ 📜 dogs.cy.js  
 ┣ 📂 fixtures  
 ┃ ┗ 📜 example.json  
 ┗ 📂 support  
   ┣ 📜 commands.js  
   ┗ 📜 e2e.js  
📦 models  
 ┗ 📜 Dog.js  
📦 node_modules  
📦 routes  
 ┗ 📜 dogs.js  
📜 cypress.config.js  
📜 package-lock.json  
📜 package.json  
📜 server.js

