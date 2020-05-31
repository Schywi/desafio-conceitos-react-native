<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h3 align="center">
  Desafio 04: Conceitos do React Native
</h3>


## :rocket: Sobre o desafio

Nesse desafio, você deve criar uma aplicação para treinar o que você aprendeu até agora no React Native!

Agora você deve continuar desenvolvendo a aplicação que irá armazenar repositórios do seu portfólio, que você já desenvolveu o backend utilizando o Node.js, e no último desafio em ReactJS.

## Conceitos abordados

#### Propriedades do FlatList:

- **FlatList**

     FlatList é um componente do React Native que é responsável por aprensentar lista na nossa tela

- **data**

    São os nossos dados que vieram do back-end e vão preencher nossa lista

- **keyExtractor**

    É a nossa key que é passsada em uma lista do ReactJs, só que nesse caso fazemos um map especificando qual é o atributo que não se repete cada um dos nossos items.

- **renderItem**

    É uma função responsável por renderizar nossa lista na tela, dentro dela criamos um loop com o código que queremos que se repita dentro

    ex: 

    ```jsx
    renderItem={({item: project}) => (
    	 <Text style={styles.project}>{project.title}</Text>
    )}
    ```
 **SafeAreaView** : Serve para deixar a nossa aplicação ocupando somente sua area visivel.
 
**Touchable** : São componentes tocáveis, eles não possuem estilo então devemos cria-los.

## Instalando dependências

 Execute o comando `yarn` no seu terminal para instalar todas as dependências .

**Atenção**: Caso você esteja emulando no iOS, na pasta do seu projeto navegue até a pasta ios executando o comando `cd ios` e depois execute `pod install` para instalar todas as dependências para o iOS.

### Funcionalidades esperadas da aplicação

- **`Listar os repositórios da sua API`**: Deve ser capaz de criar uma lista de todos os repositórios que estão cadastrados na sua API com os campos **title**, **techs** e número de curtidas seguindo o padrão `${repository.likes} curtidas`, apenas alterando o número para ser dinâmico.

- **`Curtir um repositório listado da API`**: Deve ser capaz de curtir um item na sua API através de um botão com o texto **Curtir** e deve atualizar o número de likes na listagem no mobile.

### Específicação dos testes

Em cada teste, tem uma breve descrição no que sua aplicação deve cumprir para que o teste passe.

Para esse desafio temos os seguintes testes:

- **`should add a like to the like counter of the repository`**: Para que esse teste passe, sua aplicação deve permitir ao clicar no botão `Curtir`, um like seja adicionado ao repositório listado, e que essa atualização possa ser visualizada na tela.
