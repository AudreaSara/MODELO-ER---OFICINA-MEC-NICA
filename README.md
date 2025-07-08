# 💻 Sistema de Oficina Mecânica - Esquema Conceitual

Este projeto tem como objetivo representar um **esquema conceitual (modelo ER)** para um sistema de **gerenciamento de ordens de serviço em uma oficina mecânica**, desenvolvido como parte de um desafio da plataforma DIO.

---

## 📘 Contexto do Sistema

A oficina recebe veículos de clientes para manutenção ou revisão. Cada veículo é atribuído a uma **equipe de mecânicos**, que identifica os serviços necessários e gera uma **ordem de serviço (OS)**. Os valores da OS são calculados com base em uma tabela de mão-de-obra e nos valores das peças utilizadas.

---

## 🧩 Componentes do Modelo ER

### Entidades Principais:
- **Cliente**: identifica os donos dos veículos.
- **Veículo**: pertence a um cliente e pode passar por várias ordens de serviço.
- **Equipe**: conjunto de mecânicos responsáveis por uma OS.
- **Mecânico**: profissionais com especialidades distintas.
- **Ordem de Serviço (OS)**: documento de controle dos serviços executados.
- **Serviço**: atividades realizadas na oficina.
- **Peça**: componentes utilizados nas manutenções.

### Relacionamentos:
- Um cliente pode ter vários veículos.
- Cada veículo pode gerar várias ordens de serviço.
- Cada ordem de serviço é atribuída a uma equipe.
- Uma equipe contém vários mecânicos.
- Uma ordem de serviço pode incluir diversos serviços e várias peças.

---

## 🛠️ Observações
- Valores de mão-de-obra são consultados em uma tabela de referência.
- Caso um dado não tenha sido explicitado na narrativa, foram feitas suposições razoáveis, como adicionar uma tabela intermediária para representar relações N:M entre OS e serviços/peças.

---

## 📂 Tecnologias
- Modelagem: MySQL Workbench
- Linguagem: Modelo Entidade-Relacionamento (ER)

---

## 🔗 Autoria
Desenvolvido por **Audrea Sara Pimenta de Vasconcelos** como parte do desafio de projeto da DIO.
