# Imersão Alura IA Gemini

Esse projeto visa criar um bot no qual utilizamos agentes para poder processar uma lista de compra fornecida pelo usuário, identificar os supermercados ao redor do endereço fornecido e retornar a lista com os melhores preços da sua região.

**Recomendações:**

* Rodar a aplicação no Google Colab;
* Ter uma API Key do Google AI Studio para ser utilizada no projeto. Você pode obter uma gratuitamente seguindo as instruções em [link para a documentação do Google AI Studio, se disponível].

**Execução:**

Ao executar todos os blocos iniciais, poderá executar o bloco Main que iniciará o projeto.
![image](https://github.com/user-attachments/assets/a1450b66-e3b4-42bb-8270-b70c72859baa)

1.  **Passe um endereço** (bairro, cidade - País):
    ![image](https://github.com/user-attachments/assets/d9150c41-58be-4a0b-a4fe-4f5183da2d9d)
    ![image](https://github.com/user-attachments/assets/75a85810-fec4-4452-89b9-ae6f54ce3565)

2.  **Depois, a lista de itens que quer pesquisar:**
    ```
    Exemplo:
    Arroz
    Feijão
    Biscoito
    Coca cola zero 2L
    ```
    ![image](https://github.com/user-attachments/assets/75a85810-fec4-4452-89b9-ae6f54ce3565)
    ![image](https://github.com/user-attachments/assets/e465397b-ccd9-4a1e-9d42-c208d8d07cd3)

Depois disso, é só deixar os agentes em ação:

* **Agente 1:** É responsável por pesquisar os supermercados da sua região, com um limite de até três.
* **Agente 2:** Pega a lista de compras e a lista de supermercados do Agente 1 e transforma em uma lista Python.
    ![image](https://github.com/user-attachments/assets/4adaecd4-ceb1-4a40-adf8-cf0e9d94eb92)
* **Agente 3:** É responsável por pegar cada supermercado da lista e pesquisar os preços dos itens. Se o usuário passar uma lista com elementos genéricos, o agente tenta pesquisar algo mais popular daquele item. E se não conseguir localizar um valor, irá procurar em outro local.
    ![image](https://github.com/user-attachments/assets/806c38fb-6c65-4227-b5c8-58504b0605b7)
    ![image](https://github.com/user-attachments/assets/5c708077-f9ca-4c3f-bc9f-f41aa09bf855)
* **Agente 4:** É responsável por analisar todas as listas de preços e montar a melhor lista ou escolher o melhor supermercado.
* **Agente 5:** É o revisor, valida se a formatação da lista está dentro do esperado.
    ![image](https://github.com/user-attachments/assets/479ab6ea-af5d-4571-a29f-208fa0bb3c2e)

**Observação:** O Agente 3 pode ter um delay na resposta devido à alta demanda de pesquisas por vários elementos.

**Testes Mockados:**

Para testes mockados, temos o bloco de teste:
![image](https://github.com/user-attachments/assets/195566b1-73de-46c0-b7e7-dc0fae8ee725)

Obrigado por curtir meu projeto LnB!
