```markdown
# 🛡️ Phishing Awareness Lab - Ethical Hacking  

Este projeto tem o objetivo de demonstrar como ataques de **phishing** podem ser conduzidos por hackers mal-intencionados e como podemos **testar e fortalecer a segurança** contra esse tipo de ameaça. **Este guia é apenas para fins educacionais e de auditoria em ambientes autorizados.**  

## ⚠️ Aviso Legal  
Este projeto é destinado a **profissionais de segurança** que possuem **autorização explícita** para realizar testes de engenharia social. **NÃO USE ESTE GUIA PARA FINS ILEGAIS.**  

## 🛠️ Ferramentas Utilizadas  
- **Kali Linux** – Distribuição especializada em pentesting e segurança ofensiva  
- **SET (Social-Engineer Toolkit)** – Framework para testes de engenharia social  

---

## 📌 Configuração do Phishing no Kali Linux  

### 🔹 1. Acesso root  
Antes de iniciar, garanta que você tem privilégios administrativos:  
```bash
sudo su
```

### 🔹 2. Iniciando o SET  
Execute o Social-Engineer Toolkit (SET):  
```bash
setoolkit
```

### 🔹 3. Selecionando o Tipo de Ataque  
No menu do SET, selecione:  
1️⃣ **Social-Engineering Attacks**  
2️⃣ **Web Site Attack Vectors**  
3️⃣ **Credential Harvester Attack Method**  
4️⃣ **Site Cloner**  

### 🔹 4. Obtendo o Endereço da Máquina  
Abra um terminal e descubra o IP da máquina no ambiente de testes:  
```bash
ifconfig
```

Copie o endereço **IP local** da interface de rede ativa (por exemplo, `192.168.1.100`).  

### 🔹 5. Clonando a Página Alvo  
No SET, quando solicitado pela ferramenta, insira a **URL da página legítima** para clonagem:  
```bash
http://www.facebook.com
```

O SET irá clonar a página e hospedar um servidor local para capturar credenciais digitadas na versão falsa do site.  

---

## 🔍 Resultados e Proteção  
### ✅ O que o teste demonstra?  
- Como ataques de phishing funcionam  
- Como credenciais podem ser capturadas em sites falsos  
- A importância da **verificação de URL** e da **autenticação de dois fatores (2FA)**  

### 📸 Exemplo de Captura de Credenciais  
Aqui está um exemplo de saída gerada durante um teste de phishing, mostrando possíveis credenciais capturadas:

![Captura de Tela](passwd.png)

### 🔐 Como se proteger?  
- **Sempre verifique a URL** antes de inserir credenciais  
- **Ative autenticação de dois fatores (2FA)** sempre que possível  
- **Não clique em links suspeitos** enviados por e-mail ou mensagens  
- **Utilize navegadores atualizados** que detectam phishing automaticamente  

---

## 📜 Conclusão  
Este experimento é uma simulação para demonstrar o funcionamento de ataques de engenharia social. A finalidade é conscientizar usuários e profissionais sobre os riscos do phishing e como evitá-lo.  

**Use este conhecimento com responsabilidade! 🚀**  
```
