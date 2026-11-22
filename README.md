# ⌨️ Keyboard Monitoring Lab — Python

### Educational Cybersecurity Project | Python | Windows | Email & Event Monitoring

> **Projeto exclusivamente educacional.** Desenvolvido com o propósito de estudar mecanismos de monitoramento de eventos de teclado, manipulação de eventos no Windows, tratamento de caracteres e conceitos relacionados à segurança da informação. Não deve ser utilizado para monitorar terceiros sem consentimento explícito.

---

## 📌 Sobre o projeto

Este projeto explora, em Python, conceitos relacionados ao monitoramento de eventos de teclado em ambientes Windows, identificação de janelas ativas, tratamento de caracteres especiais e automação de comunicação por e-mail.

A estrutura permite analisar como diferentes componentes de software podem ser integrados, demonstrando também os riscos associados ao uso indevido de mecanismos de monitoramento de entrada.

O projeto é voltado para aprendizado técnico, análise de código e conscientização sobre ameaças cibernéticas.

## 🎯 Objetivos educacionais

- Compreender o funcionamento de listeners de teclado em Python.
- Estudar eventos de teclado e a distinção entre caracteres e teclas especiais.
- Analisar o tratamento de caracteres acentuados em layouts de teclado.
- Compreender a interação entre aplicações Windows e informações da janela ativa.
- Estudar conceitos de threads e execução paralela.
- Conhecer o funcionamento do protocolo SMTP e envio automatizado de mensagens.
- Identificar riscos de privacidade, exposição de informações e monitoramento indevido.
- Desenvolver conhecimentos aplicáveis à análise de ameaças e defesa cibernética.

## 🧰 Tecnologias utilizadas

| Tecnologia | Finalidade técnica |
|---|---|
| Python | Linguagem de programação |
| pynput | Biblioteca para interação com eventos de teclado |
| pywin32 | Integração com recursos e APIs do Windows |
| threading | Conceitos de execução paralela |
| smtplib | Comunicação com servidores SMTP |
| MIME | Estruturação de mensagens de e-mail |
| datetime | Manipulação de datas e horários |
| time | Controle de intervalos e tempo |
| os | Interação com arquivos e sistema operacional |

## 🧠 Arquitetura do projeto

O código está organizado em cinco blocos principais.

### 1. Configuração de e-mail

Responsável pelas variáveis relacionadas à comunicação SMTP, incluindo remetente, destinatário, credenciais e intervalo de envio.

<details>
<summary>Conceitos envolvidos</summary>

- Autenticação SMTP.
- TLS.
- Credenciais de aplicação.
- Estrutura de mensagens MIME.
- Riscos de armazenamento de credenciais no código-fonte.

</details>

### 2. Configurações e variáveis globais

Define estruturas utilizadas pelo programa para representar teclas ignoradas, caracteres acentuados, estado de execução e referências temporais.

<details>
<summary>Conceitos envolvidos</summary>

- Conjuntos (`set`).
- Dicionários (`dict`).
- Variáveis globais.
- Estados de aplicação.
- Representação de caracteres.

</details>

### 3. Funções auxiliares e comunicação

Agrupa funções relacionadas à interação com o sistema operacional, manipulação de arquivos e estruturação da comunicação por e-mail.

<details>
<summary>Conceitos envolvidos</summary>

- Manipulação de arquivos.
- Tratamento de exceções.
- APIs do Windows.
- SMTP.
- Formatação de mensagens.
- Operações de leitura e escrita.

</details>

### 4. Lógica de eventos

Contém a estrutura responsável pelo tratamento dos eventos recebidos e pela análise de diferentes tipos de teclas.

<details>
<summary>Conceitos envolvidos</summary>

- Callbacks.
- Eventos de teclado.
- `try` e `except`.
- Teclas especiais.
- Caracteres Unicode.
- Teclas mortas e acentuação.
- Controle de fluxo.

</details>

### 5. Inicialização e execução paralela

Representa a estrutura de inicialização do programa e a integração entre diferentes componentes.

<details>
<summary>Conceitos envolvidos</summary>

- Ponto de entrada `__main__`.
- Threads.
- Execução em segundo plano.
- Listener.
- Ciclo de vida de processos.

</details>

## 🔬 Roteiro de estudo

O projeto pode ser utilizado como referência para estudos de análise de código e segurança defensiva.

### Etapa 1 — Análise estrutural

- Identificar os módulos importados.
- Analisar a divisão das funções.
- Compreender o fluxo de execução.
- Identificar variáveis globais e dependências.

### Etapa 2 — Análise dos eventos

- Estudar a documentação da biblioteca `pynput`.
- Diferenciar `Key` e `KeyCode`.
- Compreender callbacks.
- Analisar o tratamento de exceções.

### Etapa 3 — Windows e processos

- Estudar os conceitos de janela ativa.
- Compreender a interação entre Python e APIs do Windows.
- Analisar as permissões de aplicações.

### Etapa 4 — Comunicação e segurança

- Estudar SMTP e TLS.
- Compreender autenticação de aplicações.
- Identificar riscos relacionados a credenciais.
- Analisar mecanismos de envio de dados.

### Etapa 5 — Segurança defensiva

- Identificar comportamentos potencialmente maliciosos.
- Estudar mecanismos de detecção de monitoramento de teclado.
- Analisar permissões e persistência de aplicações.
- Conhecer estratégias de prevenção contra coleta indevida de dados.

## ⚠️ Segurança e privacidade

Aplicações que monitoram eventos globais de teclado podem capturar informações sensíveis, incluindo:

- Credenciais de autenticação.
- Informações pessoais.
- Mensagens privadas.
- Dados corporativos.
- Informações financeiras.

A identificação de janelas ativas e a transmissão de registros por e-mail aumentam os riscos de exposição de informações.

### Recomendações

- Não utilizar o projeto em equipamentos de terceiros.
- Não monitorar usuários sem consentimento explícito.
- Não utilizar contas pessoais ou corporativas reais para testes.
- Não armazenar credenciais diretamente no código-fonte.
- Não publicar senhas, tokens ou informações confidenciais no GitHub.
- Realizar análises em ambientes isolados.
- Priorizar estudos de detecção, análise e prevenção.

## 🛡️ Aplicação em cibersegurança

O estudo de mecanismos de monitoramento de teclado pode contribuir para o entendimento de técnicas utilizadas em ameaças cibernéticas, especialmente no contexto de:

- Spyware.
- Keylogging.
- Exfiltração de dados.
- Monitoramento não autorizado.
- Engenharia social.
- Análise de comportamento de malware.
- Segurança de endpoints.

O conhecimento desses mecanismos pode auxiliar profissionais de TI e segurança da informação na identificação de comportamentos suspeitos e no desenvolvimento de estratégias de proteção.

## 📚 Referências

- [Python Documentation](https://docs.python.org/3/)
- [pynput Documentation](https://pynput.readthedocs.io/en/latest/)
- [pywin32 Documentation](https://github.com/mhammond/pywin32)
- [MITRE ATT&CK — Input Capture (T1056)](https://attack.mitre.org/techniques/T1056/)
- [MITRE ATT&CK — Exfiltration (TA0010)](https://attack.mitre.org/tactics/TA0010/)

## ⚖️ Disclaimer

Este repositório possui finalidade exclusivamente educacional e de pesquisa em segurança da informação.

O autor não incentiva, autoriza ou assume responsabilidade pelo uso deste código para monitoramento não autorizado, coleta de informações privadas, violação de privacidade ou qualquer atividade ilícita.

A utilização de ferramentas de monitoramento deve respeitar a legislação aplicável, os direitos individuais, as políticas de segurança e a autorização expressa dos envolvidos.

---

<sub>Educational Cybersecurity Research | Python | Windows | Security Awareness</sub>
