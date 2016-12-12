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
