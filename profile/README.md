<div align="center">

# 7WAMP

**Ambiente integrado de alto desempenho para desenvolvimento e orquestração de servidores locais.**

Uma evolução moderna e blindada para stacks WAMP, baseada nos conceitos de controle unificado com foco em estabilidade, segurança ativa e ferramentas completas para bancos de dados e cache em memória.

---

[![Status](https://img.shields.io/badge/Status-Active_Development-00d26a?style=for-the-badge)](#)
[![Stack](https://img.shields.io/badge/Architecture-High_Performance-007acc?style=for-the-badge)](#)
[![Security](https://img.shields.io/badge/Protection-Watchdog_%26_Anti--DDoS-e63946?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-GPL_v2-black?style=for-the-badge)](#)

</div>

---

## ⚡ Sobre a Organização 7WAMP

O ecossistema **7WAMP** expandindo a proposta original para entregar uma solução resiliente, tolerante a falhas e pronta tanto para desenvolvimento diário quanto para simulações rigorosas de pré-produção.

Diferente de gerenciadores tradicionais de ambiente local que apenas disparam processos básicos, o 7WAMP incorpora controle transacional dos serviços, interfaces avançadas de gerenciamento de cache e bancos de dados relacionais duplos, além de defesas em nível de aplicação.

---

## 🚀 Principais Diferenciais e Módulos Integrados

### 🗄️ Flexibilidade Relacional: MySQL & MariaDB
* **MySQL:** Suporte ao motor transacional oficial da Oracle com suporte completo a dados JSON binários de alta performance.
* **MariaDB:** Opção 100% open source equipada com Thread Pool nativo e motores versáteis (Aria, ColumnStore), selecionável diretamente pelo painel.

### ⚡ Cache em Memória: Redis + phpRedisAdmin
* **Redis Server:** Execução local de cache chave-valor para testes com sessões de alta velocidade, filas de mensageria e indexação rápida de dados.
* **phpRedisAdmin:** Painel web integrado para inspecionar chaves, gerenciar índices TTL e monitorar a memória do Redis sem necessidade de comandos via CLI.

### 🛠️ Gerenciamento Visual com HeidiSQL
* Integração nativa e atalho rápido para o **HeidiSQL**, permitindo conexão imediata, exportação, sincronização de schemas e administração completa das instâncias MySQL e MariaDB em uma interface nativa leve.

### 🛡️ Engenharia de Blindagem e Resiliência
* **Watchdog Supervisor:** Monitoramento ativo do ciclo de vida dos processos. Caso o servidor sofra paradas forçadas ou falhas críticas, o supervisor restabelece as instâncias automaticamente.
* **Mitigação de Ataques de Aplicação:** Rate limiting, timeouts para conexões lentas (estilo Slowloris) e detecção de sobrecarga para proteger o painel contra travamentos acidentais durante testes de carga.
* **Execução Segura:** Controle de processos isolado sem execução de comandos em shell arbitrário, mitigando vetores de injeção de parâmetros no host.

---

## 🧩 Matriz de Componentes

| Componente | Função | Diferencial Integrado |
| :--- | :--- | :--- |
| **Apache / Nginx** | Web Server Engine | Mapeamento inteligente de vhosts e isolamento local |
| **PHP Multi-Versão** | Runtime | Troca rápida de versão e controle de extensões |
| **MariaDB** | RDBMS | Thread Pool ativado e suporte a engines analíticos |
| **MySQL** | RDBMS | Compatibilidade nativa estrita com ecossistemas Oracle |
| **Redis** | NoSQL & Cache | Instância local para sessões e mensageria |
| **phpRedisAdmin** | Interface de Cache | Inspeção visual de chaves em tempo real |
| **HeidiSQL** | Client SQL Desktop | Ferramenta visual leve e integrada ao fluxo do painel |
| **Watchdog Core** | Autocura / Resiliência | Recuperação automática de crashes e supervisão contínua |

---

## 📌 Filosofia de Arquitetura

O 7WAMP prioriza três diretrizes fundamentais:

1. **Autonomia:** Mínima intervenção manual para resolver conflitos de portas, travamentos de serviços ou reinícios pós-falha.
2. **Modularidade:** Facilidade para alternar entre engines relacionais (MySQL vs MariaDB) e habilitar camadas de cache conforme as demandas do projeto.
3. **Segurança por Padrão:** Serviços vinculados estritamente às interfaces corretas por padrão, evitando exposições acidentais de portas administrativas à rede local ou externa.

---

<div align="center">

Desenvolvido para entregar o máximo de controle, desempenho e tolerância a falhas no ecossistema local.

<sub>7WAMP &copy; 2026</sub>

</div>
