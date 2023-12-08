# Um cilindro muito longo carregado

Para calcula o campo elétrico dessa distribuição de carga com simetria axial é conveniente utilizar a lei de Gauss, utilizando uma superfície Gaussiana com a mesma simetria, axial, da distribuição. 
Sendo $\rho$ a densidade de carga e $L$ um comprimento arbitrário na direção do eixo do cilindro, temos que a carga total de um segmento $L$ do cilindro vai ser igual ao volume interior ao raio $r$  desde que seja menor que $R$, portanto temos para $r \leq R$ a carga total vai ser $q = V\rho = \pi L r^2\rho$. 
Para $r > R$ temos $q = \pi R^2 L\rho$.  
Assim temos a lei de Gauss $$\frac{V\rho}{\varepsilon_0} = \int \vec E \cdot d\vec A.$$ Precisamos encontrar agora o elemento de área do cilindro que envolve o volume da $V$, ou seja, a superfície gaussiana. Podemos imaginar a superfície Gaussiana nesse caso como sendo composta por um número infinito de pequenos anéis de altura $dh$, dessa forma a área total vai ser integrada de $0\rightarrow L$. Então o elemento de área vai ser $$d\vec A = \hat r (2 \pi r)dh.$$ Onde $\hat r$ é o vetor unitário na direção radial, e $r$ é um comprimento do raio da superfície gaussiana. Temos então dessa forma 
$$\frac{V\rho}{\varepsilon_0} = \int_0^L (\vec E \cdot\hat r) 2\pi r dh.$$
Como a simetria do problema permite assumir que $\vec E$ e $\hat  r$ são paralelos, $\parallel$, podemos assumir que $\vec E \cdot \hat r = E$. Resolvendo a integral a seguir encontramos: $$\frac{V\rho}{\varepsilon_0} = E 2\pi r L.$$ Onde $V$ é o volume englobado pela superfície gaussiana. Teremos duas situações diferentes. 
### $r < R$
A primeira em que $r < R$ temos apenas uma fração da carga total contribuindo para o campo elétrico, lembrando que apenas a carga no interior da superfície Gaussiana contribui para o campo elétrico na superfície. Então o campo elétrico vai ser 
$$\frac{\pi L r^2\rho}{\varepsilon_0} = 2\pi rE L$$$$E = \frac{r\rho}{2\varepsilon_0}.$$Temos que o campo elétrico cresce linearmente com o raio. 
### $r > R$
Na segunda situação temos que o volume envolto pela superfície gaussiana é maior do que o volume total que possui carga, dessa forma quanto maior a superfície menor vai ser o volume ocupado pela distribuição de carga. Vamos escrever isso nas contas, usando a carga total do volume $q = \pi R^2 L \rho$ na equação obtida anteriormente $$\frac{\pi R^2 L \rho}{\varepsilon_0} = 2\pi r E L$$ Mais uma vez, cancelando o $L$ dos dois lados: $$\frac{\pi R^2\rho}{\varepsilon_0} = 2\pi r E$$ Isolando $E$ e simplificando a expressão obtemos a expressão para o campo elétrico em função do raio $r$:
$$E = \frac{R^2 \rho}{2 r\varepsilon_0}.$$
Podemos notar que dessa vez temos uma função que decresce em função de $r$, como todos os outros termos são constantes temos uma função que diminui como $1/r$.
### O potencial elétrico 
O potencial elétrico de uma distribuição de carga pode ser obtido a partir da integral do campo elétrico sobre um caminho, nesse caso, devido à simetria do problema podemos tomar o caminho como partindo da origem $$V = -\int_0^r \vec E\cdot\hat r'dr'$$
O potencial elétrico em função do raio para a primeira parte, onde $r < R$ temos que realizar a integral 
$$V(r) = -\int_0^r \frac{r'\rho}{2\varepsilon_0} dr' = -\frac{r^2 \rho}{2\varepsilon_0}.$$
Para a segunda parte temos que considerar que a partir do raio $r=R$ a função muda, portanto a integral é igual ao potencial anterior avaliado em $V(R)$ somado à diferença de potencial de $R \rightarrow r$. Assim para $r > R$ temos: $$V(r) = V(R) - \int_R^{r} \vec E \cdot \hat r' dr' = V(R) - \int_R^{r} \frac{R^2 \rho}{2 r\varepsilon_0}dr',$$
$$V(r) = V(R) - \frac{R^2\rho}{2\varepsilon_0}\log\left(\frac{r}{R}\right)$$
$$V(r) = -\frac{R^2 \rho}{2\varepsilon_0} -\frac{R^2\rho}{2\varepsilon_0}\log\left(\frac{r}{R}\right)$$
