![TrackNMe](https://www.tracknme.com.br/app/images/logo-tracknme.png)


# Desafio WEB

O candidato deve dar **fork** neste repositório e após o termino do desenvolvimento, realizar um **pull request** e avisar por **email** para análise do time.

O desafio consiste em criar uma página web com as seguintes características:

# Task 1 - Desenhar um trajeto no mapa

Implementar uma página web cuja tela principal apresenta um mapa (google maps) e um trajeto obtido de uma api REST.
Recomendamos que use o [Apiary](https://apiary.io) como API nessa etapa ou alguma similar de sua escolha.
O app deve consultar a api REST e salvar o resultado (JSON) localmente (session/local storage).
Após a consulta o app deve buscar na session/local storage os dados salvos da consulta na API e desenhar o trajeto obtido.

Exemplo de retorno da API:

``` json
[
    {
    	"dateTime": "2017-10-12T21:34:15",
		"latitude": -23.962676666666667,
		"longitude": -46.3884785
    },
    {
    	"dateTime": "2017-10-12T21:40:15",
		"latitude": -23.982676666666667,
		"longitude": -46.4084785
    }
]
```

Diferencial, porém não obrigatório:
Personalizar o marcador e animar sua transição no mapa.

# Task 2 - Calendario

Nesta fase, o app deve ser capaz de fazer uma consulta ao serviço REST passando uma data como parametro e mostrando o trajeto conforme a data informada.

Ex.

GET /posicoes?data=2017-01-01 (Imprime apenas as posições obtidas do dia 01/01/2017).

GET /posicoes?data=2017-01-02 (Imprime apenas as posições obtidas do dia 02/01/2017).

E assim por diante.

Todos os resultados devem ser salvos localmente (session/local storage).
Para efeito de cache, posições de uma data já pesquisada, não devem fazer a chamada REST novamente. Seu conteudo deve ser obtido do storage, neste caso.

Diferencial, porém não obrigatório:
Mostrar informações em cada ponto do trajeto (infowindow)

---
#### LICENSE
```
MIT License

Copyright (c) 2017 TrackNMe

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```



# TracknmeWebJrChallenge

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.2.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
