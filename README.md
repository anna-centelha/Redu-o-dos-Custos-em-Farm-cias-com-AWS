# SOLUÇÃO AWS PARA REDUÇÃO DE CUSTOS OPERACIONAIS EM FARMÁCIAS

**Data:** 11 de Agosto de 2025

**Empresa:** Abstergo Industries

**Responsável:** Anna Carolina Centelha

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Anna Carolina Centelha. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos e aumentar a eficiência operacional da infraestrutura de TI.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma focada em uma área de otimização: computação, armazenamento e banco de dados. A seguir, serão descritas as etapas do projeto:

### Etapa 1
* **Nome da ferramenta:** AWS Auto Scaling
* **Foco da ferramenta:** Otimização de custos e elasticidade da infraestrutura de computação.
* **Descrição de caso de uso:** A Abstergo Industries possui aplicações com picos de demanda variáveis, como portais internos com maior acesso no início e fim do mês, e sistemas voltados ao cliente com tráfego imprevisível. Atualmente, a empresa mantém servidores (instâncias EC2) superprovisionados para suportar esses picos, o que gera custos elevados com recursos ociosos na maior parte do tempo. Com o AWS Auto Scaling, a infraestrutura se ajustará dinamicamente: novas instâncias serão adicionadas automaticamente durante picos de demanda para garantir a performance e, da mesma forma, serão removidas quando o tráfego diminuir.

    🔽 **Redução de custos:** Eliminação de gastos com capacidade computacional ociosa, pagando apenas pelos recursos efetivamente consumidos.
    
    🔼 **Principal ganho:** Alta disponibilidade e performance consistente para as aplicações, melhorando a experiência do usuário sem necessidade de intervenção manual da equipe.

### Etapa 2
* **Nome da ferramenta:** Amazon S3 Intelligent-Tiering
* **Foco da ferramenta:** Automação da economia de custos de armazenamento de objetos.
* **Descrição de caso de uso:** A empresa armazena um volume massivo de dados no Amazon S3, incluindo backups, logs de aplicação, documentos corporativos e arquivos de mídia. O padrão de acesso a esses dados muda com o tempo: são acessados frequentemente no início e raramente após alguns meses. A gestão manual do ciclo de vida para mover esses dados para camadas de armazenamento mais baratas é complexa e raramente executada. O S3 Intelligent-Tiering automatiza esse processo, monitorando os padrões de acesso e movendo os objetos entre camadas de acesso frequente e infrequente, gerando economia sem impacto na performance e sem sobrecarga operacional.

    🔽 **Redução de custos:** Economia automática e significativa na fatura do Amazon S3, sem a necessidade de análises manuais ou da criação de políticas de ciclo de vida complexas.
    
    🔼 **Principal ganho:** Gestão de armazenamento simplificada e otimização de custos contínua, liberando a equipe de TI para focar em atividades estratégicas.

### Etapa 3
* **Nome da ferramenta:** Amazon Aurora Serverless v2
* **Foco da ferramenta:** Banco de dados relacional sob demanda com escalonamento automático.
* **Descrição de caso de uso:** A Abstergo mantém diversos bancos de dados para aplicações com cargas de trabalho intermitentes ou imprevisíveis, como ambientes de desenvolvimento, ferramentas de análise interna e sites com tráfego esporádico. Manter instâncias de banco de dados (RDS) provisionadas para esses cenários é ineficiente e caro, pois a capacidade fica ociosa na maior parte do tempo. Ao migrar para o Aurora Serverless v2, o banco de dados escalará a capacidade de forma instantânea e granular de acordo com a demanda da aplicação, podendo escalar para uma capacidade mínima muito baixa durante períodos de inatividade.

    🔽 **Redução de custos:** Eliminação de custos com capacidade de banco de dados ociosa. A cobrança é baseada na capacidade consumida, representando uma economia de até 90% para cargas de trabalho variáveis.
    
    🔼 **Principal ganho:** Obtenção de um banco de dados de alta performance que se ajusta a qualquer tipo de carga de trabalho, desde as mais imprevisíveis até as mais exigentes, sem a necessidade de provisionamento manual.

## Conclusão
A implementação de ferramentas na empresa **Abstergo Industries** tem como esperado **a criação de uma infraestrutura de nuvem mais inteligente, elástica e financeiramente eficiente**. A adoção combinada do AWS Auto Scaling, S3 Intelligent-Tiering e Amazon Aurora Serverless v2 permitirá que a empresa responda dinamicamente às demandas de negócio, garantindo performance e disponibilidade enquanto reduz drasticamente os custos operacionais com recursos ociosos. Isso aumentará a eficiência e a produtividade da empresa, permitindo que a equipe de tecnologia se concentre em inovação em vez de gerenciamento de infraestrutura.

Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos
* [Documentação do AWS Auto Scaling](https://aws.amazon.com/pt/autoscaling/)
* [Documentação do Amazon S3 Intelligent-Tiering](https://aws.amazon.com/pt/s3/storage-classes/intelligent-tiering/)
* [Documentação do Amazon Aurora Serverless](https://aws.amazon.com/pt/rds/aurora/serverless/)

---

## Assinatura do Responsável pelo Projeto
**Anna Carolina Centelha**
