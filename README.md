# Prevenção à Fraude — Tabulador de Atendimento

> Ferramenta de **prevenção à fraude** e tabulação de disputas para uma operação de **varejo de grande porte**, com **IA de classificação** e distribuição de casos entre analistas.

![C#](https://img.shields.io/badge/C%23-.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-T--SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![IA](https://img.shields.io/badge/IA-Classificação-0ea5e9?style=flat-square)

> ⚠️ Repositório de **portfólio**: descreve arquitetura e resultados. Não contém código proprietário nem credenciais.

## Resultado de destaque 💰

> **R$ 200.000,00 em prejuízo com fraude evitado** graças à ferramenta de prevenção desenvolvida para a operação.

## O problema

Uma operação de varejo com alto volume de transações precisava **triar rapidamente** casos suspeitos, distribuir a carga entre analistas e padronizar o desfecho de cada atendimento (fraude x desacordo comercial) — reduzindo perdas e acelerando a resposta.

## O que eu construí / evoluí

- **Distribuição de bases entre analistas** — vincular/desvincular casos a partir da lista de usuários liberados, com processamento otimizado no banco.
- **Atendimento Base** — fila dos casos pendentes de cada analista, com critérios de "não finalizado".
- **IA de classificação** — apoio à triagem de **Desacordo Comercial**, acelerando a decisão do analista.
- **Integração com status de agentes (Genesys)** — carga e tratamento dos estados de operação.
- **Visibilidade de menu por perfil** — analista x administrador.

## Destaques de engenharia

- Substituição de `STRING_SPLIT` por _split_ via XML nas _procedures_ de vínculo (compatibilidade e performance).
- Tratamento robusto de dados na carga (durações, _encoding_ UTF-8 com BOM, conversões).
- Controle de acesso por perfil aplicado no menu e nas rotas.

## Stack

| Camada | Tecnologia |
|---|---|
| Back-end | C# · ASP.NET Core MVC |
| Banco | SQL Server · T-SQL · _stored procedures_ |
| Integrações | Genesys · IA de classificação |

## Impacto

Menos perda por fraude (**R$ 200 mil evitados**), triagem mais rápida e distribuição justa de carga entre a equipe.
