# Implementação de Infraestrutura Automatizada com AWS CloudFormation

Durante o laboratório, foram abordados os seguintes pontos:

AWS CloudFormation: Serviço da AWS que permite criar e gerenciar recursos na nuvem através de templates. Cada template descreve os recursos desejados (como EC2, S3, Security Groups, VPCs) de forma declarativa, funcionando como documentação viva da infraestrutura.

Benefícios do CloudFormation:

Automação completa: Criação e destruição de ambientes sem configuração manual.

Reprodutibilidade: É possível replicar a mesma infraestrutura em múltiplas regiões ou contas.

Padronização e segurança: Aplicação consistente de regras de segurança, como Stacks de firewall, evitando erros humanos.

Documentação automática: Os templates descrevem todos os recursos e suas configurações.

Formatos de criação de templates: Foi possível trabalhar com JSON e YAML, entendendo as vantagens de cada formato. Por exemplo, YAML é mais legível e compacto, enquanto JSON é amplamente compatível com scripts e APIs.

Acesso ao console do CloudFormation: Aprendemos a criar Stacks diretamente pelo console, selecionando templates pré-existentes ou fazendo upload de nossos próprios arquivos. Foi possível acompanhar o progresso de criação dos recursos, identificar erros e revisar logs detalhados de provisionamento.

Diferenças em relação ao Terraform:

CloudFormation é totalmente integrado à AWS, enquanto Terraform é multi-cloud.

CloudFormation gerencia dependências de recursos automaticamente dentro da AWS.

Terraform oferece maior flexibilidade para ambientes híbridos ou multi-cloud, mas pode exigir scripts adicionais para integração.

# anotações de estudo

Sempre validar templates antes de criar Stacks para evitar falhas de provisionamento.

Usar outputs para expor informações importantes da infraestrutura (IPs, ARNs, nomes de buckets).

Agrupar recursos relacionados em um único template facilita manutenção e padronização.

Versionar templates no GitHub garante rastreabilidade e permite replicar a infraestrutura de forma confiável.

Parametrizar recursos com Parameters aumenta flexibilidade e reduz duplicação de código.
