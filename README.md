# 💈 Supreme Barbershop - Sistema de Agendamento Online

Uma solução simples, rápida e intuitiva para clientes agendarem cortes de cabelo e barbeiros gerenciarem sua agenda diária sem perda de tempo.

O projeto elimina a necessidade de conversas demoradas por WhatsApp para consultar horários disponíveis. O cliente acessa, escolhe o serviço, visualiza a foto do barbeiro e agenda em segundos.

![Demo do Supreme Barbershop](https://via.placeholder.com/800x400?text=Screenshot+do+projeto)

> 🔗 **Demo ao vivo:** [adicione aqui o link do Firebase Hosting]

---

## 🚀 Funcionalidades

### 📱 Para o Cliente
- **Interface Intuitiva:** processo de agendamento simples e direto.
- **Escolha de Profissional:** visualização do nome e foto do barbeiro de preferência.
- **Verificação de Disponibilidade:** exibição apenas dos dias e horários livres.
- **Identificação Rápida:** cadastro simplificado com apenas nome e celular.

### 💼 Para o Barbeiro (Painel Administrativo)
- **Autenticação Segura:** login exclusivo para os profissionais da barbearia.
- **Agenda do Dia:** visualização clara do nome do cliente, celular, serviço, data e hora.
- **Notificação Instantânea:** assim que o cliente clica em agendar, o barbeiro recebe uma mensagem de confirmação no seu WhatsApp.

---

## 🛠️ Tecnologias Utilizadas

| Camada | Tecnologia | Função |
|---|---|---|
| Frontend | HTML5, CSS3, JavaScript (Vanilla) | Interface do usuário |
| Backend (BaaS) | Firebase Firestore | Armazenamento de agendamentos e horários em tempo real |
| Backend (BaaS) | Firebase Authentication | Controle de acesso seguro para o painel do administrador |
| Integração | WhatsApp Deep Linking | Notificação gratuita ao barbeiro via link direto |

---

## 📋 Pré-requisitos

- Um navegador web atualizado (Chrome, Edge, Firefox, etc.).
- Uma conta no [Firebase](https://console.firebase.google.com/) para configurar o banco de dados.

---

## 🔧 Instalação e Configuração

**1. Clone o repositório:**

```bash
git clone https://github.com/jtovarmorales93/Supreme-Barbershop.git
```

**2. Configure o Firebase:**

- Crie um projeto no [console do Firebase](https://console.firebase.google.com/).
- Ative o **Firestore Database** e o **Authentication**.
- Adicione as chaves de configuração do seu projeto no arquivo JavaScript correspondente (ex: `firebase-config.js`):

```javascript
const firebaseConfig = {
  apiKey: "SUA_API_KEY",
  authDomain: "SEU_PROJETO.firebaseapp.com",
  projectId: "SEU_PROJETO_ID",
  storageBucket: "SEU_PROJETO.firebasestorage.app",
  messagingSenderId: "SEU_SENDER_ID",
  appId: "SEU_APP_ID"
};
```

> ⚠️ **Importante:** nunca suba credenciais reais em repositórios públicos. Adicione o arquivo de configuração ao `.gitignore` e configure as **Firestore Security Rules** para permitir escrita apenas a usuários autenticados como administradores.

**3. Execução:**

Abra o arquivo `index.html` diretamente no navegador ou utilize uma extensão como o **Live Server** no VS Code.

---

## 🔒 Segurança

Este projeto depende das **Firestore Security Rules** para proteger os dados dos clientes. Certifique-se de restringir a escrita/leitura da coleção de agendamentos apenas a usuários autenticados com permissão de administrador antes de publicar em produção.

---

## 🗺️ Roadmap / Próximos Passos

- [ ] Deploy via Firebase Hosting
- [ ] Testes automatizados
- [ ] Versão mobile-first refinada

---

## 📄 Licença

Este projeto está sob a licença MIT — veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## ✒️ Autor

**José Tovar** - Desenvolvedor Júnior
[GitHub: @jtovarmorales93](https://github.com/jtovarmorales93)
