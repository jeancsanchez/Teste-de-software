# Teste de software - Definição
Segundo Pressman, o teste de software é um conjunto de atividades que podem ser planejadas com antecedência e executadas sistematicamente.
O teste começa no nível do componente e progride em direção à integração do sistema computacional como um todo.
Assim como o processo de desenvolvimento de software, o teste de software também possui um ciclo de vida:

## Planejamento
- Procedimentos iniciais
	Consiste na elaboração de um documento de um estabelecimento de acordo entre as partes envolvidas no projeto de teste, para definir, por exemplo, o pessoal envolvido, as responsabilidades de cada um, avaliação de riscos, etc...

- Especificação
	Elaboração e definição dos casos de testes "scripts" e dos roteiros de testes

- Execução 
	Execução dos testes planejados de acordo com os casos de testes "scripts" com os correspondentes registros dos resultados obtidos.

- Entrega
	Conclusão dos processos de testes e entrega do sistema para o ambiente de produção.


Segundo Myers, o custo de correção de defeitos tende a aumentar quanto mais tarde o defeito é detectado. Defeitos encontrados durante a produção tendem a custar muito mais do que defeitos encontrados em modelos de  dados e em outros documentos do projeto do software. Myers afirma ainda que: 
	- Os testes unitários podem remover entre 30% e 50% dos defeitos dos programas;
	- Os testes de sistemas podem remover entre 30% e 50% dos defeitos remanescentes;
	- Desse modo, os sistemas podem ir para a produção ainda com aproximadamente 49% de defeitos;
	- Por último, as revisões de códigos podem reduzir entre 20% e 30% desses defeitos;

Neste contexto, um erro é definido como um problema de qualidade encontrado antes do software ser liberado aos usuários finais. O defeito é um problema de qualidade encontrado depois de o software ter sido liberado aos usuários finais. Porém, na maioria das vezes os termos são utilizados como sinônimos devido à dificuldade de classificação dos termos.


# Revisões técnicas

As revisões técnicas são o mecasnismos mais efetivos para descobrir erros antes que sejam passados par os usuários finais. Por isso são utilizadas logo no inicio de gestão de qualidade.

Utilizamos as revisões técnicas para encontrar erros durante o processo de desenvolvimeto, de modo a não se tornarem defeitos depois da liberação do software. A descoberta precoce de erros, evita que sejam propagados para a próxima etapa na gestão de qualidade.
Segundo Pressman, diversos estudos e análises sobre o tema indicam que as atividades de projeto introduzem de 50 a 60% de todos os erros durante a gestão da qualidade. Entretanto, técnicas de rescisão demonstraram ser até 75% eficazes na descoberta de falhas no projeto.

## Revisões técnicas formais (RTF)

Devem ser estabelecidas previamente diretrizes para a realização das revisões técnicas formais e distribuídas a todos os revisores. *Uma revisão não controlada pode ser pior do que não fazer nenhuma revisão.*

Cada reunião de revisão deve ser preparada antecipadamente, porém não deve tomar mais que duas horas de trabalho de cada pessoa. Devem estar envolvidas de 3 a 5 pessoas em uma revisão e cada reunião de revisão deve ser pelo menos de duas horas. Durante a RTF, um revisor registra ativamente todos os problemas levantados. Estes são sintetizados no final da reunião de revisão e é produzida uma lista de problemas de revisão, além do relátorio sintetizado da revisão técnica formal. O relatório sintetizado de revisão deve responder a três questões:
 - O quê foi revisado?
 - Quem revisou?
 - Quais foram as descobertas e as conclusões?

# Depuração
O processo de depuração frequentemente ocorre em consequência de um teste. Quando um caso de teste descobre um erro, a depuração será o processo que irá resultar na remoção do erro. O processo de depuração tenta combinar o sintoma com a causa, levando assim à correção do erro. Normalmente apresentará um dentre dois resultados:
 - A causa será encontrada e corrigida;
 - A causa não será encontrada;

Segundo Pressman, uma vez encontrado o erro, ele precisa ser corrigido. A correção de um defeito pode introduzir outros erros e, portanto, causar mais danos do que trazer benefícios.
Segunda Van Vleck, três perguntas devem ser feitas antes de fazer a "correção" que remove a causa de um defeito:
- A causa do defeito é reproduzida em alguma outra parte do programa?
- Qual é o próximo defeito que pode ser introduzido pelo reparo que estou prestes a fazer?
- A causa do defeito é reproduzida em alguma outra parte do programa?

## Teste de Caixa-branca
O teste de caixa branca, segundo Pressman também chamado dde caix-de-vidro, utiliza a estrutura de controle descrita no programa para derivar casos de teste. São baseados nos elementeos internos de um trecho de programa. O objetivo é encontrar o menor número de casos de teste que permita que todos os comandos de um programa sejam executados pelo menos uma vez.
Casos de teste são determinados a partir das estruturas de controle do programa e desta forma forçar que todos os caminhos possíveis do fluxo de controle do programa sejam percorridos durante os testes. Desta forma é possível criar casos de caminos possíveis do fluxo de controle do programa sejam percorridos durante os testes. Desta forma é possível criar casos de teste que:
	- Garatnam que todos os caminhos independentes de um módulo foram exercitados pelo menos uma vez;
	- Exercitam todas as decisões lógicas nos seus estados verdadeiros e falso;
	- Executam todos os ciclos em seus limites e dentro de suas fronteiras operacionais;
	- Exercitam estruturas de dados internas para assegurar sua validade;

Existem diferentes tipos de testes de caixa branca que podem ser subdividos:
	- Teste de caminho básico:
	 	O passo inicial é determinar todos os caminhos possíveis. Normalmente utiliza-se um grafo de fluxo de controle do programa. O gráfico permite identificar os caminhos possíveis para que se possa elaborar os casos de uso. Como cada caminho é definido pelas expressões condicionais das estruturas de controle, devem-se determinar os casos de teste escolhendo valores de varíaveis para os casos nos quais cada uma das expressões sejam verdadeiras ou não.
	- Teste de condição:
		O teste de condição, segundo Pressman, é um método de projeto de caso de teste que exercita as condições lógicas contidas em um módulo de programa: Uma condição simples é uma variável boolean ou um expressão relacional, possívelmente precedida por um operador NOT. Uma condição composta é formada por duas ou mais condições simples, operadores booleanos e parênteses.
Este tipo de teste foca o teste de cada condição no programa para garantir que ele não contenha erros.
	- Teste de fluxo de dados:
		Este método seleciona os caminhos de teste de um programa de acordo com as localização de definições e usos de variáveis no programa. São úteis para selecionar caminhos de teste de um programa que contenha instruções de laços e if aninhadas.

## Teste de Caixa-preta
O teste da caixa preta também conhecido como teste comportamental, focaliza os requisitos funcionais do software. Este tipo de teste complementa o teste da caixa branca, pois permite descobrir uma classe de erros diferentes daquela obtida com métodos da caixa-branca. Desta forma o teste de caixa-preta tenta encontrar erros nas seguintes categorias:
	- Funções incorretas ou faltando;
	- Erros de interface;
	- Erros em estrutura de dados ou acesso a base de dados externas;
	- Erros de comportamento ou desempenho;
	- Erros de inicialização e término;

to be continued slide 7 aula 3...

