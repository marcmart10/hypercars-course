# HTML e CSS de alta performance

#1 - Formas de lidar com CSS e JS

    Inline, incorporado e externo;

    Inline e incorporado, apesar de fazerem menos requisições, aumentam o tamanho do HTML, dificultando a manutenção para projetos grandes.

    Na maioria dos casos prefira o externo, pois ajuda na organização e possibilita que eles sejam armazenados no cache do navegador, ou seja, quando formos acessar pela segunda vez, esses arquivos já existirão, o que aumentará ainda mais a velocidade

#2 - Estilos no topo, scripts no rodapé

    O motivo dessa prática é simples: Se colocarmos os estilos antes, toda a parte que interessa ao usuário num primeiro momento, que é o visual com css, será renderizado progressivamente, pois já teremos os estilos e cada elemento html da página já aparecerá estilizado. Se o css viesse depois, primeiro veríamos o esqueleto html, para só então posteriormente os estilos serem aplicados. Se os scripts vierem antes, primeiro o site terá que carregar todo o javascript e só então trabalhará na formatação do site, pois eles bloqueiam a renderização da página enquanto estiverem carregando.

#3 - async

    Se utilizarmos essa propriedade poderemos carregar o script "ao mesmo tempo" que todo o resto. É importante ressaltar que se tivermos vários scripts a serem carregados, eles não obedecerão a nenhuma ordem específica, por isso a utilização do async deve ser muito bem pensada.

    <script async src="example.js"></script>

#4 - Utilize pré-processadores CSS

    Ao utilizar os pré-processadores economizamos várias linhas de código devido à sua sintaxe otimizada, modularizamos o CSS, promovendo assim uma maior organização, o que facilita a manutenção e legibilidade.

#5 - minifique o seu CSS e JS

    Quando escrevemos um código e importante que ele esteja legível e organizado, pois isso nos ajudará em manutenções futuras. No entanto, para o computador nada disso importa, e quanto mais arquivos tivermos, mais requisições o browser terá que fazer. Ao minificarmos nossos arquivos economizaremos vários bytes, pois isso estará em uma única página, o que diminuirá o número de requisições e nos ajudará a carregar as nossas páginas ainda mais rapidamente.

#TOOLS
business model - OK
thinking the content - OK
wireframe
gulp
sass
bem
grid layout
flexbox
jquery

# business model
- who is the owner
    Everton Braga
- what is important to me (instructor)
    Give a good knowledge to the students about the technologies that I'll speak in the course
- who is the audience?
    Students that want to learn about web development, mainly html and css

When I'm going to search a course, what I think is important?
    Didatic
    Good content - OK
    Best practices
    Up-to-date technologies - OK
    Complete project from scratch using all the concepts - OK
    Support

# thinking the content
In this course I'll build a high-performance car shop. My goals building this project aren't just about the client (car shop), but it's also about the way I'll do it, because the most important thing here is to give to my students a strong foundation of the modern web development. Of course all the sections have to make sense, but it's secondary.

#wireframe
Let's do our wireframe. Let's think about what a car website must have to be a good resource for potential buyers. Let's do some research:
www.porsche.com (showroom)
www.ferrari.com (css)
www.jeep.com 
www.bugatti.com