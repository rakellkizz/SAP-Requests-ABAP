# SAP-Requests-ABAP

# 🚀 Request no SAP - Guia Completo

## 📌 Sobre o Projeto
Este repositório contém uma explicação detalhada sobre o conceito de **Request no SAP**, sua importância e como utilizá-lo corretamente dentro do sistema. Ele serve como um guia para iniciantes que desejam entender como funciona o gerenciamento de transporte no SAP.

---

## 📖 O que é um Request no SAP?
No SAP, um **Request** (ou **Ordem de Transporte**) é um mecanismo usado para gerenciar mudanças feitas no sistema e transportá-las entre diferentes ambientes (ex: Desenvolvimento → Qualidade → Produção). 

Os requests garantem que todas as modificações sejam controladas e documentadas corretamente através do **Transport Management System (TMS)**.

---

## 🔹 Tipos de Requests no SAP

### 1️⃣ Workbench Request (**W**)
✔️ Utilizado para objetos **independentes de cliente** (*cross-client*), como:
- Programas ABAP
- Tabelas
- Classes
- Configurações técnicas

### 2️⃣ Customizing Request (**C**)
✔️ Usado para configurações **dependentes de cliente** (*client-dependent*), como:
- Parâmetros de configuração de módulos do SAP
- Ajustes específicos de um cliente

📌 Outros tipos incluem transporte de código ABAP, requests manuais e ajustes específicos de um ambiente.

---

## ⚙️ Como Criar um Request no SAP?
1. Acesse a transação **SE09** (Workbench) ou **SE10** (Customizing).
2. Clique em **Criar Request (F6)**.
3. Escolha o tipo de Request (**Workbench** ou **Customizing**).
4. Adicione uma descrição clara da mudança.
5. Associe os objetos necessários (ex: programas ABAP, tabelas, configurações).
6. Salve e libere a ordem quando estiver pronta para transporte (**SE10 > Liberar**).

---

## 🔄 Como Funciona o Transporte no SAP?
1️⃣ **Criação do Request** → As mudanças são agrupadas.
2️⃣ **Aprovação** → O desenvolvedor ou consultor revisa e libera.
3️⃣ **Exportação** → O request é enviado do ambiente de desenvolvimento.
4️⃣ **Importação** → O request é transportado para qualidade e produção.

Os administradores do SAP gerenciam esses transportes através da transação **STMS**.

---

## 📚 Recursos Adicionais
📌 [SAP Help - Change and Transport System](https://help.sap.com)  
📌 [Transações SAP: SE09, SE10, STMS]  
📌 [Curso OpenSAP sobre Desenvolvimento ABAP](https://open.sap.com/)  

---

## 🤝 Contribuições
Sinta-se à vontade para contribuir com este repositório! Se tiver dúvidas ou sugestões, abra uma **Issue** ou envie um **Pull Request**. 🚀

---

## 📝 Licença
Este projeto está sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

💡 **Criado para ajudar desenvolvedores SAP a entender Requests e Transportes.**
