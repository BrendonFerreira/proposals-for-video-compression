# Propostas para compressão de videos

Primeiramente, esse documento não é para ser formal msm, é necessariamente 
para eu despejar o meu fluxo de pensamento, e ideias que eu tenho para melhorar e optimizar a compressão de vídeos.

Ok?

Entao, eu estava vendo algumas coisas sobre compressão de video, e percebi que temos muito mais recurso a serem utilizados.

Como a separação por blocos. Que eu sinceramente achei aquilo horrivel.

Eu penso da seguinte forma.

Temos uma imagem para compressão. Ok?. Então podemos despejar pontos nessa imagem, podemos despejar dependendo da qualidade
da compressão desejada. Por exemplo, temos uma imagem de 10 x 10 pixels, desepejamos pontos em um espaçamento de 2 pixeis.
Ou seja iremos ficar com 25 pontos.
Pensando em 25 pontos, tentei pensar em algo do tipo: 
  - Se eu ligasse esses pontos, eu poderia detectar padrões, e detectar se há uma variação de cor muito grande entre eles. 
  - Caso tenha uma variação muito grande, eu coloco um ponto entre os dois pontos onde essa variação é grande.
  - Quando a variação for minima, eu procuro no dicionario de padrões, e aplico nesse intervalo entre dois pontos.
  
  

 
