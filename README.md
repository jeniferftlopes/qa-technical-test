
````md
# QA Technical Test

Projeto desenvolvido para validação técnica de QA contemplando testes funcionais manuais e testes de API.

---

# Objetivo

Validar funcionalidades da aplicação Sauce Demo e da API Restful Booker através de cenários positivos e negativos, utilizando testes manuais e Postman.

---

# Aplicações Testadas

## UI Testing
- Sauce Demo
- https://www.saucedemo.com

## API Testing
- Restful Booker
- https://restful-booker.herokuapp.com

---

# Ferramentas Utilizadas

- Postman
- Google Chrome
- macOS
- GitHub
- Markdown
- Microsoft Word

---

# Estrutura do Projeto

```txt
qa-technical-test/
│
├── evidencias-ui/
├── evidencias-api/
├── README.md
├── UI_Testing_Evidence_Report.docx
├── API_Testing_Evidence_Report.docx
└── Restful Booker - QA Test.postman_collection.json
```

---

# Cenários Testados

# UI Testing

## Fluxo de autenticação
- Login válido
- Login inválido
- Usuário bloqueado

## Gerenciamento de produtos
- Ordenação A-Z
- Ordenação Z-A
- Ordenação por preço
- Adicionar/remover produtos

## Checkout
- Fluxo completo de compra
- Checkout sem itens
- Validação de campos obrigatórios

## Navegação
- Navegação entre páginas
- Logout

---

# API Testing

## Autenticação
- Geração de token

## CRUD de reservas
- Create Booking
- Get Booking
- Update Booking
- Partial Update Booking
- Delete Booking

## Filtros e buscas
- Busca por firstname
- Busca por lastname

## Cenários negativos
- Update sem token
- Booking inexistente
- Datas inválidas
- Campo obrigatório ausente

---

# Bugs Encontrados

## UI
- Imagens incorretas com problem_user
- Lentidão no login com performance_glitch_user
- Checkout permitido sem produtos
- Usuário bloqueado

## API
- API aceita datas inválidas no Create Booking

---

# Como Executar os Testes

## UI Testing
1. Acessar https://www.saucedemo.com
2. Executar os cenários documentados
3. Validar comportamento esperado
4. Registrar evidências

---

## API Testing
1. Abrir o Postman
2. Importar a collection:
   - `Restful Booker - QA Test.postman_collection.json`
3. Configurar environment:
   - `baseUrl`
   - `token`
   - `bookingId`
4. Executar os requests na ordem:
   - Create Token
   - Create Booking
   - Get Booking
   - Update Booking
   - Partial Update
   - Delete Booking

---

# Premissas Assumidas

- A aplicação Sauce Demo é utilizada para fins de treinamento QA.
- Os usuários especiais simulam comportamentos específicos da aplicação.
- A API Restful Booker pode apresentar comportamentos inconsistentes em cenários negativos.

---

# Evidências

As evidências dos testes estão organizadas nas pastas:

- `evidencias-ui`
- `evidencias-api`

---

# Considerações Finais

Os testes executados cobriram os requisitos obrigatórios do desafio técnico, incluindo validações funcionais, cenários negativos, análise de bugs e documentação das evidências.
````

