# - MTA:SA ANDROID

""Android" (https://img.shields.io/badge/Plataforma-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)" (#)
""ARM64" (https://img.shields.io/badge/Arquitetura-ARM64-blue?style=for-the-badge)" (#)
""C++" (https://img.shields.io/badge/Linguagem-C%2B%2B-orange?style=for-the-badge&logo=cplusplus&logoColor=white)" (#)
""Equipe" (https://img.shields.io/badge/Equipe-5%20Desenvolvedores-purple?style=for-the-badge)" (#)
""Status" (https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge)" (#)

Projeto independente desenvolvido por uma equipe de cinco desenvolvedores, dedicado à criação e ao aprimoramento de um cliente Android do Multi Theft Auto: San Andreas (MTA:SA).

---

Sobre o Projeto

O MTA:SA Android é um projeto desenvolvido por uma equipe de cinco desenvolvedores, com o objetivo de construir uma experiência multiplayer do MTA:SA diretamente em dispositivos Android.

O desenvolvimento utiliza como referência técnica o projeto original MTA Neon Android, trabalhando sobre sua arquitetura e implementações existentes para desenvolver melhorias, corrigir problemas e expandir as funcionalidades do cliente.

A integração com a engine do GTA San Andreas será realizada por meio da biblioteca nativa "libGTASA.so", permitindo que o cliente interaja com os componentes necessários do jogo.

O trabalho é dividido entre os cinco integrantes, que possuem liberdade para escolher as áreas e os arquivos em que desejam trabalhar. Posteriormente, as modificações são revisadas, organizadas, testadas e integradas ao repositório principal.

Principais Objetivos

- Desenvolver um cliente multiplayer nativo para Android.
- Integrar os sistemas do cliente com a engine por meio da "libGTASA.so".
- Aprimorar a comunicação entre cliente e servidor.
- Expandir os sistemas de sincronização multiplayer.
- Melhorar a compatibilidade com as funcionalidades do MTA.
- Desenvolver e aprimorar a API Lua.
- Melhorar a estabilidade e o desempenho.
- Corrigir erros e limitações existentes.
- Organizar e documentar a arquitetura do projeto.

---

Arquitetura do Projeto

O projeto utiliza tecnologias nativas do Android e componentes responsáveis pela comunicação com a engine do jogo.

Tecnologias Utilizadas

Tecnologia| Utilização
Android| Plataforma principal
ARM64 / aarch64| Arquitetura de execução
C / C++| Desenvolvimento nativo
C++20| Recursos modernos da linguagem
Android NDK| Compilação nativa
CMake| Gerenciamento de build nativo
Gradle| Compilação do aplicativo
"libGTASA.so"| Integração com a engine
Lua 5.3| Sistema de scripts
Opus| Processamento de áudio
RenderWare| Tecnologia gráfica da engine

Integração com a Engine

A comunicação com a engine será realizada por meio da biblioteca:

libGTASA.so

Essa biblioteca faz parte da camada nativa utilizada pelo cliente para interagir com os componentes da engine do GTA San Andreas.

A integração deverá contemplar sistemas como:

- Gerenciamento de jogadores.
- Controle de entidades.
- Veículos e pedestres.
- Animações.
- Renderização.
- Eventos do jogo.
- Estados e informações da engine.

A implementação será organizada para permitir a comunicação entre os componentes nativos do cliente multiplayer e a engine.

---

Estrutura do Projeto

A organização do código poderá evoluir conforme as necessidades técnicas.

Estrutura de referência:

MTA-SA-ANDROID/
│
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           ├── cpp/
│           │   ├── main.cpp
│           │   ├── game/
│           │   ├── network/
│           │   ├── multiplayer/
│           │   ├── sync/
│           │   ├── lua/
│           │   ├── audio/
│           │   └── utils/
│           │
│           ├── assets/
│           └── AndroidManifest.xml
│
├── docs/
│   ├── ARQUITETURA.md
│   ├── COMPILACAO.md
│   ├── COMUNICACAO.md
│   ├── SINCRONIZACAO.md
│   ├── API_LUA.md
│   └── ROADMAP.md
│
├── CMakeLists.txt
├── build.gradle
├── settings.gradle
└── README.md

A estrutura acima é ilustrativa. A organização real deverá acompanhar os diretórios existentes no código-fonte.

---

Equipe de Desenvolvimento

O projeto é desenvolvido por cinco integrantes, trabalhando de maneira colaborativa em diferentes partes do código-fonte.

Não existe uma divisão rígida em que cada desenvolvedor fica permanentemente responsável por apenas um sistema. Cada integrante pode escolher os arquivos e componentes nos quais deseja trabalhar.

Isso permite que todos contribuam em diferentes áreas, mantendo liberdade de desenvolvimento e evitando que o trabalho fique concentrado em apenas uma pessoa.

Organização do Trabalho

O desenvolvimento segue um processo interno para manter o código organizado e evitar conflitos entre modificações.

1. Escolha: o desenvolvedor escolhe os arquivos ou componentes em que deseja trabalhar.
2. Reserva: informa à equipe quais arquivos pretende modificar.
3. Desenvolvimento: realiza suas alterações individualmente.
4. Entrega: disponibiliza os arquivos modificados ou um Pull Request.
5. Revisão: as alterações são analisadas e possíveis conflitos são resolvidos.
6. Integração: as modificações aprovadas são incorporadas ao repositório principal.
7. Testes: o conjunto atualizado é testado antes de ser considerado concluído.

Organização do Repositório

O GitHub será utilizado como repositório central do projeto.

As alterações deverão ser organizadas para que o trabalho de um desenvolvedor não sobrescreva acidentalmente o de outro.

O código original utilizado como referência permanecerá independente do repositório da equipe.

---

Estado do Desenvolvimento

O progresso será atualizado conforme as implementações forem concluídas e testadas.

Componente| Situação
Estrutura Android| Em desenvolvimento
Integração com "libGTASA.so"| Em desenvolvimento
Comunicação multiplayer| A verificar
Sistema de conexão| A verificar
Sincronização de jogadores| A verificar
Sincronização de pedestres| A verificar
Sincronização de veículos| A verificar
Sistema Lua| A verificar
Sistema de áudio| A verificar
Interface e HUD| A verificar
Otimização| A verificar
Estabilidade| A verificar

«[!NOTE]
Os estados representam o progresso do repositório da equipe. Funcionalidades herdadas do projeto original não serão consideradas novas implementações sem revisão e validação.»

---

Sistemas Multiplayer

Um dos principais objetivos é aprimorar os sistemas necessários para o funcionamento do multiplayer.

Sincronização

As áreas de desenvolvimento incluem:

- Sincronização de jogadores.
- Posição e rotação.
- Animações.
- Veículos.
- Pedestres.
- Combate.
- Estados e ações.
- Eventos multiplayer.
- Gerenciamento de entidades.

Comunicação Cliente-Servidor

A camada de rede será responsável pela comunicação com servidores compatíveis.

Entre suas responsabilidades estão:

- Estabelecimento de conexões.
- Processamento de pacotes.
- Gerenciamento de sessões.
- Transmissão de informações.
- Recebimento de atualizações.
- Tratamento de desconexões.
- Compatibilidade com os protocolos utilizados pelo servidor.

---

Sistema Lua

O projeto pretende ampliar e aprimorar a compatibilidade com os recursos de scripting do MTA.

Os trabalhos nessa área incluem:

- Implementação de funções da API Lua.
- Integração entre Lua e C++.
- Gerenciamento de recursos.
- Eventos e callbacks.
- Funções relacionadas a jogadores.
- Funções relacionadas a veículos.
- Funções relacionadas ao mundo do jogo.
- Documentação das funcionalidades implementadas.

A compatibilidade será acompanhada por documentação técnica e uma matriz de funcionalidades.

---

Planejamento do Projeto (Roadmap)

O roadmap apresenta as principais etapas planejadas para o desenvolvimento.

1. Estrutura e Organização

- [ ] Organizar o repositório principal.
- [ ] Revisar a estrutura do código original.
- [ ] Documentar os componentes existentes.
- [ ] Organizar o processo de integração.
- [ ] Definir padrões de desenvolvimento.
- [ ] Estabelecer o processo de revisão.

2. Integração com a Engine

- [ ] Revisar a integração com "libGTASA.so".
- [ ] Organizar os pontos de acesso à engine.
- [ ] Melhorar a comunicação entre C++ e a engine.
- [ ] Revisar o gerenciamento de entidades.
- [ ] Aprimorar o tratamento de erros nativos.

3. Sistemas Multiplayer

- [ ] Revisar o sistema de conexão.
- [ ] Melhorar a comunicação cliente-servidor.
- [ ] Aprimorar a sincronização de jogadores.
- [ ] Melhorar a sincronização de veículos.
- [ ] Aprimorar a sincronização de pedestres.
- [ ] Revisar sistemas de combate e animações.

4. Scripts e Funcionalidades

- [ ] Expandir a API Lua.
- [ ] Melhorar o gerenciamento de recursos.
- [ ] Implementar novas funções.
- [ ] Aprimorar o sistema de eventos.
- [ ] Atualizar a documentação técnica.

5. Otimização e Estabilidade

- [ ] Otimizar o código nativo.
- [ ] Melhorar o gerenciamento de memória.
- [ ] Reduzir problemas de desempenho.
- [ ] Melhorar a estabilidade multiplayer.
- [ ] Realizar testes em diferentes dispositivos.
- [ ] Corrigir erros identificados.

---

Compilação do Projeto

O projeto utiliza ferramentas de desenvolvimento Android e compilação nativa.

Requisitos

- Android Studio.
- Android SDK.
- Android NDK.
- CMake.
- Java Development Kit (JDK).
- Git.

As versões específicas das ferramentas deverão acompanhar a configuração efetiva do projeto.

Clonando o Repositório

git clone https://github.com/SEU-USUARIO/mta-sa-android.git

cd mta-sa-android

Compilação

./gradlew assembleDebug

O APK gerado estará disponível no diretório de saída do módulo Android correspondente.

«[!NOTE]
A compilação poderá exigir configurações adicionais relacionadas às bibliotecas nativas e à integração com a engine. Consulte os arquivos de configuração do projeto.»

---

Projeto Original

O desenvolvimento utiliza como referência técnica o projeto original MTA Neon Android.

Repositório original:

https://github.com/samuk190/mta-sa-neon-android

O código original será mantido independente. As modificações desenvolvidas pela equipe serão organizadas em nosso próprio repositório, preservando os créditos e os avisos de licença dos componentes utilizados.

---

Arquitetura de Servidor

O projeto utiliza como referência o ambiente San Andreas Online / MTA Neon.

Repositório do servidor:

https://github.com/Dryxio/san-andreas-online

A compatibilidade será validada conforme a implementação do cliente, os protocolos utilizados e os recursos disponibilizados pelo servidor.

---

Documentação Técnica

A documentação será mantida pela equipe e atualizada conforme o desenvolvimento avançar.

Documento| Descrição
"ARQUITETURA.md"| Organização interna do projeto
"COMPILACAO.md"| Configuração do ambiente
"COMUNICACAO.md"| Arquitetura de comunicação
"SINCRONIZACAO.md"| Sistemas de sincronização
"API_LUA.md"| Funções e compatibilidade Lua
"ROADMAP.md"| Planejamento e progresso

---

Créditos e Agradecimentos

Agradecimentos aos projetos e tecnologias utilizados como referência e base para o desenvolvimento:

- MTA Neon Android: projeto original utilizado como referência técnica.
- Multi Theft Auto: arquitetura multiplayer e ecossistema do MTA.
- San Andreas Online: projeto de servidor relacionado ao ambiente multiplayer.
- Lua: linguagem de scripts.
- Opus: tecnologia de codificação de áudio.
- Rockstar Games / Take-Two Interactive: criadores e detentores dos direitos de Grand Theft Auto: San Andreas.

Todos os créditos, avisos e condições das licenças dos componentes originais deverão ser respeitados.

---

Licença e Informações Legais

Este projeto poderá conter códigos derivados ou adaptados de outros projetos.

A utilização, modificação e redistribuição dos componentes deverão respeitar as respectivas licenças, os avisos de direitos autorais e as condições estabelecidas pelos autores originais.

As marcas registradas e os materiais protegidos pertencem aos seus respectivos proprietários.

---

MTA:SA ANDROID

Cinco desenvolvedores. Um único projeto. Desenvolvimento em equipe.
