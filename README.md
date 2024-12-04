# Repositório de Documentações

**Por favor, leia antes de usar**

Este repositório foi criado para centralizar as documentações relacionadas aos testes de hardware e ao desenvolvimento de projetos. Siga as orientações abaixo para manter o repositório organizado e acessível a todos os colaboradores.

## Estrutura de Pastas

A organização do repositório atualmente possui a seguinte aparência:

```
DOCUMENTATIONS/
│
├── Comunicação/
│   └── E28/
|       ├─ src/ ... 
|       └─ README.md
│   ├── ESP-Now/...
│   ├── NRF24L01L/...
│   └── README.md
│
├── DriversBDC/
│   └── ESC01/ .... 
│   └── README.md
│
├── DriversBLDC/
│   └── README.md
│
├── kicker/
│   └── README.md
│
├── Sensores/
│   └── README.md
│
├── LICENSE
└── README.md
```

### Detalhes sobre a Estrutura:
1. **Comunicação**: Contém documentações relacionadas a módulos de comunicação, como E28, ESP-Now, e NRF24L01L.
2. **DriversBDC e DriversBLDC**: Documentações relacionadas a drivers para controle de motores de corrente contínua e motores brushless.
3. **kicker**: Documentações específicas de mecanismos ou dispositivos atuadores.
4. **Sensores**: Contém informações de hardware e bibliotecas relacionadas a sensores.
5. **README.md**: Cada pasta deve ter um arquivo `README.md` descrevendo o conteúdo, a configuração e os testes realizados.

Sinta-se a vontade para criar novas divisões se assim achar necessário.


## Regras para Colaboração

### 1. Criação de Novas Documentações
- Para documentar um novo teste de hardware ou funcionalidade:
  1. Crie uma nova branch com o padrão:
     ```
     feat/nome_do_hardware
     ```
  2. Documente o hardware em uma nova pasta, seguindo a estrutura já existente ou se necessário, crie um novo ramo.
    - A pasta deve conter:
        - **README.md** com as instruções completas:
            - Adicione um arquivo `README.md` dentro da pasta, usando os templates já existentes.
        - Scripts ou códigos usados nos testes;
        - Resultados ou dados relevantes do teste.
  4. Após finalizar, crie um Pull Request (PR) para a branch `main` com uma descrição detalhada do teste.

### 2. Correções ou Melhorias
- Para corrigir um erro ou melhorar uma documentação existente:
  1. Crie uma nova branch com o padrão:
     ```
     fix/nome_do_hardware
     ```
  2. Realize as alterações necessárias e garanta que as informações estejam claras e atualizadas.
  3. Crie um PR para a branch `main`, detalhando as mudanças realizadas.

### 3. Boas Práticas de Git
- Sempre use mensagens de commit claras e objetivas:
  ```
  feat: (feature) Adiciona documentação para o módulo E28
  fix: (correção) Correção do erro na configuração do NRF24L01L
  wip: (work in progress) Trabalhando no protocolo do NRF24L01L
  ```
- Evite commits diretos na branch `main`.
- Após a revisão e aprovação, as alterações serão integradas na branch principal.



Com essas regras, garantimos que o repositório se mantenha organizado, consistente e acessível para toda a equipe.