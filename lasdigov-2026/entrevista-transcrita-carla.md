**Giovanna Barbosa**

Eu quero entender como que é o processo, né? Como que foi o processo de desenvolvimento do Brasil Participativo e tudo mais. Meu objetivo, talvez, e no futuro seria talvez generalizar um processo de adoção de software livre dentro da administração pública, de forma que seja fácil para qualquer departamento de TI. Em qualquer parte, em qualquer esfera governamental, eu posso pegar aquele processo, tipo...

**Carla Aguiar**

Então, eu vou até te falar, vou até te adiantar, porque eu pedi para o Paulo escrever um livro sobre isso, o Paulo Meirelles. Aí ele tá escrevendo sobre, já vou falar um, pode ir começando falando?

**Giovanna Barbosa**

Pode falar, eu tô gravando já. Ah, então,

**Carla Aguiar**

beleza. Então, assim, é porque qual é a lógica, por exemplo, do software livre comum, né? Você faz seu fork, assign um eixo, abre um pull request, a comunidade que vão ter os mantenedores, vão ver se tá alinhado a um roadmap, vai aceitar ou não e vai te dar feedback, né? E aí, esse é o a maioria adota e tem os esquisitos, tipo o Linux, que você tem que mandar um patch para um e-mail, tarará, tarará. Então, a gente, a gente como laboratório, a gente como quem contribui para a software livre educacional, que é o meu universo, estava acostumado com essa lógica de abrir PR e mandar, né, e aí, o Brasil participativo, quando a gente pegou o Brasil participativo, foi muito atropelado, a gente colocou ele em produção em um mês, a gente não teve muito onboarding, e depois desse um mês, já veio essa pressão,

**Carla Aguiar**

porque a primeira versão dele a gente colocou via snippet, então se você sobrescrevia um HTML e um CSS em cima de uma página para ficar bonito, mas por trás dos panos, originalmente estava o código Decidim puro, raiz, aí tinha essa necessidade de customizar o Decidim para o Brasil participativo, né. E aí a gente foi, como teve o PPA, que foi a maior experiência da história do Decidim, a maior experiência de participação do Brasil e do mundo digital, isso gerou, abriu portas, a gente tem uma relação com a galera do Decidim, uma relação política e teoricamente técnica, e a gente falou, beleza, e isso vamos contribuir para o Decidim, né, que essa foi a nossa visão ingênua. E aí, já com pressão de trazer a nacionalização, que é trazer com a visão, com o GovBR, mudar alguns tipos de processos, né, assim, um exemplo bem típico, conferência,

**Carla Aguiar**

né, o Decidim tem um módulo chamado Conference, e aí, o Conferência para o gringo, né, é como se fosse uma conferência de pesquisa, que é um evento, eventão, que você faz, se inscreve, tem trilhas, tem agenda, tarará. Conferência para o brasileiro, politicamente, as conferências nacionais, é um processo participativo, começa no município, estado, nacional, e aí tem vários momentos de participação nesse centro. Então, assim, só o conference não, metodologicamente, não conversa, o que é o decidinho que a gente como conferência no Brasil. Então, a gente tinha que fazer essa adaptação. Localização das metodologias de participação, né, então teve essa pressão para fazer ao mesmo tempo, que a gente estava aprendendo como é que funcionava o módulo,

**Carla Aguiar**

então a gente entendeu que era a arquitetura do Decidim é a arquitetura orientada a plugins, né, então você vai colocando os plugins ali, mas é o monolito de Rails que você tem que ficar, a gente ficava, aí o que a gente fez? A gente ficou sobrescrevendo a interface ali, para, por exemplo, colocar o GovBR, da forma como a gente conhecia, né? E a gente não conseguia emplacar por request, a gente abria por request, ou ele não era avaliado, ou era recusado, e o próprio mantenedor ia lá e copiava o código como estava na main, né? Ou eu, mantenedor, que é um cara lá que mantém o decidindo. E aí amadurecendo, né, indo para o Decide e Fecha, a gente entendeu como que, aí eu acho que é onde eu quero chegar, que é o modelo tecnopolítico de contribuição para software livre, né, que não é a lógica do software livre tradicional, porque a decisão não é técnica, ela é política. O que entra e o que não entra ali na plataforma. Então, essa lógica de request não funciona.

**Carla Aguiar**

Por exemplo, como com o Decidim, você contribui com o Decidim? Primeiro, você faz o seu módulo, você faz o seu plugin no seu repositório para o seu trabalho, né? Então, assim, tem dois protagonistas que tem, que é o pessoal da França e da Suíça, né? E que eles fazem porque eles vendem o serviço de oferecimento.

**Carla Aguiar**

Aí você faz o plugin. Beleza, por exemplo, o plugin do Hadrien lá, deixa eu ver o que foi legal dele. Ah, de geolocalizar tudo que tem na plataforma. Aí ele fez isso para atender um cliente. Aí ele faz bonitinho o documento, o tutorial, tarará. E aí no comitê do Decidim, que é um grande comitê, que participa todo mundo que faz parte lá do grupo do Decidim, que você paga uma taxa lá e participa. eles eles decidem o que entra para o core ou não então, vamos dizer, se por request não acontece via por request, é via plugin, então assim o que o pessoal comemora meu plugin foi incorporado ao core do Decidim mas é o plugin já com a visão política clara com a visão metodológica clara e já validada em algum contexto E aí depois isso volta pro decidir. Então a gente demorou pra entender isso, né? Pra entender essa jornada. Aí, por exemplo,

**Carla Aguiar**

Hoje um dos grandes gargalos que o pessoal decide mais reclama é o texto participativo. Que ele é implementado de forma super elegante, mas não é performático, assim. O texto participativo é aquele comentário por parágrafo.

**Giovanna Barbosa**

Sei, sei.

**Carla Aguiar**

Que tem zero usabilidade e não tem performance. E aí no Brasil, fudeu. a gente precisava dos dois, assim, e agora a gente teve, por exemplo, do da carteira de motorista, né, de que teve essa proposta do CNH, então passou na plataforma, e a plataforma quebrou várias vezes, porque não aguentava, porque tiveram 25 mil comentários, que também foi o maior comentário para o Pará, da história do Decidim do mundo, mas a gente praticamente reescreveu todo esse componente, mas assim, mesmo sendo uma necessidade de todo mundo, para ser aceito a gente tem que passar por esse processo, né, de fazer o plugin, publicar e fazer a propaganda lá para esse grande grupo, para querer ter ele dentro do dentro do ecossistema, e eu acho que esse processo é muito, até no próprio lá, na documentação desse disso, não é evidente,

**Carla Aguiar**

Isso são as pessoas que trabalham que sabem e como é muito distante de um software livre normal, assim normal no sentido do padrão de software livre, tem uma barreira muito grande. A gente até hoje não tem nenhum plugin nosso aceito, depois de três anos de projeto. Assim, eles pegaram parte do código que a gente faz, mas assim, apesar da gente ter feito várias contribuições, de performance e melhoria de usabilidade, a nossa contribuição nunca, até hoje, nunca foi para o core, porque a gente nunca teve energia, né, de organizar para fazer esse processo todo, né. Então, é assim, aí eu acho que isso, pensando nesse grande escopo, né, de softwares tecnopolíticos, essa capacitação de como contribuir com softwares tecnopolíticos, para mim, tem sido um grande aprendizado. E nesse processo de grande aprendizado tem muita frustração, né, de você falar, nossa, tá arrasando, vou lá contribuir com decidinho. Ah, não, só que não. Pera aí, que eu não vou aceitar sua contribuição, porque não é assim, não.

**Giovanna Barbosa**

Exige um certo capital social ali, pra você adentrar. Eu falo assim, uma confiança. Então. Ser introduzido, participar de certas coisas.

**Carla Aguiar**

É, exatamente. É um capital social e político, né? Porque a tua ideia política tem que ser validada e tida como prioritária para todo mundo. E as pequenas correções, mesmo as pequenas correções, eles não aceitam PRs. Assim, do dia a dia é muito difícil eles aceitarem. O que eu ouvi várias vezes, ah, não, eu abri o PR, ele fechou meu PR, mas ele copiou meu código e colocou lá.

**Giovanna Barbosa**

Outra coisa que quero saber: estou fazendo um recorte especificamente do Brasil Participativo. Eu quero entender essa caminhada e parte do que você falou faz parte dessa caminhada de como o Brasil Participativo se entende como parte desse ecossistema. Você sente que quais experiências profissionais suas ou de software livre tiveram uma grande influência pra você conseguir desbravar esse mundo do Decidim, o ecossistema essas imposições, barreiras essa conversa esse ganho de confiança como que foram suas experiências passadas com software livre na administração pública e como foi essa e o que que torne essa tão distinta. Você já falou algumas coisas, mas eu quero enquadrar melhor.

**Carla Aguiar**

Ah, excelente. Então, assim, lá em 2017, sei lá, a gente fez o chatbot, né, que foi um dos primeiros chatbots...

**Giovanna Barbosa**

Eu lembro de... Eu acho que eu lembro de ver, quando o Nitai fez uma reunião dos laboratórios, eu lembro do chatbot que tá lá.

**Carla Aguiar**

E aí foi um dos primeiros chatbots que foi 100% linguagem natural, foi na época do chat GPT-2, que ainda rodava na tua máquina, você baixava e testava ela, o chat GPT-2 no terminal. Então, assim, para o governo, era super novidade, estava tendo muito debate sobre o uso e adoção, porque tinha uma barreira muito grande e de usar a linguagem natural ao invés de botão, que era aquela norma do momento. O nosso foi o primeiro que foi usado linguagem natural no governo. Mas qual foi o software livre que a gente decidiu, na época, a gente foi e usou o Rasa, mas o Rasa é um software livre comercial, é um software livre que é, não é específico de governo, então tem uma lógica de software livre normal, então a gente ia lá, havia problema, melhorava, abria o prequest, tudo certo, mas a gente tinha um certo distanciamento da comunidade,

**Carla Aguiar**

eles sabiam quem era a gente, eles ainda eram startup, mas a gente não tinha relação de nada com eles, assim, não tinha uma relação de funcionalidade, teve muita coisa que era específico do Mink, que era específico nosso, que a gente contribui, fez para o nosso caso, e depois o Rasa fez a solução, por exemplo, arquiteturalmente. O Rasa era um monolito, o pipeline era código e modelo no mesmo pipeline, então se eu mudasse uma linha de código, eu tinha que retreinar todo o meu modelo, então isso computacionalmente era muito caro, Então a gente separou arquiteturalmente o próprio Rasa para ter um fluxo de dados, de treinamento, de machine learning, um outro de código, e aí deu, sei lá, uns seis, oito meses, eles lançaram uma versão também com esse desacoplamento.

**Carla Aguiar**

Mas aí a falta dessa comunicação Dessa relação entre A gente e eles Teve muito, aconteceu muito Isso, de a gente fazer alguma coisa que era Importante para a gente e eles depois Se aplicarem, fazerem Porque era necessidade da comunidade Mas a gente estava muito, como De novo, era um comercial, a gente estava mais Preocupado em resolver o problema do Ministério da Cultura Porque a gente entendia que Era um produto que Usava software livre E o produto eram, vamos dizer, a gente sabia que era uma nacionalização daquele software livre, então a gente se preocupava em documentar internamente, que era mostrar para a esfera federal como fazer um chatbot em língua portuguesa, que foi algo que a gente teve que aprender também na raça, e aí a gente trouxe isso para dentro só do nosso fork, então,

**Carla Aguiar**

e virou referência para muito trabalho que veio em seguir, né, assim, Uma coisa legal que a gente teve uma reunião esses dias com o Serpro sobre o uso do WhatsApp, da comunicação, e eles falaram que eles usavam a arquitetura e a estrutura que a gente propôs lá atrás hoje, né, que eles se basearam na gente para propor a solução deles. Então, assim, o que ficou de legado foi muito mais o aprendizado, mas a nossa preocupação nunca foi integrar com o Rasa, sempre foi nacionalizar uma solução de software livre para o problema governamental daquele momento. E aí eu acho que, assim, e aí agora a gente viu que, aí a gente já, no Decidim, a gente já entendeu que a gente precisa, como é um tecnopolítico, o Decidim, ele é tecnopolítico, ele não é um software comercial, assim, no sentido, ele não tem a lógica comercial, né,

**Carla Aguiar**

então a gente sentiu desde o começo a necessidade de aproximar da comunidade deles, pelo menos de forma institucional, né, então isso ajudou, assim, entender que o Brasil participativo, a gente precisa, e a gente precisava trazer para o Brasil essa mesma lógica de capacitar, de ter algo que pudesse fomentar dentro da esfera de governo, o uso de plataforma de participação, né, mas ao mesmo tempo a gente sabe que por ser tecnopolítico junto, a comunidade soft-leave é mais forte, que eu acho que é isso que é o diferente, né, no do Rasa, a gente ter relação ou não com eles não impactava o projeto, porque a gente não era um player importante para eles, ao decidir que é tecnopolítico, a gente é um player importante dentro do ecossistema. Não sei se eu respondi a tua pergunta.

**Giovanna Barbosa**
Eu preciso olhar qual que é o modelo de financiamento do Rasa. Porque eu estou vendo algumas distinções aqui, né? Você estava falando que o Rasa tem uma pegada muito comercial.

**Carla Aguiar**

É. E aí, hoje, ele começou como bem software livre, aí agora ele está naquela lógica de Apache. Tipo assim, o core dele é software livre, mas para você fazer um chatbot de forma com boa usabilidade, tem uma plataforma que aí é fechada.

**Giovanna Barbosa**

Tipo, acho que o Rocket Chat também. É. Acho que o Zulip ainda não. Acho que o Zulip ainda não, Bitwarden também tem umas coisas nesse sentido também/

**Carla Aguiar**

Assim, o Rasa começou muito aberto e foi entrando nesse modelo comercial de software livre. Já o Decidim...

**Giovanna Barbosa**

Você falou que ele tem um um arcabouço Que cuida da... Direitos autorais, trademarks, etc. O que é? É uma organização?

**Carla Aguiar**

Tem a estrutura organizacional. Tem esse Andréas, que é o mantenedor. O time deles é bem pequeno, que é esse Andréas, tem mais uns dois desenvolvedores, tem uma PO, que é a Carol, que fica olhando ali os roadmaps, né? E aí eles têm um comitê gestor, que aí eu faço até parte dele. É um comitê que é eleito pela comunidade, e aí essa questão de trademark, toda a parte legal do Decidim, decidido por esse comitê. Assim, por exemplo, agora o pessoal da Suíça pediu para fazer um chapter local do Decidim na Suíça. Decidim Association. É, Association, essa mesmo. Aí, por exemplo, o mais novo foi o pessoal, o Adrian lá, querendo trazer um chapter do Decidim para a Suíça, para ele conseguir entrar em edital público, né, que precisa ter uma associação nacional. Então, tem essa questão para ele, ele não pode,

**Carla Aguiar**

ele não queria colocar ele como associação lá dele, ele queria colocar decidim. E aí, para isso, teve uma conversa de mais de um ano, dentro dessa associação, com esse comitê, para fazer um estatuto de trademark, tarará, tarará, e agora foi aprovado.

**Giovanna Barbosa**

Primeiro era de controle do conselho da cidade de Barcelona e depois foi transferido para a associação.

**Carla Aguiar**

Então, tem associação e dentro da associação tem esse comitê de coordenação. O nome do comitê de coordenação. Que aí é essa galera eue decide. E aí tem outra estrutura também, estou entrando aqui nos grupos Telegram, que eu vejo. Aí tem direção executiva. Aí tem essa estrutura que gere institucionalmente a organização Decidim. E gera esses fundos que vão para lá, que mantém, que os fundos que eles têm é basicamente da prefeitura de Barcelona e alguns outros pequenos, assim, digitais, mas a maioria é do governo.

**Giovanna Barbosa**

Como que o Decidim entra na história do governo federal? De onde surge a ideia de criar o Brasil Participativo? Eu sei que havia outra plataforma.

**Carla Aguiar**

Tem o Participa Mais, né? E aí, na época, acho que você traduziu o dinheiro público, o código público, e lá, se você ver, tem várias falas desse dinheiro.

**Giovanna Barbosa**

Sim, eu lembro.

**Carla Aguiar**

Não, mas então, é nisso que nasce a semente Decidim. Porque a decisão do Decidim foi do comitê que você já conhece, que é Nitai, Poppi e a assessora da ministra, que é a, esqueci o nome dela, Miriam Chaves. Aí, politicamente, são essas três pessoas que falam, a gente precisa trazer esse framework Decidim, que já tinha esse histórico de software livre, de participação social forte, né, então era mais trazer isso, trazer essa cultura também aqui no Brasil, que era, que era, antes do Decidim era o quê? Esqueci, aquele de Madri. É que antes tinha, a história do Decidim é essa, né, vem essa história de Madri, que era só, acho que eu sei o que eu ponço, é, e aí o Poppi conhece essa galera do consul, tal, aí o Consul vira decidim, e aí já tem essa essa ideia, e quando muda o Lula 3, o Poppi é chamado pra ser o diretor de participação digital.

**Carla Aguiar**

Aí ele não aceita, ele indica a Laila, mas ele já indica a Laila já com essa visão de adoção de Decidim, já desenhado, já amadurecido, do que eles querem politicamente. Eu acho que aí essa parte de como isso foi feito vai ser o Pop que vai te falar. Que é dele.

**Giovanna Barbosa**

Lá em 2019, com a tradução lá daquela campanha do dinheiro público, código público, começam essas discussões de trazer essa forma de participação social atrelada ao software livre.

**Carla Aguiar**

Isso. É, porque o Poppi vai pra lá, que lá tem, tem um, em Madrid tinha um evento anual de softwares tecnopolíticos, depois ele vai te falar, e aí ele vai, e lá ele conhece o Polis, que aí depois, a partir do Polis, ele melhora e vira o EJ [Empurrando Juntas], e lá é a galera do Consul que pagava esse evento, então também aí tem todo esse histórico que não foi de um dia para o outro, foi construído mesmo.

**Giovanna Barbosa**

O Nitai me falou Uma das coisas mais marcantes Que eu tive na conversa com ele foi Ah, a gente tinha Iniciativas como software público. Tinha os repositórios de software público. Foi criado em 2007. Mas essas iniciativas, elas não ganharam aderência. Ele me passou a impressão de que tudo é muito pontual; a adoção de software livre ou a promoção de software livre ela é centralizada em certos indivíduos que são alinhados com os valores de software livre, mas isso não é uma política transversal dentro da administração pública. Então é uma pessoa ou um grupo de pessoas pequeno tem essa ideia e ela impulsiona essas iniciativas da melhor forma possível... Mas que isso não implaca ainda como uma política que torna o software livre a escolha lógica dentro da administração pública.

**Giovanna Barbosa**

Tem coisa tipo projeto de lei para alterar a lei da informática, para que preconize que o software livre... Mas, na prática, parece mais o impulsionamento de certas pessoas, certas gerações de profissionais dentro do governo. Ou nas adjacências do governo.

**Carla Aguiar**

Isso. É isso, por exemplo, uma coisa que a gente estava brigando desde o ano passado, o desenho do projeto é pensar numa estratégia de que se mudar de governo, a plataforma não cai. Então, isso é um trabalho porque a gente sabe que não é institucional, não é política de Estado, é política de governo. Das pessoas que estão ali naquele momento. Então, isso é verdade, mas hoje, eu acho que não sei se traz para o software livre, mas hoje, assim, uma conversa que está muito forte por causa da IA e de soberania sim.

**Carla Aguiar**

mas olha qual o problema eu vou te falar a soberania é muito distorcida por exemplo, a soberania, se você perguntar para uma pessoa do Serpro hoje eu vi essa conversa para ele, é soberano pagar milhões e milhões, sei lá, bilhões para a OpenAI para ele colocar um modelo da OpenAI na infraestrutura brasileira. Tipo assim, para o modelo ficar em grandes servidores da CEPRO e eu garantir que aquele dado nosso brasileiro não vai sair. Mas para ele isso é soberania.

**Giovanna Barbosa**

A conversa na União Europeia está completamente diferente.

**Carla Aguiar**

Então, aí...

**Giovanna Barbosa**

Isso foi interessante. Eu fui...

**Carla Aguiar**

Ele voltou, assim, profundamente.

**Giovanna Barbosa**

Eu fui para Berlim há poucos meses depois da eleição do Trump. Então, imagina o alvoroso que foi naquela, que era um pós-backstage, tinha um monte de gente da União Europeia lá falando sobre a implementação do software livre dentro da União Europeia como um todo, tinha o governo da França, Alemanha também, o departamento de Munique, inclusive é patrocinador desse evento, e estava o maior alvoroso, por quê? a União Europeia altamente dependendo da Microsoft, altamente dependendo de um bilhão de fornecedores nos Estados Unidos, e os Estados Unidos se tornou um agente hostil.

**Carla Aguiar**

Exato. É isso, quando você pensa agora que ele falou, a stack toda é privada, você tem NVIDIA, você não faz IA sem NVIDIA, sim, né? A maioria dos players, e aí você tem a nível de software, assim, e eu acho um absurdo, a gente sabe, uma vez que você contrata uma empresa de TI para o Estado, você cria um grande loquinho, é muito caro fazer migração, é muito caro, assim, então, assim, é uma decisão que eu acho sempre negligenciada, assim, mas aqui no Brasil eu acho que ainda não estamos lá, assim, a conversa vai, mas o que o Brasil entende como soberania é outra coisa.

**Giovanna Barbosa**

Esse era o negócio que eu queria ter feito no meu projeto final, mas não tinha espaço. Mas eu estou louca nesse assunto, porque eu realmente tenho visto, tenho duas visões bem divergentes lá na União Europeia sobre o que é soberania digital. Um que é, não, a gente tem que adotar princípios abertos, tecnologias abertas, tecnologias que conversam entre si, então, interoperáveis e tudo mais, e tem gente falando, não, a gente quer ter o nosso Google. Mas repetindo o mesmo modelo da Google. A gente quer a nossa própria Microsoft, repetindo o modelo da Microsoft.

**Carla Aguiar**

Que é isso, que é um pouco o que a China tá fazendo, assim, né? Tá montando aquele ecossistema dele, mas aí vai vender, vai virar outro loquinho. Só que o legal, por exemplo, que a China tem alguns padrões abertos, pelo menos assim, a gente tem alguns escolhas, tem mais escolhas, né, não é uma caixa preta. Quando você vê lá na China, padrão aberto, te facilita um pouco a fazer migração, enfim.

**Giovanna Barbosa**

Mas não é uma coisa transversal e não é não é tão política de Estado como a diplomacia brasileira, por exemplo. Claro que a gente teve loucuros aí no governo Bolsonaro na diplomacia brasileira, a diplomacia brasileira, ela se mantém bem estável com certos princípios que ela segue, a maneira como ela negocia com certos países e tudo mais. O Brasil tem uma visão bem estabelecida na diplomacia mundial. De uma postura, que é a postura da diplomacia brasileira. Essa é a postura que é adotada pela diplomacia brasileira. Vem governo, sai governo. E é bem madura. O que você acha que falta Para que Software livre seja isso dentro da administração pública? Esse desfile do software livre como movimento político e virar um ser apresentado como uma coisa mais técnica, qual que é a resistência?

**Carla Aguiar**

Ah, eu acho que são tantas camadas. Por exemplo, primeiro capacitação. Capacitação de equipes técnicas, capacitação de gestores para entender valor. Aí um, que eu acho que onde a gente grande perde é o lobby. Porque, assim, aqui em Brasília, o que eu mais vejo é lobby até de empresa brasileira, privada, para vender, ganhar licitação. É muito, tem muito licitação casada, que já abre, já pensa, já muito desenhada para um fornecedor, que foi desenhado antes. Então, assim, e eu acho que vai para além de corrupção, não é uma questão de corrupção, é uma questão de de como que que a lógica, né de trabalho, assim tipo assim, você é que esse problema do lobby eu não sei como resolver usando software livre, assim porque aí vem uma questão de normativa, de tarará de ter uma coisa de imposição mas mesmo trazendo imposição é muito gerencial de adotar, que é uma coisa que eu vejo que o mercado privado ele é muito bom, assim, por exemplo, de abrir licença pra estudante, porque ele sabe que aqui 15 anos aquele estudante vai ser tomador de decisão.

**Giovanna Barbosa**

Passa o mel na boca da criança ali.

**Carla Aguiar**

Exato. Então isso é tipo assim, uma jornada que ela é muito complexa, assim, sabe, assim, eu vejo, por exemplo, no laboratório, todo mundo usa, eu tento, né, colocar todo mundo usando o Linux, quando eu vejo alguém usando o Windows, eu quero chorar, que eu vejo que eu falhei como profissional, mas é porque, assim, também a minha conta estratégica, eu sei que essa galera daqui a pouco vai ser chefe, então, assim, aí, mas, eu nem sei se eu estou te respondendo, mas, assim, só que eu vejo muito do viés técnico, né, eu não consigo te dar essa informação, talvez, do viés político, mas onde eu vejo muita barreira de adoção de software livre é na resistência de adoção, de achar que não tem suporte técnico, mas por quê? Porque é ignorante, que não conhece, então tem a resistência técnica, e tem uma resistência de governança de quem toma a decisão...

**Carla Aguiar**

Porque eles têm a falta também de conhecimento, que eles têm a falsa impressão que o privado vem pronto, e sendo que o governo é uma anomalia, ele trabalha com a lógica diferente do mercado, então o que vem de mercado não é bom para o governo, só um exemplo, acho que a Caixa paga 150 milhões para a Microsoft, por ano, não sei se é por ano, sei que é 150 milhões, e aí eles nunca conseguiram configurar, instalar o Skype corporativo, Aí o Dorgão foi lá oferecer o... Como é que é o nome? O Rocket Chat. O Rocket Chat. E aí eles queriam pagar um Rocket Chat, mas porque tinha várias soluções da Microsoft que não atendia a regra de negócio deles, né? Então, isso... Mas aí quando você olha, você fala assim, ah, não, porque o software é muito transparente até nesse ponto. Você vai comprar, mas eu tenho um momento que eu preciso customizar para você.

**Carla Aguiar**

Não é de prateleira, pode ser, mas assim para o governo quase nunca é esse tempo que o privado falou que não existe, isso também eu acho que é uma barreira para a adoção do software livre esse imediatismo que é de governo não estado, assim, que eu vejo que todo mundo pensa, assim o gestor padrão do governo federal, um gestor que está no cargo de comissionado, né que é realmente quem vai assinar contrato ele quer um ganho político imediato. Ele, assim, isso pra mim é mais uma regra do que uma exceção. Eles não pensam no Estado, eles pensam em ganho político. Assim, aqui que eu, eu pessoalmente, ou minha frente ali, vou ganhar politicamente fazendo isso. Então, é muito, as decisões de contratação são muito imediatistas, fica esses franquistais todos aí, aconselhando...

**Giovanna Barbosa**

eu quero voltar aproveitar esses últimos minutos que eu quero voltar num ponto que eu achei interessante que você levantou da dificuldade de ingressar no ecossistema desse dinheiro uma coisa que eu fico pensando é que é difícil foi difícil adentrar porque eles estão lá no norte global e a gente está aqui no sul global e era difícil para eles entenderem o do qual a gente vinha, ou o acesso aos locais onde eles estavam, não só os locais virtuais, você tem aí as comunidades, canais, mas os eventos, é custoso para a gente fazer esse deslocamento para a Europa, por exemplo, para estar ali presente. Quanto você acha que isso influenciou na demora para um ganho de confiança, para adentrar dentro do ecossistema, desse dia? Até porque vocês não estão completamente dentro, você está falando, a gente nunca está dentro.

**Carla Aguiar**

A gente não está dentro, eu entendo que a gente não está dentro, eu acho que quem está dentro são as europeias. Apesar dos casos bem conhecidos serem americanos, no sentido assim, Brasil, Nova York tem uma instância legal do Decidim, tem um processo interessante de participação, então a gente tem casos Uruguai, tem Argentina, tem vários casos aqui na América Norte e Latina de uso positivo do Decidim. Europa é uso muito restrito, é muito pequeno, mas eles ainda são esse petit comité, por exemplo, eles não entendem a... assim, aí, primeiro, tem essa questão de visão mesmo que você falou, né, E tem um elitismo porque tem coisas que eles já venceram e a gente ainda não. Por exemplo, acesso à internet. Internet rápida. Para eles, o Decidim não é um problema ele ser pesado, que demora para carregar, é uma...

**Giovanna Barbosa**

É difícil de acessar no celular.

**Carla Aguiar**

Não é mobile first. Para eles, isso nunca foi um problema. Para a gente, é impeditivo de usar. É muito difícil, porque demora cinco segundos, às vezes, para fazer um load de uma página do Decidim, assim, aqui no Brasil. E aí, os nossos problemas, eles não vêm como problema, assim. Isso é um menosprezo, né, talvez, de alguns problemas que a gente tem. Só que, ao mesmo tempo, a gente tem o poder de ter falado, não, cara, a gente fez o que vocês nunca fizeram, em termos de escala, de usar federal, que é muito pequeno. Então tem tem esse silo cultural eu acho, ali no meio.

**Giovanna Barbosa**

Você sente que essa dificuldade, essas coisas tão próprias da nossa realidade, foi o motivo pelo qual vocês primeiro começaram como um fork e depois vocês retornaram—ah não, vamos modularizar isso aqui.

**Carla Aguiar**

A gente fez o fork porque era o que a gente tecnicamente sabia fazer naquela hora, que era reescrever tudo e costumar...

**Giovanna Barbosa**

Isso não influenciou, que interessante.

**Carla Aguiar**

Isso não influenciou. E aí foi uma intenção política de integrar com a comunidade justamente para dificultar que a plataforma caia. Ou que a gente construiu com a plataforma, se mudar o político, sei lá, a gestão, isso seja desconstruído, né.

**Giovanna Barbosa**

É uma resiliência comunitária.

**Carla Aguiar**

É, uma resiliência, e essa é aquela capitalidade, quanto mais garras você tem, mais difícil é te derrubar. Então, a intenção é muito mais política do que técnica, porque técnica, a gente continua tendo todas as barreiras, deles acharem que essa, sei lá, vocês não programam tão bem quanto o Alecrim Dourado deles lá, tem que ser do jeito que ele quer, que é super bem escrito, mas para não ter performance, então a gente faz o negócio otimizado para ter performance, então tem essa barreira, hoje a gente só não adentra porque tem esse silo cultural ali no meio, tem um silo. Existe essa barreira clara, imposta, de muita coisa que a gente fala, eles não veem valor, e deles não entenderem o que, assim, o porquê da gente faz algumas, por que que a gente faz, por exemplo, simplificar, eles, a ideia desse dia é trazer transparência ao extremo,

**Carla Aguiar**

Então ele complexifica para o usuário, cognitivamente, e a nossa é assim, a gente quer que mais pessoas participem, então eu tenho que diminuir a carga cognitiva, e isso para eles, a gente está tirando transparência, então assim, está vendo que, mas é porque onde que eles querem atingir lá é a pessoa que já é politicamente engajada, que já é digitalizada, eles não querem atingir vamos dizer, a gente quer, como que eu falo, a gente quer atingir a rodoviária, a gente quer ser a participação da rodoviária, qualquer pessoa vai lá e participe, que não tenha barreira. Eles não querem isso. Assim, isso não é o objetivo deles, enquanto o nosso é o principal objetivo, para eles não é.

Eu acho que tem todos esses silos aí que até quase impedem uma colaboração e a contribuição nossa.

**Giovanna Barbosa**

O que você faria diferente hoje, se você fosse começar esse projeto hoje? Quais foram as maiores lições que você aprendeu nessa caminhada até agora?

**Carla Aguiar**

Então, ceder a atropelos políticos, né? A gente cedeu muito, assim, como equipe de desenvolvimento, porque a gente entende a importância da plataforma, a gente entende as urgências, às vezes, de ah, eu tenho que lançar uma coisa sem a plataforma estar madura. E aí a gente cedeu, e muitas vezes, aí trazia bug, que trazia resistência do outro lado, menor acesso, e isso foi recorrente, assim, e às vezes a gente fez muito retrabalho, muito retrabalho, assim, você cede a pressão ao requisito, não está maduro, você implementa, e aí você fica revisando o requisito em código enquanto já está em produção. Então, isso acho que foi a maior lição que eu tenho desse projeto, e aí dificulta você justamente contribuir para a comunidade, pensar como módulo, pensar como tecnopolítica, pensar como ter essas reflexões todas, né,

**Carla Aguiar**

Que aí eu acho que a gente teve atropelado e a gente está tendo essa reflexão agora, assim, de que a gente está conseguindo aplicar o que deveria ter sido feito para o SAS, que é fazer cadenciado, fazer, pensando mais no impacto e na política como um reflexo técnico do que apagar um fogo, às vezes até de capricho, de alguém.
