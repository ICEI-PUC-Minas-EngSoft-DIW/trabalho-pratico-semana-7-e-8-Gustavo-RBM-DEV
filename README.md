# Trabalho Prático 05 - Semanas 7 e 8

**Páginas de detalhes dinâmicas**

Nessa etapa, vamos evoluir o trabalho anterior, acrescentando a página de detalhes, conforme o  projeto escolhido. Imagine que a página principal (home-page) mostre um visão dos vários itens que existem no seu site. Ao clicar em um item, você é direcionado pra a página de detalhes. A página de detalhe vai mostrar todas as informações sobre o item do seu projeto. seja esse item uma notícia, filme, receita, lugar turístico ou evento.

Leia o enunciado completo no Canvas. 

**IMPORTANTE:** Assim como informado anteriormente, capriche na etapa pois você vai precisar dessa parte para as próximas semanas. 

**IMPORTANTE:** Você deve trabalhar e alterar apenas arquivos dentro da pasta **`public`,** mantendo os arquivos **`index.html`**, **`styles.css`** e **`app.js`** com estes nomes, conforme enunciado. Deixe todos os demais arquivos e pastas desse repositório inalterados. **PRESTE MUITA ATENÇÃO NISSO.**

## Informações Gerais

- Nome: Gustavo Rodrigues Barbara Moreira
- Matricula:898623
- Proposta de projeto escolhida: Temas e Conteúdos Associados
- Breve descrição sobre seu projeto: Site de curiosidades e noticias a respeito de jogos e consoles antigos.

## Print da Home-Page

<< <img width="1920" height="4144" alt="home page" src="https://github.com/user-attachments/assets/4903fc3e-e6cb-44ec-b26e-393e40b59cc8" />
  >>

## Print da página de detalhes do item

<<  <img width="1920" height="1135" alt="pagina detalhes" src="https://github.com/user-attachments/assets/0740a58f-4c6d-475a-a465-de35c7cf8642" />
 >>

## Cole aqui abaixo a estrutura JSON utilizada no app.js


const dadosGerais = [
  
  {
    "id": 101,
    "titulo": "Atari 2600 (1977)",
    "descricao": "Lançado em 1977, o Atari 2600 é um dos primeiros consoles de videogame domésticos...",
    "conteudo": "O **Atari 2600** revolucionou o mercado em 1977, popularizando o conceito de cartuchos intercambiáveis. Com gráficos simples, mas inovadores para a época, trouxe a experiência de arcade para a sala de estar. Jogos como *Space Invaders* e *Pitfall!* se tornaram clássicos instantâneos. Sua influência é inegável, estabelecendo as bases para toda a indústria moderna de videogames.",
    "categoria": "Console",
    "data": "1977-09-11",
    "imagem": "img/atari2600.jpg"
  },
  {
    "id": 102,
    "titulo": "Nintendo Entertainment System (NES) (1983)",
    "descricao": "Lançado em 1983, o NES revitalizou a indústria de videogames após a crise de 1983...",
    "conteudo": "O **NES** não apenas salvou a indústria após a crise de 1983, mas a redefiniu. Com um controle de qualidade rigoroso e títulos icônicos como *Super Mario Bros.* e *The Legend of Zelda*, ele introduziu a jogabilidade baseada em enredo e mecânicas mais complexas. Seu sucesso transformou a Nintendo em uma gigante global.",
    "categoria": "Console",
    "data": "1983-07-15",
    "imagem": "img/nes.jpg"
  },
  {
    "id": 103,
    "titulo": "Sega Master System (1985)",
    "descricao": "Lançado em 1985, o Sega Master System foi o principal concorrente do NES...",
    "conteudo": "O **Master System** foi a primeira grande aposta da Sega no mercado de consoles. Embora tenha tido mais sucesso na Europa e no Brasil do que na América do Norte, ele possuía gráficos tecnicamente superiores ao NES e introduziu personagens como *Alex Kidd*. Foi fundamental para iniciar a 'Guerra dos Consoles' com a Nintendo.",
    "categoria": "Console",
    "data": "1985-10-20",
    "imagem": "img/Master-System.jpg"
  },
  {
    "id": 104,
    "titulo": "Sega Genesis (Mega Drive) (1988)",
    "descricao": "Lançado em 1988, o Sega Genesis, conhecido como Mega Drive fora da América do Norte...",
    "conteudo": "O **Mega Drive** marcou a transição para a era dos 16 bits. Sua campanha de marketing agressiva, focada na velocidade e no público adolescente, e a introdução de *Sonic the Hedgehog*, permitiram à Sega competir de igual para igual com o SNES. É lembrado por sua vasta biblioteca de jogos de arcade e RPGs.",
    "categoria": "Console",
    "data": "1988-10-29",
    "imagem": "img/Mega-Drive.jpg"
  },
  {
    "id": 105,
    "titulo": "Super Nintendo Entertainment System (SNES) (1990)",
    "descricao": "Lançado em 1990, o SNES é conhecido por seus gráficos avançados e uma biblioteca de jogos lendários...",
    "conteudo": "O **SNES** elevou o padrão dos jogos de 16 bits com o uso de chips de melhoria (*Mode 7*, *Super FX*), resultando em jogos visualmente deslumbrantes como *Super Mario World* e *Final Fantasy VI*. O foco em jogos de plataforma e RPGs de alta qualidade garantiu sua posição como um dos consoles mais amados da história.",
    "categoria": "Console",
    "data": "1990-11-21",
    "imagem": "img/snes.jpg"
  },
 
  {
    "id": 201,
    "titulo": "Pong (1972)",
    "descricao": "Lançado em 1972, Pong é um dos primeiros videogames da história...",
    "conteudo": "**Pong** é creditado como um dos primeiros jogos de arcade de sucesso comercial. Seu design extremamente simples (duas barras e uma bola) provou que o mercado de jogos eletrônicos era viável. Ele desencadeou a indústria de videogames e inspirou inúmeros jogos de esporte.",
    "categoria": "Jogo",
    "data": "1972-11-29",
    "imagem": "img/pong.jpg"
  },
  {
    "id": 202,
    "titulo": "Space Invaders (1978)",
    "descricao": "Um clássico de 1978, Space Invaders coloca o jogador no comando de uma nave que deve atirar e destruir hordas de alienígenas...",
    "conteudo": "**Space Invaders** foi um fenômeno cultural global. É um dos primeiros jogos de tiro (shmup) e popularizou o conceito de pontuação alta. Sua demanda por moedas era tão alta que se diz ter causado uma escassez temporária de moedas de 100 ienes no Japão!",
    "categoria": "Jogo",
    "data": "1978-06-16",
    "imagem": "img/space-invaders.jpg"
  },
  {
    "id": 203,
    "titulo": "Pac-Man (1980)",
    "descricao": "Pac-Man é um clássico jogo de arcade lançado em 1980, onde o jogador controla o personagem Pac-Man em labirintos...",
    "conteudo": "**Pac-Man** (originalmente Puck Man) é um dos jogos de arcade mais vendidos e reconhecidos de todos os tempos. Sua jogabilidade de labirinto, focada em estratégia e evasão, e o apelo do personagem, o transformaram em um ícone pop que transcendeu o mundo dos games.",
    "categoria": "Jogo",
    "data": "1980-05-22",
    "imagem": "img/pac-man.jpg"
  },
  {
    "id": 204,
    "titulo": "Tetris (1984)",
    "descricao": "Lançado em 1984, Tetris é um jogo de quebra-cabeça onde o jogador deve encaixar peças de diferentes formas...",
    "conteudo": "**Tetris** é notável por ter sido criado por um engenheiro de software russo e por ser um dos jogos mais portados de todos os tempos. Sua popularidade explodiu globalmente com o lançamento do Nintendo Game Boy, provando que jogos simples e viciantes podem ser eternos. É um mestre em design de jogos pela sua simplicidade e profundidade.",
    "categoria": "Jogo",
    "data": "1984-06-06",
    "imagem": "img/tetris.jpg"
  },
  {
    "id": 205,
    "titulo": "Super Mario Bros (1985)",
    "descricao": "Lançado em 1985, Super Mario Bros é um jogo de plataforma onde o jogador controla Mario...",
    "conteudo": "**Super Mario Bros.** é o jogo de plataforma definitivo. Ele definiu o gênero, introduzindo conceitos como rolagem lateral suave, power-ups, e design de fases que ensina o jogador através da experiência. Seu sucesso no NES o tornou um divisor de águas e o jogo mais influente de todos os tempos.",
    "categoria": "Jogo",
    "data": "1985-09-13",
    "imagem": "img/super-mario-bross.jpg"
  },
 
  {
    "id": 1,
    "titulo": "O Retorno dos Arcades",
    "descricao": "Nos últimos anos, os arcades têm visto um ressurgimento, com novos estabelecimentos abrindo em várias cidades...",
    "conteudo": "Nos últimos anos, os **arcades** têm visto um ressurgimento, com novos estabelecimentos abrindo em várias cidades ao redor do mundo. Esses locais oferecem uma experiência nostálgica, combinando jogos clássicos com novas tecnologias, atraindo tanto jogadores antigos quanto novos. É uma forma de reviver a era de ouro dos fliperamas. **O conceito de 'barcade' (bar + arcade) se popularizou, onde adultos podem desfrutar de bebidas e jogos clássicos.**",
    "categoria": "Curiosidade",
    "data": "2025-03-30",
    "imagem": "img/arcades.jpeg"
  },
  {
    "id": 2,
    "titulo": "Remakes e Remasters",
    "descricao": "Muitos jogos retro estão sendo remasterizados ou refeitos para plataformas modernas. Títulos como 'The Legend of Zelda: Link's Awakening'...",
    "conteudo": "Muitos jogos retro estão sendo **remasterizados ou refeitos** para plataformas modernas. Títulos como 'The Legend of Zelda: Link's Awakening' e 'Final Fantasy VII Remake' trazem gráficos atualizados e jogabilidade aprimorada, permitindo que novas gerações experimentem esses clássicos com uma roupagem nova e atraente, mantendo a essência original. **A facilidade de acesso em consoles modernos é um grande atrativo para os fãs do retrô.**",
    "categoria": "Notícia",
    "data": "2025-03-28",
    "imagem": "img/remake.jpeg"
  },
  {
    "id": 3,
    "titulo": "Preservação de Jogos Antigos",
    "descricao": "Organizações e comunidades dedicadas à preservação de jogos antigos estão ganhando destaque. Elas trabalham para arquivar...",
    "conteudo": "Organizações e comunidades dedicadas à **preservação de jogos antigos** estão ganhando destaque. Elas trabalham para arquivar e manter o acesso a jogos que poderiam ser perdidos devido à obsolescência tecnológica, garantindo que a história dos videogames seja preservada para o futuro e que as novas gerações possam conhecer a origem da cultura gamer. **Museus de videogame e projetos de emulação legal têm um papel crucial nisso.**",
    "categoria": "Curiosidade",
    "data": "2025-03-27",
    "imagem": "img/preservaçao.jpeg"
  },
  {
    "id": 4,
    "titulo": "Chegada do Analogue 3D (Console tipo N64 moderno)",
    "descricao": "O Analogue 3D, console retro que reproduz fielmente o Nintendo 64 com tecnologia FPGA...",
    "conteudo": "O **Analogue 3D**, console retro que reproduz fielmente o Nintendo 64 com tecnologia FPGA, compatível com cartuchos originais, saída em 4K e suporte a Bluetooth, viu seu lançamento adiado para julho/agosto de 2025 devido a arancelas. É uma esperada opção premium para fãs do retrô que buscam a experiência autêntica com qualidade moderna. **Esta empresa é conhecida por produzir consoles de alta qualidade para jogos antigos.**",
    "categoria": "Notícia",
    "data": "2025-03-25",
    "imagem": "img/analogues3d.jpeg"
  }
];



function criarCardHTML(item, tipo) {
  const urlDetalhes = `detalhes.html?id=${item.id}`; 
  const textoBotao = item.categoria === 'Console' ? 'Ver Console' : 
                     item.categoria === 'Jogo' ? 'Ver Jogo' : 'Ver Notícia';
  
  return `
    <div class="col-12 col-md-6 col-lg-4">
      <article class="card bg-dark text-light h-100 border-warning">
        <a href="${urlDetalhes}">
            <img src="${item.imagem}" class="card-img-top" alt="${item.titulo}">
        </a>
        <div class="card-body">
          <a href="${urlDetalhes}" class="text-decoration-none text-light">
            <h3 class="card-title text-warning">${item.titulo}</h3>
          </a>
          <p class="card-text">${item.descricao}</p>
          <a href="${urlDetalhes}" class="btn btn-sm btn-outline-warning mt-2">${textoBotao}</a>
        </div>
      </article>
    </div>
  `;
}


function carregarSecaoHome(idContainer, categoria) {
    const container = document.getElementById(idContainer);
    if (!container) return;

    // Filtra os itens do array unificado pela categoria desejada
    const itensFiltrados = dadosGerais.filter(item => item.categoria === categoria);
    
    let htmlContent = '';
    itensFiltrados.forEach(item => {
        htmlContent += criarCardHTML(item);
    });
    
    container.innerHTML = htmlContent;
}




function buscarDetalhesItem(id) {
   
    return dadosGerais.find(item => item.id == id); 
}

function carregarDetalhesPagina() {
    const detalhesContainer = document.getElementById('detalhes-item');
    if (!detalhesContainer) return;

    const urlParams = new URLSearchParams(window.location.search);
    const itemId = urlParams.get('id'); 
    
    const item = buscarDetalhesItem(itemId);

    if (item) {
        
        let textoDetalhes;
        if (item.categoria === 'Console') {
            textoDetalhes = `Detalhes Históricos: ${item.titulo}`;
        } else if (item.categoria === 'Jogo') {
             textoDetalhes = `Análise e Impacto: ${item.titulo}`;
        } else {
             textoDetalhes = `Notícia Completa: ${item.titulo}`;
        }
        
        const htmlDetalhes = `
            <h1 class="text-warning mb-4">${item.titulo}</h1>
            <img src="${item.imagem}" class="img-fluid rounded mb-4" alt="${item.titulo}">
            <p class="text-muted small">
                Tipo: <span class="badge bg-warning text-dark">${item.categoria}</span> | 
                Data de Lançamento/Publicação: ${new Date(item.data).toLocaleDateString('pt-BR')}
            </p>
            <hr class="border-warning">
            <p class="lead">${item.descricao}</p>
            <div class="mt-4 full-content">
                <h3 class="text-warning">${textoDetalhes}</h3>
                <p>${item.conteudo.replace(/\n/g, '<br>')}</p> 
            </div>
        `;
        
        detalhesContainer.innerHTML = htmlDetalhes;
        document.title = `${item.titulo} - Games Retro`; 
    } else {
        detalhesContainer.innerHTML = `
            <h1 class="text-danger text-center mb-4">Item não encontrado!</h1>
            <p class="text-center">O ID especificado na URL não corresponde a nenhum item, console, jogo ou notícia.</p>
        `;
    }
}




document.addEventListener('DOMContentLoaded', () => {
    if (document.body.id === 'home-page') {
        
        carregarSecaoHome('cards-consoles', 'Console'); 
        
        
        carregarSecaoHome('cards-jogos', 'Jogo');
        
        
        carregarSecaoHome('cards-dinamicos', 'Curiosidade');
        carregarSecaoHome('cards-dinamicos', 'Notícia'); 
        
    } else if (document.body.id === 'detalhes-page') {
        carregarDetalhesPagina();
    }
});
```
