# Como Começar

## Programa de Parceiros

O Programa de Parceiros engloba programadores, designers e experts que desenvolvem na plataforma da Nuvemshop. Você pode cadastrar sua conta [clicando aqui](http://www.nuvemshop.com.br/parceiros).

Sendo um Parceiro Nuvemshop você tem acesso ao [Painel de Parceiros](https://partners.nuvemshop.com.br/). Dentro do painel você pode criar uma loja de testes, gerenciar e criar aplicativos, acompanhar o recebimento de pagamentos, e ficar por dentro da últimas novidades sobre a Nuvemshop.

---

## Passo-a-passo para criar seu primeiro Aplicativo

1. Registre-se no [Programa de Parceiros](http://www.nuvemshop.com.br/parceiros)
2. Dentro do painel de administração de parceiros, clique em "Aplicativos > Criar Aplicativo" 
3. Preencha os dados da sua aplicação.
4. Leia sobre [como autenticar](https://github.com/tiendanube/api-docs/#authentication) seu aplicativo conosco.
5. Leia a [documentação da API](https://github.com/TiendaNube/api-docs) para saber como se comunicar com a Nuvemshop.

## Formulário de Criar Aplicativo
Explicaremos abaixo como preencher o [formulário de criação de aplicativo](https://partners.nuvemshop.com.br/apps/new/) detalhadamente. Ao finalizar o formulário você receberá as credenciais `API Key` e `APP ID` que permitirão a autenticação para realizar chamadas à nossa API.

### Configurações do App
Preencha cada um dos campos obrigatórios, defina a categoria para o aplicativo e selecione cuidadosamente as permissões necessárias para o correto funcionamento:


![urls](media/guidelines_urls.jpg)
1. **Nome**: Uso simples do nome do produto ou aplicativo, sem adjetivos, pontos de exclamação ou frases adicionais
2. **URL em que redirecionaremos o cliente quando o aplicativo estiver instalado:** A URL que o usuário será redirecionado ao instalar o aplicativo. Esta é sua URL de Callback, você deve usa-lá para receber e salvar o Store ID e Token do cliente durante o processo de [autenticação](https://github.com/tiendanube/api-docs/blob/master/resources/authentication.md).
3. **URL:** A URL do seu painel de administração que o usuário acessará para utilizar o aplicativo.
4. **URL de Preferências:** A URL para a área do seu aplicativo onde o usuário possa setar as configurações do app.
5. **URL de Suporte:** Endereço onde o usuário será redirecionado quando precisar de ajuda. Pode ser uma página de suporte *self-service* ou formulário de contato.
6. **Email de Suporte:** E-mail de contato para suporte no qual os usuários do aplicativo poderão entrar em contato.
7. **Categoria:** Selecione a categoria que seu aplicativo melhor se encaixa.
8. **Permissões:** Escolha somente os tipos de permissões você precisará de ter acesso.
  - *read_content* - Apenas leitura (não poderá alterar) as páginas de conteúdo da loja.
  - *write_content* - Modificar, eliminar e criar as páginas de conteúdo da loja.
  - *read_products* - Apenas leitura (não poderá alterar) os produtos e categorias da loja.
  - *write_products* - Modificar, eliminar e criar os produtos e categorias da loja.
  - *read_coupons* - Apenas leitura (não poderá alterar) os cupons de desconto
  - *write_coupons* - Modificar, eliminar e criar os cupons de desconto.
  - *read_customers* - Apenas leitura (não poderá alterar) os clientes da loja.
  - *write_customers* - Modificar, eliminar e criar os clientes da loja.
  - *read_orders* - Apenas leitura (não poderá alterar) as vendas da loja.
  - *write_orders* - Modificar, eliminar e criar vendas para a loja.
  - *write_scripts* - Adicionar componente usando javascript para a loja.
  - *read_shipping* - Apenas leitura (não poderá alterar) meios de envio.
  - *write_shipping* - Modificar, eliminar e criar meios de envio.
  
### Informações sobre o App
Essa seção possui os campos referentes a apresentação do aplicativo na nossa App Store. 

?> _DICA_ Você pode alterar essas informações antes de publicar o aplicativo, portanto não se preocupe em preencher tudo corretamente enquanto estiver na fase de testes. 

1. **Logo:** Imagem da logo do aplicativo. _(Tamanho Padrão: 310px x 100px)_
2. **Logo na tela própria da Loja de Aplicativos:** Esse é o ícone que identificará o aplicativo na App Store. Seu ícone deve medir 600x600 px, estar no formato .JPG e incluir um plano de fundo completo. Você pode usar nosso [template](https://www.nuvemshop.com.br/img/partners/guidelines-appstore/templates/icon_template.zip) para simular como será visto.
3. **Descrição Curta:** Acompanha o ícone e o nome do aplicativo na lista de aplicativos de nossa loja.  Busque oferecer um resumo claro da funcionalidade principal da integração em apenas uma frase, não excedendo 60 caracteres. Recomendamos não incluir o nome da aplicação para aproveitar melhor o espaço.
4. **Descrição:** A ideia é oferecer aos lojistas da Nuvemshop uma descrição clara, concisa e oportuna dos recursos do aplicativo e os benefícios da integração. A descrição não deve exceder 1600 caracteres e, por sua vez, não deve ter uma extensão inferior a 500 caracteres. Quanto ao formato de texto, deve ser "Normal" e alinhado à esquerda. Em seu conteúdo, tente desenvolver os seguintes pontos:
  - Qual problema seu aplicativo resolve?
  - Descreva os principais recursos do aplicativo
  - Para quem é idea?
  - Qual o seu diferencial competitivo
5. **Imagens:** As capturas de tela podem dar aos clientes uma ideia de como seu aplicativo funciona e servem como um complemento para ilustrar as informações fornecidas na descrição. As imagens devem ter um tamanho de 1600 x 800 px e estar no formato .JPG. Você pode usar nosso [template](https://www.nuvemshop.com.br/img/partners/guidelines-appstore/templates/screenshot_template.zip) para garantir que eles atendam às nossas especificações.
6. **Links do Administrador:** Permite os lojistas acessarem o aplicativo a partir de diferentes partes do painel administrativo da Nuvemshop. Isso facilita o acesso rápido às funções de um aplicativo diretamente na tela em que ele se encontra. Existem duas opções disponíveis:
    - **Links do Administrador:**  Quando nosso cliente clicar, ele acessa o URL inserida e enviamos os seguintes parâmetros: id = {id do objeto selecionado} e locale = {language do administrador}.
        - *Selecione onde o link vai aparecer:* Escolha a página da Nuvemshop que o link será exibido.
        - *Texto do link:* Texto que será exibido no link da ação
        - *Ícone do Link:* Selecione um ícone que ajude a identificar a ação.
        - *URL do link:* URL do seu aplicativo que será chamada quando o usuário clicar no link da ação.
    - **Links de ação em massa:** Insere uma opção de ação em massa na página de listagem. Quando o cliente clica, ele acessa a url com um array de ids como parametro:id[]=1&id[]=2.
        - *Selecione onde o link vai aparecer:* Escolha a página da Nuvemshop que o link será exibido.
        - *Texto do link:* Texto que será exibido no link da ação
        - *URL do link:* URL do seu aplicativo que será chamada quando o usuário clicar no link da ação.