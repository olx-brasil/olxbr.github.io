# Cultura DevOps: Direitos e Deveres.

O que DevOps? Cultura, pessoa ou papel?

![DevOps](img/devops.png)

Pela imagem extraída da Wiki, fica muito simples entender visualmente: https://en.wikipedia.org/wiki/DevOps

Mas em todos os lugares que lemos ainda não fica bem claro o que é um DevOps, então, usando a técnica da matemática da negação, para entender o que é DevOps é mais fácil entender o que **DevOps NÃO É**:

* DevOps não é: Um desenvolvedor high skilled em infra e high skilled em QA;
* DevOps não é: Um cara de infra  high skilled em desenvolvimento e em QA;
* DevOps não é: Um cara de QA  high skilled em Infra e em desenvolvimento.

Então,  se não é um super dev, super qa ou super infra, entende-se que qualquer dev, qualquer qa e qualquer infra pode ser considerado DevOps ? A resposta está correta!

**Por tanto, DevOps não é uma pessoa e sim um papel que pode ser adicionado à um Dev ou Qa, ou Infra. Em um time, pode haver então uma única pessoa com essa característica ou todo o time.**


## Por que um time precisa entrar na cultura DevOps.

![DevOps](img/devopsman.png)


Quais são as reais necessidades do time quando se pensa em pedir ajuda para infra ?

1. Acesso ao ambiente de produção para puxar logs e realizar depurações
2. Auxílio em configurar/manter as ferramentas de monitoramento
3. Auxílio em configurar/manter os processos de deploy em produção
4. Configurar um novo recurso de infraestrutura para subir um novo deploy.
5. Auxílio em configurar controle de versão ou garantir o bom funcionamento deste controle.

Essas tarefas são simples e plausíveis de serem replicados para dentro dos times, ou seja,  é muito fácil treinar os desenvolvedores a realizarem estas 5 tarefas no dia a dia, gerando total dinamismo e velocidade.

A cultura DevOps permite você escolher um candidato com mais musculatura ops, ou dev ou qa, isso conforme os gaps existente nos times mas em linhas  gerais, todos serão DevOps.

## Então não precisamos ter um DevOps dedicado?

---
**Todos os membros dos times, sem exceção, pode ser um DevOps!** O que ocorre é uma fase de transição, onde não existe ainda um alicerce em infra-estrutura para proteger os times (deles mesmos) de impactos ocasionado pela nova filosofia de trabalho. Do outro lado, há ainda a necessidade dos times de desenvolvimento aprender as novas ferramentas que compõe o papel de um DevOps.
---


Logicamente, durante a transmissão entre uma cultura tradicional e DevOps, há a necessidade de um plano de ação transitório e naturalmente, é normal em a cultura tradicional, toda a parte operacional esteja em infraestrutura.

Então, em um processo trânsito, infraestrutura possui a missão de auxiliar os desenvolvedores a entender as ferramentas e atividades operacionais necessária para que o time absorva a cultura DevOps e recebam total ownership do ambiente.

O recurso de infra tentará participar das cerimônias dos times sempre que possível mas sua principal atribuição será suportar e treinar o time em ser auto suficiente através da cultura DevOps.

Uma vez que o time absorveu por completo toda a cultura DevOps, não há mais a necessidade de infraestrutura fornecer um indivíduo auxiliador com características Ops.


Ops = IT operator, é a parte infra da nomenclature DevOps.


## Um Ops dedicado responde para quem Infra ou Dev?

Entretanto, pode-se chegar a conclusão por questões de negócio (ou outro motivo especial) o time de fato necessite de Ops(removido o Dev propositalmente) dedicado permanente.

Em casos assim, o papel OPS soma-se igualmente na relevância técnica da composição do time, motivo evidente para que o gestor use de seu head-count a fim de contratar este recurso.

Exemplos de casos especiais: stacks como Data Store(NoSQL, SQL, Search Engine) ou qualquer outra stack de atenção no qual um desenvolvedor não conseguiria se aprofundar usando sua musculatura ops e que faça sentido ao time ter alguém especializado.

Todavia, pela característica de similaridade com infra e total sinergia, esse membro Ops do time receberá coaching técnico do time de infra. Pensando em analogia ao modelo de Squad seria o conceito de Guild.


## Na cultura DevOps pode-se fazer tudo no ambiente, já que se tem acesso a tudo ?

Uma boa analogia para definir limites é pensar exatamente como um prédio:

![Visinhos](img/predio.png)

Mesmo comprando um apartamento que custou milhões de Reais, não podemos simplesmente ir estacionando o carro em qualquer lugar, mudar a fachada de nossa varanda, muito menos impedir outros moradores de usar o elevador. Em um prédio há o síndico e sua equipe que tem como responsabilidade a  segurança, organização e manutenção da área comum!

Como dono do apartamento, podemos quebrar paredes para ampliar um espaço em especial, mudar a decoração, dormir o dia todo ou ficar sempre acordado mas não podemos criar uma nova entrada para o apartamento que force o vizinho a tomar medidas por causa disso. Deve-se tomar cuidado com a palavra AUTONOMIA DA STACK!

Na cultura DevOps não pode fugir do escopo do time, deve pensar que criar uma VPC pode abrir um problema de comunicação entre VPN e VPC entre o escritório e outros times (usando a analogia AWS). Desta maneira, o time tem acesso a sua infraestrutura mas suas ações não podem impactar algumas diretrizes.

Os times no contexto DevOps devem ser responsáveis por manter o ambiente documentado, para isso existem algumas ferramentas com o [gliffy.com](https://www.gliffy.com/) que permite desenho colaborativo.

O escopo DevOps é unicamente o próprio time:
* Garantir a comunicação e alinhamento entre as áreas em nível horizontal (uso do Slack).
* Cultura “Você fez, você cuida."
* Documentação da stack.
* Atuação em questões de infraestrutura e Qualidade/Automação.
* Garantir automações que melhorem a qualidade do lifecycle.
* Garantir o bom uso dos recursos computacionais do time
* Garantir que todo o time se comuniquem de forma documentada, por exemplo, incentivando o time a detalhar situações em ferramentas como Slack.

Sendo assim, desenvolvedores DevOps devem ter uma interação muito grande com todos: Infra, QA e os demais Devs de outros times para conseguir atingir os objetivos.

Mais adiante será exposto em duas sessões o que dentro da cultura DevOps **poderá** e **não poderá** fazer.

## Então, qual seria o papel de Infra-estrutura.

Exatamente como na analogia do síndico e sua equipe, a OLX vem se dedicando em **garantir que as equipe possam desenvolver suas características em velocidade rápida sem risco de ser bloquear outras equipes (MISSÃO)**.

O Síndico geralmente tem um apartamento no prédio mas mesmo ele precisa seguir as mesmas regras para que tudo funcione perfeitamente.

Para conseguir criar os alicerces necessários à  autonomia dos times, todos os três cases possuem em seus respectivos time infraestrutura a cultura DevOps ao ponto de possuir desenvolvedores backend/frontend e BigData Engineers.

O papel desses times passaram de ser operacional para gerarem soluções que garantam a segurança, autonomia e harmonia técnica entre os times que geram os produtos.

## Cloud Engineering

O time responsável dentro da OLX por essa gestão chama-se Cloud Engineering.

Um Cloud Engineer, é responsável por desenhar as soluções em parceria com os times de desenvolvimento para garantir boas práticas aos novos ambientes necessários. Essa parceria deve garantir sempre um Win-Win.

O escopo do cloud engineer atinge todos os times da engenharia/produto de software (cross):
* Responsável juntamente com um especialista em segurança da informação das questões práticas de segurança.
* Responsável sobre a infraestrutura base dos times
* Responsável sobre  CDN e WAF dos times
* Responsável sobre os DNSs externos dos times.
* Auxílio na resolução de problemas e documentação da stack dos times de tecnologia.
* Responsável sobre os pontos de convergência inter-times, como banco de dados monolito.

Mas, dentro da cultura DevOps os times não deveriam resolver os problemas sozinhos ?

```Sim, porém,  lembrando que alguns problemas envolve um grau de conhecimento muito especialista impensável para a definição do que é um DevOps, para esse caso, o Cloud-Engineer é um segundo nível, sendo o primeiro nível o próprio time.
```

## Sendo prático, o que dentro de cultura DevOps os times não deve/conseguiram fazer sozinho.

**Alterar configurações de rede: VPC e  security group Group(AWS ou equivalente em outra Cloud).**

Essas configurações devem ser realizadas em parceria com o time de Cloud em função de serem configurações que impactam a segurança da empresa como um todo e os scripts que automatizam os controles da Cloud criados pelos Cloud Engineers.

**Desligar ou reiniciar serviços, instâncias de outros times.**

Os DevOps poderão reiniciar, desligar e dar terminate nos recursos computacionais do próprio time, terão total autonomia para isso mas não deverão realizar esse procedimento na stack do outro time mesmo que a causa raiz de um dado problema seja um mal funcionamento em um serviço deste dado time. Para casos assim, deve-se envolver os DevOps do dado time para que haja essas ações.

**Criar sozinho máquinas cuja o custo seja maior que U$ 0.30 hora.**

A iniciativa  é o envolver diretamente um Cloud Engineer para avaliar alternativas como por exemplo, a utilização de escalamento horizontal utilizando máquinas mais baratas e por consequência, um Double check a fim de validar a real necessidade do recursos computacionais de preço expressivo.

**Levantar instância computacionais fora do padrão.**

Há algumas precisas para que uma instância computacional seja legível estar em operação no ambiente e fora destes padrões:

* Deve possuir tags de identificação
* Deve utilizar as credenciais de acesso SSH adequado ao time (pem key do time já pré, existe).
* Deve ser instâncias levantada dentro da rede (VPC em analogia AWS) do time.

Esses padrões servem para a segurança e uniformidade da tecnologia. Instâncias fora destes requisitos terão tempo de vida máxima de 30 minutos no ambiente.

**Criação de novos logins  / usuários ou roles.**

Todos os objetos que se referem a segurança, são pontos de gestão cross-team e necessita de uma gestão unificada.

## Sendo prático, o que os times deveriam/conseguiriam fazer sozinhos.

Qualquer coisa que não esteja listado no tópico anterior 😄.
