# TP2-IHC - Relatório de Análise de Engajamento em AVA

## Definição do problema
O problema está inserido no contexto de um Ambiente Virtual de Aprendizagem (AVA), como o Moodle ou Canvas, aplicado à disciplina de Cálculo I no curso de Engenharia de Software. Essa disciplina apresenta historicamente altas taxas de reprovação e evasão, principalmente nas primeiras semanas do semestre, quando os alunos ainda estão em fase de adaptação. 

O objetivo é identificar o nível de engajamento de alunos em um Ambiente Virtual de Aprendizagem (AVA) com base em seus comportamentos na plataforma, visando intervenções pedagógicas precoces.

---
## Atributos utilizados na Base

- `percentual_videos_vistos`: porcentagem de vídeos assistidos
- `percentual_exercicios_entregues`: porcentagem de exercícios entregues
- `posts_iniciados_forum`: número de posts iniciados
- `respostas_em_posts`: número de respostas em posts
- `media_tempo_sessao_min`: tempo médio por sessão (minutos)
- `regularidade_acesso`: Regular ou Irregular
- `nivel_engajamento`: alto, médio ou baixo

---
## Classe-alvo: 
- `nivel_engajamento`, podendo assumir os valores alto, médio ou baixo.

---
## Regras de Classificação
As regras que definem o nível de engajamento foram estabelecidas com base em padrões de comportamento observados: 

Alto: aluno que assiste aos vídeos, entrega exercícios e participa dos fóruns. 

Regra para nivel_engajamento = Alto

Os numeros são porcentagem % (exceto em post_iniciados e respostas)

## Regras usadas para gerar a Classe-alvo 
As regras que definem o nível de engajamento foram estabelecidas com base em padrões de comportamento observados: 

Alto: aluno que assiste aos vídeos, entrega exercícios e participa dos fóruns.

Regra para nivel_engajamento = Alto 
os numeros são porcentagem % (exceto em post_iniciados e respostas) 

- Se `(percentual_videos_vistos > 75)` 
- E `(percentual_exercicios_entregues > 80)`
- E `(posts_iniciados_forum > 1 OU respostas_em_posts > 2)`
- E `(media_tempo_sessao_min > 20)`
- E `(regularidade_acesso == 'Regular')`
- Então `nivel_engajamento = Alto`

Médio: aluno que participa apenas de uma dimensão — por exemplo, assiste vídeos e entrega atividades, mas não interage nos fóruns. 

Regra para nivel_engajamento = Medio 

Qualquer aluno que "escapa" das duas definições de Alto e Baixo, cai automaticamente em 'Médio'.

Baixo: aluno com pouco consumo de conteúdo, poucas entregas e nenhuma interação. Regra para nivel_engajamento = Baixo 

- Se `(percentual_videos_vistos < 30)`
- E `(percentual_exercicios_entregues < 25)` 
- E `(posts_iniciados_forum == 0 E respostas_em_posts == 0)` 
- E `(regularidade_acesso == 'Irregular')` 
- Então `nivel_engajamento = Baixo`

De acordo com a árvore gerada pelo algoritmo J48, o atributo mais importante foi media_tempo_sessao_min. Se o tempo médio for menor que 14 minutos, o aluno é baixo engajamento. Mas se o tempo médio for maior que 14 minutos e o número de respostas_em_posts for menor que 3, o aluno é médio engajamento. E se o tempo for maior que 14 minutos e houver mais de 3 respostas, o aluno é alto engajamento.

---
## Descrição da base sintética
A base de dados é sintética, simulando comportamentos de alunos em um AVA durante as três primeiras semanas do semestre.

Ela contém 209 instâncias e 7 atributos, sendo seis preditores e uma classe. Cada instância representa um aluno e seu respectivo comportamento de acesso, entrega de atividades e interação.

Os dados foram construídos de forma a representar situações reais observadas em cursos online, diferenciando padrões de comportamento em relação ao tempo de estudo, interação social e frequência de acesso.

---
## Experimentos com Weka

Os experimentos foram realizados no software Weka, utilizando diferentes algoritmos de classificação: 

- ZeroR
- OneR
- J48
- NaiveBayes
- IBK

Cada modelo foi treinado e testado sobre a base sintética, e os resultados foram avaliados com base na acurácia e nas matrizes de confusão. 
Análises gráficas foram feitas para explorar a relação entre os atributos: 
- Exercícios entregues × Vídeos vistos; 
- Tempo médio por sessão × Vídeos vistos; 
- Posts iniciados × Respostas em posts.

Essas visualizações mostraram que há uma relação direta entre o engajamento e o tempo de estudo, número de vídeos assistidos e exercícios entregues.

---
## Visualize                                                           (Azul: alto; vermelho: médio; ciano baixo)
<img width="1057" height="942" alt="Visualize geral" src="https://github.com/user-attachments/assets/38c0fc7c-7527-48ff-ae9e-116333e111c1" />

---
## Exercícios entregues X Vídeos vistos
<img width="964" height="583" alt="exercicio entrgue X Video visto" src="https://github.com/user-attachments/assets/cd9ef4fc-a4f5-4292-bc13-6f3f8fefd870" />

*Ao analisarmos esta relação podemos perceber que quanto mais exercícios o aluno entregou e mais vídeos ele assistiu mais engajado ele é; sendo que os entregaram poucos exercícios e viram poucos vídeos tiveram seu engajamento considerado como baixo; podemos notar também que os mesmos alunos que entregaram poucos exercícios também assistiram poucos vídeos, não tendo alunos que viram poucos vídeos que entregaram muitos exercícios e vice-versa.*

---
## Tempo médio por sessão X Videos vistos
<img width="965" height="604" alt="tempo sessão X videos vistps" src="https://github.com/user-attachments/assets/646aa48e-0378-4191-b7de-c976876a946f" />

*Os alunos que ficaram mais tempo em uma sessão consequentemente viram mais vídeos, e os que ficaram pouco tempo viram poucos vídeos, o que nos mostra uma separação clara dos pontos coloridos, o que nos mostra que as classes são nem separadas e que seguem um padrão, assim como a relação de Exercícios entregues X Vídeos vistos.*

---
## Posts iniciados e respostas em posts
<img width="1718" height="452" alt="resposta e criação de post" src="https://github.com/user-attachments/assets/f23cac57-d83c-4e1e-8bd8-01325a5e8cea" />

*Ao analisarmos ambos as classes comparados com as demais, podemos notar que elas não são tão confiáveis quanto as demais, pelo menos não de forma individual; nem todos os alunos que são realmente engajados iram interagir na sessão de postagem; As citadas anteriormente nos dá uma noção maior do que a mostrada agora.*

---
## Media de tempo por sessão
<img width="1734" height="225" alt="Media tempo sessão" src="https://github.com/user-attachments/assets/0aa632fe-1e66-4f31-99cb-06263cd4ad3c" />

*A media de tempo por sessão é uma das classes mais determinantes para classificar o nível de engajamento do aluno, já que quanto mais tempo ele passa em uma sessão, mais atividades ele entrga, mais posts ele faz, mais ele interage e mais vídeos ele assiste.*

---
## ZeroR
<img width="946" height="543" alt="ZeroR" src="https://github.com/user-attachments/assets/74bc717a-83f0-4c32-a1d7-dce65f2f70bc" />

*O algoritmo ZeroR foi o menos preciso dentre os demais modelos testados neste trabalho; analisando a porcentagem de instancias classificadas corretamente nós podemos perceber que sua taxa de sucesso é 32,39% ou seja de 1 para três, o que se comparado aos outros que tiveram um desempenho muito superior em relação a este se mostra não ser tão confiável assim, pelo menos não neste caso.
Ao analisarmos a matriz de confusão do algoritmo ZeroR podemos notar que ele classificou todas as instancias como médio e nenhuma como alta ou baixa, das que ele classificou como médio ele acertou somente 23 instancias e errou todas as demais, ou seja, ele apenas definiu que todas são médias, a classe mais comum entre os dados usados para treino.*

---
## OneR
<img width="1039" height="546" alt="OneR" src="https://github.com/user-attachments/assets/cbf9e339-ce5e-46f2-813f-7c9a091e29e2" />

*O algoritmo OneR classificou 97.18% das instancias corretamente, ou seja, das 71 instancias ele acertou 69 errando apenas duas, um grande salto de qualidade em relação ao algoritmo ZeroR. A matriz de confusão nos mostra onde o algoritmo OneR errou e reforça que ele erou apenas duas instancias sendo uma que ele considerou como alto e a outra como médio erroneamente, e que acertou todas os que eram baixo, e acertou somente 24 das que ele classificou como alta e 22 das ele classificou como médio.* 

---
## J48
<img width="987" height="536" alt="J48" src="https://github.com/user-attachments/assets/60b48375-14d2-471d-9928-cdc9c3057baf" />

*Assim como o OneR o algoritmo J48 classificou corretamente somente 97.18% das instancias, ou seja, ele acertou 69 instancias e errou somente duas. A matriz de confusão mostra que o algoritmo J48 acertou todas as 23 instancias de classe médio, acertou apenas 24 instancias que ele classificou como alto e errou uma que ele considerou como média; e classificou corretamente apenas 22 como baixa e errou uma que classificou como média.*

---
## NaiveBayes e IBK
<img width="980" height="536" alt="IBK" src="https://github.com/user-attachments/assets/6fe268c2-82dc-4fad-b377-17c80672b3b1" />
<img width="935" height="541" alt="NaiveBayes" src="https://github.com/user-attachments/assets/11e70a6d-d4fb-456e-a204-fe13634d09c0" />

*Ambos os algoritmos NaiveBayes e IBK tiveram uma performance superior aos algoritmos ZeroR, OneR e J48; tendo 100% das instancias classificadas corretamente. Ou seja eles foram mais precisos que os modelos citados anteriormente, já que classificaram as 71 instancias de forma correta diferente das demais.*

---
## Arvore J48 
<img width="963" height="456" alt="Arvore J48" src="https://github.com/user-attachments/assets/1444a735-358b-479f-890b-a050a69df616" />

*A arvore gerada pelo algoritmo J48 considera o media_tempo_sessao_min como o atributo mais discriminativo entre os sete existentes na base para classificar se um aluno é ou não engajado/participativo. Segundo a arvore gerada, se um aluno fica em uma sessão por menos de 14 minutos o seu nível de engajamento é classificado como baixo. Se for maior que 14 minuto o algoritmo usará mais um atributo como referencia para decidir que seria o respostas_em_posts, se o número de respostas em posts for menor que três o aluno tem seu engajamento classificado como médio. Se o aluno assiste mais de 14 minutos por seção e tem um número de respostas maior que três, logo ele é considerado um aluno com um nível de engajamento alto.*

---
## Comparação entre os algoritmos
| Algoritmo   | Instancias corretas | Acuracia |
|-------------|---------------------|----------|
| ZeroR       | 23/71               | 32,39%   |
| OneR        | 69/71               | 97,18%   |
| J48         | 69/71               | 97,18%   |
| NaiveBayes  | 71/71               | 100%     |
| IBK         | 71/71               | 100%     |

Ao colocarmos os resultados em uma tabela, podemos perceber que o algoritmo ZeroR foi o que teve o pior desempenho em relação aos demais, já que sua acurácia foi de apenas 32,39, que comparado com os demais é o menos preciso; o OneR e J48 tiveram a mesma taxa de acurácia que foi de 97,18%, sendo ainda mais assertivo que o ZeroR; o NaiveBayes e o IBK tiveram também a mesma taxa de acurácia, sendo ela de 100%, sendo os mais assertivos em relação aos demais.
