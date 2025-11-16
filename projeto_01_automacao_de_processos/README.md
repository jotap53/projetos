# 📧 Automação de Relatório Diário com PyAutoGUI

Este projeto tem como objetivo automatizar o envio diário do relatório de vendas para a diretoria da empresa.  
Todos os dias, o sistema interno atualiza os dados de vendas do dia anterior em uma pasta no Google Drive, e o analista precisa enviar por e-mail o faturamento e a quantidade de produtos vendidos.

Para eliminar esse processo manual, foi criado um script em **Python + PyAutoGUI** capaz de:

- Acessar automaticamente o sistema (Google Drive)  
- Baixar a base de dados do dia anterior  
- Processar o arquivo com **Pandas**  
- Calcular os indicadores principais:  
  - **Faturamento total**  
  - **Quantidade de produtos vendidos**  
- Enviar tudo por e-mail para a diretoria  

---

## 🚀 Funcionalidades

✔️ Acessa o Google Drive automaticamente usando PyAutoGUI  
✔️ Baixa o arquivo de vendas do dia anterior  
✔️ Processa os dados usando Pandas  
✔️ Calcula faturamento e quantidade de produtos vendidos  
✔️ Envia um e-mail automático para **seugmail+diretoria@gmail.com**  
✔️ Automação 100% sem intervenção manual  

---

## 🛠 Tecnologias Utilizadas

- **Python 3.14.0**
- **PyAutoGUI** – automação de mouse e teclado  
- **Pandas** – manipulação de dados  
- **OpenPyXL** – suporte a arquivos Excel  

### Instalação das Bibliotecas
```python
pip install pandas pyautogui openpyxl
```
---

## 🧩 Etapas da Automação

### **1. Entrar no sistema da empresa**  
A automação abre o navegador e acessa a pasta oficial de vendas do dia anterior:  
https://drive.google.com/drive/folders/149xknr9JvrlEnhNWO49zPcw0PW5icxga

### **2. Navegar até o arquivo de vendas**  
O PyAutoGUI controla o mouse para localizar o arquivo mais recente.

### **3. Exportar os dados**  
O arquivo é baixado automaticamente.

### **4. Processar as informações**  
Usando Pandas, o script calcula:

- **Faturamento total** (soma de valores)  
- **Quantidade de itens vendidos**

### **5. Enviar o e-mail para a diretoria**  
O relatório final é escrito e enviado automaticamente.

---

## 📬 E-mail enviado

O script monta e envia um e-mail contendo:

- Faturamento do dia anterior 
- Quantidade de produtos vendidos

---

## ⭐ Objetivo do Projeto

Este projeto demonstra uma solução prática de automação usada no dia a dia de análise de dados, unindo:

- **RPA (Robotic Process Automation)**  
- **Manipulação de dados**  
- **Integração com e-mail**
---

## 🎬 Demonstração do Projeto Rodando
![👉 Clique aqui ](./demo.gif)
