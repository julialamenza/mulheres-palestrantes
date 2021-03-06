# Como contribuir

1. Fork este projeto - Clique em  `Fork`

2. Crie uma nova branch para realizar suas alterações no repositório - Com o Git instalado execute o comanado abaixo no terminal. - [caso não tenha o Git, baixe aqui](https://git-scm.com/downloads) - 
    ````
    git checkout -b nome-da-branch
    ````

3. Inicie o projeto - Com Node instalado, rode o comando abaixo no terminal. - [caso não tenha o Node, baixe aqui](https://nodejs.org/en/) - 
    ```sh
    $ npm start
    ```

4. Adicione uma nova linha no arquivo `mulheres.json` com seus dados, conforme exemplo abaixo:

    ```JSON
    /* Exemplo de uma palestrante chamada Foo Bar */

    /* Abaixo desse exemplo deixamos dicas para preenchimento dos campos: photo, redes sociais [linkedin, github, twitter, fb] e interests */

    {
      "name": "Foo Bar",
      "interests":
        [
          "UX Design",
          "Web Design",
          "Front-end",
          "Rails"
        ],
      "location": "São Paulo/SP",
      "photo": null,
      "email": "foobar@domain.com",
      "linkedin": "foobarname",
      "github": "foobarname",
      "twitter": "foobarname",
      "fb": "foo.bar"
    }
    ```

    ## Dicas para prenchimento do arquivo `mulheres.json`:

    - **Como adicionar uma foto?**<br>
      Para adicionar uma photo ao seu card, crie uma conta e faça upload do seu avatar no Gravatar - [acesse o site através desse link](https://en.gravatar.com/) - ou use a sua conta já existente.

    - **Como preencher os campos de redes sociais?** <br>
      Em *linkedin*, *github*, *twitter* e *fb*: usar apenas o username da url da rede social.
      > Exemplo: <br>
        https://www.facebook.com/foo.bar >> "foo.bar"
        https://br.linkedin.com/in/foob >> "foob"
        etc

    - **Como preencher "interests"?** <br>
        Evite adiconar muitas tags nesse campo, dependendo da quantidade de caracteres cabem até 7 tags no card da página, mas o ideal seria usar *4* no *máximo*.

    - **Como preencher os campos que não tenho dados para adicionar?** <br>
      Caso exista algum campo onde você não tenha um valor real para ser preenchido, o mesmo pode ser adiconado o valor `null`, veja o exemplo abaixo de uma palestrante que não possui conta no facebook e twitter:
      ```
      {
        "twitter":"null",
        "fb":"null"
      }
      ```

5. Commit suas alterações - Execute no terminal: 
    ````
    git commit -m 'Add Foo Bar'
    ````

6. Suba suas alterações para o repositório remoto:
    ````
    git push origin master
    ````

7. Envie um pull request para o repositório original, após seu pull request ser aceito seus dados estarão disponíveis no site 💜 

