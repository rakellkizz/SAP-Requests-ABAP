# SAP-Requests-ABAP

# Request no SAP - Explicação Completa

## O que é um Request no SAP?
No SAP, um **request (ou ordem de transporte)** é um mecanismo utilizado para gerenciar alterações feitas no sistema e garantir que sejam movidas de um ambiente para outro (por exemplo, de desenvolvimento para qualidade e produção).

Esses requests são armazenados no sistema de gerenciamento de transporte do SAP (**Transport Management System - TMS**), garantindo que todas as modificações sejam controladas e documentadas corretamente.

---

## Tipos de Requests no SAP
Existem dois tipos principais de requests no SAP:

### 1. **Workbench Request (Tipo: Workbench - "W")**
- Utilizado para objetos independentes de cliente (**cross-client**), como programas ABAP, tabelas, classes e configurações técnicas.
- Quando um objeto está associado a um Workbench Request, ele pode ser transportado para outros sistemas.

### 2. **Customizing Request (Tipo: Customizing - "C")**
- Usado para configurações específicas de um cliente (**client-dependent**), como parâmetros de configuração de módulos do SAP.
- Contém apenas entradas em tabelas de Customizing.

**Outros tipos incluem:**
- **Transporte de código ABAP (TASK dentro de uma Workbench Request).**
- **Requests manuais para movimentação de dados específicos (por exemplo, configurações específicas de um cliente).**

---

## Como Criar um Request no SAP?
1. Acesse a transação **SE09** (para objetos Workbench) ou **SE10** (para Customizing).
2. Clique em **Criar Request** (F6).
3. Escolha o tipo de Request (**Workbench** ou **Customizing**).
4. Informe uma descrição clara da alteração realizada.
5. Associe objetos ao request (por exemplo, um programa ABAP, uma tabela, ou configurações de Customizing).
6. Salve e libere a ordem quando estiver pronta para transporte (**SE10 > Liberar**).

---

## Como Funciona o Transporte no SAP?
O processo de transporte segue estas etapas:
1. **Criação do Request** → As alterações são agrupadas em um request.
2. **Aprovação** → Um desenvolvedor ou consultor responsável revisa e libera o request.
3. **Exportação** → O request é exportado do ambiente de desenvolvimento.
4. **Importação** → O request é importado para o ambiente de qualidade e, posteriormente, para produção.

Os administradores do SAP gerenciam esse transporte utilizando a transação **STMS** (**Transport Management System**).

---

## Conclusão
O sistema de requests no SAP é essencial para garantir um fluxo de trabalho organizado e seguro dentro do ambiente de desenvolvimento. Ele permite que mudanças sejam documentadas, revisadas e transportadas de maneira eficiente entre os sistemas SAP.

Se você está iniciando no mundo SAP, dominar o conceito de requests e transporte é fundamental para o desenvolvimento e configuração dentro do sistema.

---

### 🔗 Recursos Adicionais
- [SAP Help - Change and Transport System](https://help.sap.com)
- [Transações SAP: SE09, SE10, STMS]
- [Curso OpenSAP sobre Desenvolvimento ABAP]

Se precisar de mais informações, entre em contato! 🚀

