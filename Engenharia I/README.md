# bertoti

---

## 1 - Software é intangível
*(trecho do livro Software Engineering at Google, ver slide 4) Comentar com suas palavras.*

Engenharia de software, como qualquer outra engenharia é uma profissão que requer especialização na área e exige ao profissional a capacidade de criar soluções com base em seus estudos, construir algo. "Engenharia de software" é um termo, uma área mais ampla e significa muito mais do que apenas "programação", além de estar sempre em constante evolução e desenvolvimento.

É uma área nova, a engenharia de software começou a se desenvolver a partir da segunda metade do século XX (com seu marco no início de 2007, com o lançamento do primeiro iPhone), quando os sistemas começaram a ficar mais complexos e surgiu a necessidade de métodos mais organizados para desenvolver software.

A engenharia de software que tínhamos na década de 70/80, já não se adequa mais ao panorama atual, outro diferencial dessa engenharia comparada com as outras, além de ser a mais nova, é que apesar desses engenheiros também criarem algo, os resultados são mais intangíveis, e a área não é tão rigorosa em termos de profissionalização quando comparada as outras engenharias.

Mesmo sendo intangível, o software afeta diretamente o funcionamento de sistemas bancários, redes sociais, transporte e diversas outras áreas da sociedade, o que torna necessário o uso de práticas de engenharia cada vez mais rigorosas para garantir qualidade e confiabilidade.

---

## 2 - Engenharia de Software = Programação + tempo, escalabilidade e trade-offs  
*(trecho do livro Software Engineering at Google, ver slide 7) Comentar com suas palavras.*

A Engenharia de Software vai muito além de apenas programar. Embora a programação seja uma parte importante, essa área envolve compreender as necessidades e dores do usuário e transformar isso em soluções reais, por meio de requisitos bem definidos. O profissional não trabalha só com código, mas com todo o sistema: precisa entender como cada parte funciona, desde a produção até a entrega final, reconhecendo o papel de cada elemento no resultado do produto.

Além disso, a Engenharia de Software abrange todo o ciclo de desenvolvimento — *análise, projeto, implementação, testes e manutenção* — utilizando ferramentas como diagramas, modelagem e casos de uso para organizar ideias e alinhar equipes. Também envolve decisões sobre arquitetura, redes e integração entre sistemas, garantindo que o software seja escalável, seguro e eficiente.

Outro ponto essencial é pensar no futuro do sistema: como ele vai evoluir, crescer para atender mais usuários e lidar com possíveis conflitos entre requisitos. Isso exige visão sistêmica, planejamento e a capacidade de tomar decisões equilibrando diferentes trade-offs. No fim, trata-se de unir conhecimento técnico com estratégia, sempre focando na melhoria contínua e na experiência do usuário.
 
---

## 3 - Requisitos não funcionais  
*Listar 5 requisitos não funcionais e descrevê-los com suas palavras (ver slides 8, 9 e 10).*

Requisitos não funcionais definem  **características de qualidade**, ou seja, descrevem *como* o sistema deve se comportar, e não quais funções ele deve executar.

### Security:
Ter uma boa segurança é essencial para um software, para proteger as informações e dados sensíveis, garantindo que não haja vazamento de informações e nem ataques cibernéticos, além de atender á LGPD e assegurar a parte de autenticação e permissões de cada usuário.

### Scalability:
Se trata da capacidade desse software de desempenhar da mesma forma independente do número de acessos e de requisições, ele deve ser escalável, ter a mesma performance e eficiência além da carga imposta nele.

### Usability:
É a qualidade do software de ele ser intuitivo, ser capaz que o usuário utilize ele sem que o gere muitas dúvidas, deve ser "fácil" de ser navegado e operado.

### Robustness:
Capacidade do software de continuar operando mesmo quando algum processo da errado, que ele não trave ou "crashe" quando um erro acontece, como uma entrada inválida ou uma falha inesperada.

### Reliability:
Garante que o sistema funcione com a menor quantidade de erros possíveis, sem prejudicar a experiência do seu usuário. E se ocorrer travamentos, ou até mesmo ele ficar fora do ar por conta de uma falha, garante que ele volte á operar normalmente o quanto antes.

---

## 4 - Trade-offs (negociação entre requisitos)
*Citar e descrever 3 cenários de trade-offs (ver slide 12, mas usar outros exemplos)*

### Instagram (Disponibilidade) X PIX (Consistência):
**Instagram:** No Instagram ou em outras redes sociais, é priorizado a **disponibilidade** do sistema, ou seja, a ideia é que ele esteja sempre online, então o número de curtidas de uma foto pode travar, um story pode não carregar, o feed pode demorar mais do que o normal para ser atualizado, mas você sempre verá algo ali na sua tela aparentando funcionar, a experiência tenta ser rápida, mesmo que seja imprecisa.

**PIX:** Já no sistema de pagamento PIX, é preciso que cada dado seja checado e verídico, não pode ser possível realizar um pagamento se eu não tiver aquela quantia da transação disponível na minha conta, se eu receber um pagamento, meu extrato precisa ser atualizado **na hora** que a transação cair, ou seja, é um sistema que **não pode suportar erros**, e sua experiência pode ser demorada, desde que seja concluída, retornando se foi um sucesso ou se ocorreu alguma falha, as informações que o usuário visualizar, como extrato, saldo e transações, precisam ser checadas e verdadeiras, ou o dinheiro está lá ou não.

---

### Jogos: Qualidade (Visual) X Performance (FPS)
Em muitos jogos hoje em dia, existe a opção de escolher qual a sua prioridade ao jogar uma partida online, onde existem dois modos: um que prioriza a **qualidade gráfica**, mais fluidez, como animações, uma resolução de vídeo melhor, e melhorias gráficas;

Já o modo de **Performance** ou **Desempenho**: permite que o usuário troque a experiência de ter um jogo mais bonito por ter um jogo que muitas vezes **trave menos**. Isso se faz útil para pessoas que não possuem uma máquina muito robusta e capaz de suportar muitos frames, ou até mesmo pessoas que atuam no ramo competitivo, fazendo com que um modo que priorize a performance seja mais vantajoso, assim, cedendo a experiência de ter um jogo mais agradável visualmente.

---

### E-commerce: Segurança X Usabilidade

Quando a plataforma prioriza a segurança, ela pode exigir **autenticação em dois fatores**, **confirmações** por e-mail, senhas mais complexas e validações adicionais no momento do pagamento. Essas medidas aumentam a **proteção** contra fraudes e acessos indevidos, mas também tornam o processo de compra **mais demorado** e menos prático, o que pode fazer com que alguns usuários desistam da transação.

Por outro lado, quando o sistema prioriza a **usabilidade**, ele simplifica o processo com login automático, salvamento de dados do cartão e menos etapas no checkout, tornando a **experiência mais rápida** e prática. No entanto, essa simplificação pode aumentar os riscos de invasões ou compras não autorizadas.

Assim, ao melhorar a segurança, a experiência tende a ficar menos ágil, e ao tornar o uso mais simples e rápido, pode-se reduzir o nível de proteção, evidenciando a negociação entre esses dois requisitos não funcionais.

---

## 5 - Planejamento de um hotel com 4 entregas
### Processo Tradicional x Ágil

### Tradicional
1. Construir o chão  
2. Estrutura completa (paredes e andares)  
3. Áreas de lazer e cozinha  
4. Quartos  

### Ágil
1. Construir quartos simples  
2. Recepção  
3. Melhorar os quartos  
4. Serviço de quarto  

Errado: construir peças isoladas e torcer para encaixar no final.

Certo: construir um hotel (ou software) bem simples, mas 100% funcional, e ir melhorando a conforme o tempo passa.

---

## 6 - Sprints do navegador Google

- **1998:** Desorganização da informação → criação do PageRank (Larry Page e Sergey Brin)  
- **2008:** Estabilidade → arquitetura com múltiplos processos  
- **2008:** Velocidade → motor V8 (JavaScript mais rápido)  
- **2009-2010:** Personalização → extensões e Chrome Web Store  
- **2012:** Sincronização entre dispositivos  
- **2014-2015:** Segurança → priorização de HTTPS  
- **2018:** Redesign → melhor organização e usabilidade  
- **2023:** Performance → economia de memória e energia  
- **2024:** IA → organização automática e resumo de conteúdos  