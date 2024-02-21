# Reconhecimento Facial e transformação de imagens em Dados no Azure ML

## Detectar rostos no Vision Studio
As soluções de visão geralmente exigem que a IA seja capaz de detectar rostos humanos. Suponha que a empresa varejista fictícia Northwind Traders queira localizar onde os clientes estão em uma loja para melhor atendê-los. Uma maneira de fazer isso é determinar se há algum rosto nas imagens e, em caso afirmativo, retornar as coordenadas da caixa delimitadora que mostram sua localização.

Para testar as capacidades de deteção facial do serviço Azure AI Face, utilizará o Azure Vision Studio . Esta é uma plataforma baseada em UI que permite explorar os recursos do Azure AI Vision sem a necessidade de escrever nenhum código.

### Crie um recurso de serviços de IA do Azure
Você pode usar o serviço Azure AI Face com um recurso multisserviço de serviços de IA do Azure . Se ainda não o fez, crie um recurso de serviços de IA do Azure na sua assinatura do Azure.

#### Em outra guia do navegador, abra o portal do Azure em https://portal.azure.com , entrando com a conta da Microsoft associada à sua assinatura do Azure.

#### Clique no botão ＋Criar um recurso e pesquise os serviços de IA do Azure . Selecione criar um plano de serviços de IA do Azure . Você será levado a uma página para criar um recurso de serviços de IA do Azure. Configure-o com as seguintes configurações: 

Assinatura : sua assinatura do Azure . 

Grupo de recursos : Selecione ou crie um grupo de recursos com um nome exclusivo .

Região : Leste dos EUA.

Nome : Insira um nome exclusivo .

Nível de preços : Padrão S0.

Ao marcar esta caixa, confirmo que li e compreendi todos os termos abaixo : Selecionado .

Selecione Revisar + criar e depois Criar e aguarde a conclusão da implantação.

### Conecte seu recurso de serviço de IA do Azure ao Vision Studio
#### Em seguida, conecte o recurso de serviços de IA do Azure provisionado acima ao Vision Studio.

#### Em outra guia do navegador, navegue até Vision Studio em https://portal.vision.cognitive.azure.com .

#### Entre com sua conta e certifique-se de usar o mesmo diretório onde você criou seu recurso de serviços de IA do Azure.

#### Na página inicial do Vision Studio, selecione Visualizar todos os recursos no título Introdução ao Vision .

#### Na página Selecione um recurso para trabalhar , passe o cursor do mouse sobre o recurso que você criou acima na lista e marque a caixa à esquerda do nome do recurso e selecione Selecionar como recurso padrão .

#### Feche a página de configurações selecionando o “x” no canto superior direito da tela.

### Detecte rostos no Vision Studio
#### Num navegador web, navegue até Vision Studio em https://portal.vision.cognitive.azure.com .

#### Na página inicial Introdução ao Vision , selecione a guia Face e, em seguida, selecione o bloco Detectar rostos em uma imagem .

#### No subtítulo Experimente , reconheça a política de uso de recursos lendo e marcando a caixa.

#### Selecione cada uma das imagens de amostra e observe os dados de detecção facial retornados.

#### Agora vamos tentar com algumas de nossas próprias imagens. Selecione https://aka.ms/mslearn-detect-faces para baixar detect-faces.zip . Em seguida, abra a pasta no seu computador.



