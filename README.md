# Service Unitary Test

[![NPM](https://img.shields.io/npm/l/react)](https://github.com/WelingtonFranzoso/service-unitary-tests/blob/main/LICENSE) 


# Sobre o projeto

Este projeto é um serviço Java baseado em Spring Boot, desenvolvido para demonstrar a implementação de testes unitários. Ele inclui um CRUD para gestão de pessoas, utilizando JPA para persistência e Mockito para testes.

# Funcionalidades
- Criar uma nova pessoa

- Buscar uma pessoa por ID

- Listar todas as pessoas

- Atualizar os dados de uma pessoa

- Remover uma pessoa do sistema

# Tecnologias utilizadas

- Java 17+

- Spring Boot

- Maven

- JUnit e Mockito (para testes)

# Estrutura do Projeto
```
service-unitary-test/
│-- src/
│   ├── main/
│   │   ├── java/com/franzoso/
│   │   │   ├── controllers/PersonCerontroll.java
│   │   │   ├── entities/Person.java
│   │   │   ├── exceptions/BusinessException.java
│   │   │   ├── repositories/PersonRepository.java
│   │   │   ├── services/PersonService.java
│   │   │   ├── UnitaryTestsApplication.java
│   ├── test/
│   │   ├── java/com/franzoso/services/PersonServiceTest.java
│-- pom.xml
```

# Como executar o projeto
## Back end
### Pré-requisitos: 
- Java 17 ou superior
- Maven (para construção do projeto)

```bash
# clonar repositório
git clone git@github.com:WelingtonFranzoso/service-unitary-tests
.git

# entrar na pasta do projeto back end
cd service-unitary-tests

# executar o projeto
./mvnw spring-boot:run
```

## Executando Testes

### O projeto usa JUnit e Mockito para testes.

```bash
# executar os tests
mvn test
```

# Endpoints Disponíveis

| Método | Endpoint      | Descrição                       |
|:------:|:-------------:|:-------------------------------:|
| GET    | /persons      | Lista todas as pessoas          |
| POST   | /persons      | Cria uma nova pessoa            |
| GET    | /persons/{id} | Busca uma pessoa pelo ID        |
| PUT    | /persons/{id} | Atualiza os dados de uma pessoa |
| DELETE | /persons/{id} | Remove uma pessoa do sistema    |


# Contribuição

1. Fork este repositório

2. Crie uma branch (feature-nova)

3. Commit suas mudanças (git commit -m 'Add nova feature')

4. Push para sua branch (git push origin feature-nova)

5. Crie um Pull Request

# Licença

- Este projeto está sob a licença MIT. Sinta-se livre para usá-lo e modificá-lo.
