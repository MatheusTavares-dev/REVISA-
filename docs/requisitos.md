# Documentação de Requisitos

## 1. Requisitos Funcionais

### 1.1 Cadastro e Autenticação de Usuários
- Cadastro com nome completo, e-mail e senha
- Login via Google
- Recuperação de senha por e-mail
- Senha armazenada com hash seguro
- Edição e exclusão da conta

### 1.2 Cadastro de Veículos
- Cadastro de múltiplos veículos por usuário
- Campos obrigatórios: marca, modelo, ano, tipo de combustível, quilometragem atual, placa
- Validação de placa (formatos Mercosul e antigo)
- Prevenção de duplicidade de placa
- Indicação de proprietário e motoristas autorizados
- Edição e exclusão de veículos com controle de permissões

### 1.3 Compartilhamento de Veículo
- Compartilhamento por e-mail ou código de convite
- Controle de permissões (visualização ou edição)
- Remoção de acesso a qualquer momento
- Notificações de alterações feitas por convidados
- Transferência de propriedade

### 1.4 Registro de Manutenções
- Tipo de serviço, data, quilometragem, oficina, valor, observações
- Upload de nota fiscal com leitura automática de dados (OCR)
- Edição e exclusão com rastreamento de autor

### 1.5 Alertas Inteligentes
- Alertas por tempo e quilometragem
- Notificações para todos os motoristas
- Sugestões de alertas baseadas no histórico
- Cálculo dinâmico de alertas

### 1.6 Histórico e Relatórios
- Histórico completo por veículo
- Filtros por motorista, serviço, oficina, data
- Relatórios visuais e exportação em PDF
- Geração de relatório de entrega

### 1.7 Atualização de Quilometragem
- Atualização manual
- Histórico de atualizações por usuário

### 1.8 Módulo de Despesas Gerais
- Registro de IPVA, seguro, multas, lavagens, etc.
- Categorização de despesas
- Relatórios por mês, categoria e veículo

### 1.9 Checklist de Viagem
- Lista sugerida baseada em tipo de viagem e revisão
- Exportação em PDF

---

## 2. Requisitos Não Funcionais

### 2.1 Segurança e Permissões
- Controle de permissões de usuários
- Criptografia de dados
- Autenticação JWT
- Confirmações para ações críticas

### 2.2 Compatibilidade e Acessibilidade
- Android (mínimo 8.0)
- Modo escuro
- Layout responsivo e acessível

### 2.3 Performance e Escalabilidade
- Tela inicial carregando em até 2 segundos
- Backend desacoplado e escalável (Node.js + PostgreSQL)

### 2.4 Funcionalidade Offline
- Salvamento e notificações locais
- Sincronização posterior segura

### 2.5 Backup e Confiabilidade
- Backup diário com criptografia
- Logs e testes automatizados

### 2.6 Suporte Multilíngue e Integração
- Interface em português com estrutura para multilíngue
- Integração com calendário de celular

---

## 3. Requisitos de Negócio

### 3.1 Validação de Placas
- Aceitação dos formatos ABC-1234 e AAA1A11
- Máscara e validação automática
- Prevenção contra duplicidade de placas

### 3.2 Proposta de Valor
- Controle de manutenção para evitar prejuízos e prolongar a vida útil dos veículos

### 3.3 Monetização
- Versão gratuita com funções básicas
- Versão premium com recursos adicionais

### 3.4 Parcerias
- Parcerias com oficinas, seguradoras e lojas de autopeças

### 3.5 KPIs
- Número de usuários ativos
- Taxa de engajamento com alertas
- Registros de manutenção preventiva/mês
- Retenção de usuários após 30 dias

### 3.6 Suporte e Atualizações
- Atualizações trimestrais
- Suporte via e-mail ou formulário

### 3.7 Plano Corporativo
- Gestão de frotas para pequenas e médias empresas

### 3.8 Recompensas por Uso Contínuo
- Pontuação para boas práticas de manutenção

### 3.9 Loja de Serviços Integrada (futuro)
- Catálogo de oficinas com agendamento e promoções

### 3.10 Avaliação de Serviços
- Sistema de avaliação e reputação de oficinas

### 3.11 API Pública
- API para integração com terceiros

---
