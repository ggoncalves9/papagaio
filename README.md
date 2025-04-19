# 📦 Etapa 1 - Deploy Local com Docker Compose – Projeto Papagaio

## ✅ Objetivo
Subir LangFlow com banco PostgreSQL e monitoramento (Prometheus + Grafana), com proxy reverso e autenticação simples.

---

### 🔧 [ ] 1. Pré-instalação no EliphasServer
- [ ] Instalar Docker e Docker Compose (`pre-projeto/install_tools.sh`)
- [ ] Testar conexão do servidor com Docker

---

### 📦 [ ] 2. Infraestrutura Docker
- [ ] Criar `docker-compose.yaml` com:
  - [ ] LangFlow (imagem oficial + configurações customizadas)
  - [ ] PostgreSQL com volume persistente
  - [ ] PgAdmin para acesso ao banco
  - [ ] NGINX como proxy reverso
  - [ ] Prometheus + Grafana com configuração mínima

---

### 🧩 [ ] 3. Configurações e Segurança
- [ ] Arquivo `.env` para segredos e senhas
- [ ] Configuração de dois usuários para LangFlow:
  - `admin@realmirage.com.br / victory123`
  - `user@realmirage.com.br / 123`
- [ ] Documentar portas expostas

---

### 📊 [ ] 4. Observabilidade
- [ ] Exportar métricas básicas com Prometheus
- [ ] Subir Grafana com dashboard inicial
- [ ] Criar volume persistente para Grafana

---

### 🌐 [ ] 5. Rede e Acesso
- [ ] Configurar acesso via IP `192.168.15.161`
- [ ] NGINX como proxy reverso (porta 80 → LangFlow)
- [ ] Documentar estrutura e rotas no código

---

### ✅ [ ] 6. Testes e Validação
- [ ] Acessar LangFlow localmente e via IP
- [ ] Acessar PgAdmin e validar banco
- [ ] Acessar Grafana e validar dashboard
