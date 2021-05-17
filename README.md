# PROJETO LANDING PAGE CEISC


# Montagem do layout
Para deixar o projeto pronto utilizei o framework Javascript VueJS, não utilizei SASS pois como não o uso com frequência, inicialmente estava me atrasando então optei por terminar apenas com CSS.

# Componetização
Cada componente representa uma parte específica do projeto, poderia ter mais componentes mas  se tratando de um projeto relativamente simples não achei tão importante deixar muito componentizado.

# Propriedades utilizadas para a responsividade
Para estilizar a maior parte do projeto utilizei GRID e FLEXBOX do CSS já que tenho boa experiência com essas propriedades para a montagem de estruturas pensando na responsividade. Pensei em usar Bootstrap e cheguei a instalar Vuetify para ajudar a compor o layout mas  vi que não casavam com a proposta do porjeto. 

# Mudanças sutís na versão final
O projeto está responsivo para qualquer tela de dispositivo móvel, infelizmente tive que remover o background na versão mobile pois causou um problema de comportamento, talvez seja por causa do overlay que tive que aplicar sobre ele para deixar a foto azul semi-transparente  com a propriedade CSS posição 'absolute'. 
 
# Formulário
 Deixei o preenchimemto do formulário como obrigatório, apenas após o usuário fornecer seu nome e email é que aparecerá a messagem de sucesso na tela por 3 segundos. No briefing há uma figura junto na tela de messagem mas não consegui baixá-la para inserir no projeto e tive que optar por não colocá-la na versão final. 

# Fontes e ícones
 Não encontrei as fontes descritas no briefing então optei por usar Lexend e Quicksand do Google Fonts por terem características parecidas. Utilizei as logos e fotos fornecidos pelo briefing, para as redes sociais usei os ícones do Fontawesome por se adaptarem muito melhor.

# Carrosel de imagens
Para montar o carrosel utilizei um plugin chamado UIkit JS o que deixou a versão final bem mais fiel ao proposto. Não foi difícil a montagem, tive que adaptar as imagens na quantidade correta e ajustar o tamanho para todos os tamanhos dispositivos.

# Animações
Adicionei animação no banner infomativo e formulário no momento que a página é carregada, optei por deixar apenas uma vez e também evitei adionar no restante do projeto para não impactar a perfomance.

# Instruções de visualização do projeto
Para ver o projeto basta acessar o diretório "ceisc_landingpage" dentro de um terminal e digitar "npm install" para instalar as dependências necessárias  e após o término digitar no mesmo diretório "npm run serve" e aguardar o projeto rodar na porta localhost "http://localhost:8080".