# CAMP RPG

Mod independente de RPG para **Minecraft Java Edition 1.20.1 + Minecraft Forge**.

## Objetivo

Adicionar uma camada de RPG ao Minecraft com progressão persistente e compatível com servidores:

- Classes de personagem.
- Atributos e estatísticas derivados.
- Níveis e experiência de personagem.
- Habilidades com custos, recargas e requisitos.
- Equipamentos com atributos e efeitos.
- Interface para consultar personagem e progressão.

## Stack inicial

- Minecraft: 1.20.1
- Forge: 47.3.6
- Java: 17
- Build: Gradle + ForgeGradle 6
- Linguagem principal: Java

Java/Forge é a base escolhida porque o projeto será distribuído como mod independente e precisa de dados persistentes, eventos de combate, sincronização cliente-servidor, registros de itens e uma interface própria. KubeJS/Rhino pode continuar útil para protótipos no modpack, mas não será requisito deste mod.

## Estado

**Fase 0 — estrutura inicial.** Ainda não declarar o mod pronto para jogar ou publicar: é necessário importar o MDK oficial, compilar, testar em cliente e servidor dedicados e criar os sistemas gradualmente.

## Plano de desenvolvimento

1. Inicialização do mod e configuração Gradle.
2. Dados de personagem persistentes e sincronizados.
3. Atributos, experiência e níveis.
4. Seleção de classe e regras de progressão.
5. Habilidades e combate.
6. Equipamentos e modificadores.
7. Interface de personagem e telas de habilidade.
8. Testes em servidor dedicado, documentação e release.

## Ambiente

Instale o **JDK 17** e abra a pasta como projeto Gradle no VS Code (com a extensão Gradle for Java). Use o MDK oficial do Forge para Minecraft 1.20.1 como base dos arquivos do Gradle Wrapper (gradlew, gradlew.bat e gradle/wrapper/).

Quando o wrapper estiver presente:

~~~powershell
.\gradlew.bat genVSCodeRuns
.\gradlew.bat runClient
.\gradlew.bat build
~~~

O JAR de distribuição será gerado em build/libs/.

## Compatibilidade e design

- A lógica autoritativa de personagem e combate deve executar no servidor.
- O cliente recebe dados sincronizados para exibir HUD e telas.
- Evitar dependências obrigatórias de outros mods na primeira versão.
- Não prometer compatibilidade com outros mods até que seja testada.
