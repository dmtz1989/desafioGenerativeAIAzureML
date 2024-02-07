# Desafio "Trabalhando com Machine Learning na Prática no Azule ML"

##### Como parte da resolução do desafio proposto pela DIO, estou descrevendo as etapas de como realizei a criação dos pontos de extremidades que usei no laboratório de Machine Learning.

##### Os passos seguidos foram:

###### 1. Foi criada uma conta no Portal do Azure (https://portal.azure.com/).
###### 2. Após a conta criada, foi realizada a criação do Resource Group.
###### 3. Com o Resource Group criado, foi realizada a criação de um Azure AI Services, com as seguintes configurações:

    Subscription: Your Azure subscription.
    Resource group: LAB-AI-900-DIO
    Region: East US.
    Name: labAzureCognitveServices.
    Pricing tier: Standard S0.
    By checking this box I acknowledge that I have read and understood all the terms below: Selected.
    
###### 4. Após a criação do Azure Ai Service, acessei o Vision Studio, através da URL "https://portal.vision.cognitive.azure.com".
###### 5. Após o login no Vision Studio, foi selecionada o Resource para poder iniciar a análise das imagens. Todos os inputs e outputs estão respectivamente na pasta "inputs" e "output" no repositório.
###### 6. A primeira análise realizada foi a análise de Face, utilizando a imagem encontrada no "input 1". Segue abaixo a imagem utilizada e o resultado da análise:
![input 1](https://github.com/dmtz1989/desafioGenerativeAIAzureML/blob/main/inputs/input%201.jpg)

    Face #1
    Face mask: no
    Face #2
    Face mask: no
    Face #3
    Face mask: no
    Face #4
    Face mask: no
    Face #5
    Face mask: no
    Face #6
    Face mask: no
    Face #7
    Face mask: no
    Face #8
    Face mask: yes
    Face mask covering nose and mouth: no
    Face #9
    Face mask: no
    Face #10
    Face mask: no

###### 6.1. Após análise, constatei que quando a pessoa está encoberta por alguma outra pessoa ou objeto, ele é considerado que está de máscara. O caso, poderia melhor a questão se informasse que seria uma máscara ou não.

###### 7. Para a segunda análise, foi realizada a Extração de texto com Imagem, utilizando a imagem do "input 2", com os resultados mostrados abaixo: 

![input 2](https://github.com/dmtz1989/desafioGenerativeAIAzureML/blob/main/inputs/Input%202.jpg)

    UniversidadeFederalRuraldePernambuco
    LicenciaturaPlenaemComputação
    aluno:DemetriusRicardodaDilecoOliveira
    ProvaFinalMatemáticaDiscreta
    1º)Consideremosneldoisinteirosquaisquer
    (Provauniversal)
    PorProvadireto,temos:
    n=2k+1
    sendoKEZZ
    k=2(b-4)0°
    o.b-4=20k2.
    2.b=2K+4
    n+b=2k+1
    2k+1+2K+4=2K+1
    4k+4+1=2K+1
    2(2K+2)+1=2K+1
    Considerando(2K+2)um
    20+1=2k+1
    númeroQEZ,temos!
    10
    comisso,temosquentb
    éImpar.afirmaçãoVerdadeira
    2º)Consideremosquefexsãodoisinteirosquais
    Ques(ProvaUniversal)
    porprovaexistencial,paraprovarmosqueafunção
    ésobrejetivo,temosqueprovarque((a)b-
    f(1)=7(-7)7=x+7(-7)
    0=X
    Concluimosque,existe
    uminteiroxQuesatisfaz
    aafirmação.afirmaçãoverdadeira
    
###### 7.1. Ao análisar os resultados, percebo que mesmo com uma letra legível, por ser manuscrito, a IA não conseguiu captar algumas palavras corretamente, e por isso ela deve ser treinada com mais caligrafias para um melhor resultado.

###### 8. Para última análise, foi realizada a análise de Adição de Legenda as Imagens. Foi utilizado a imagem do "input 3", e o resultado foi:

![input 3](https://github.com/dmtz1989/desafioGenerativeAIAzureML/blob/main/inputs/Input%203.jpg)

    A group of people in clothing
    
###### 8.1 Após analise, percebi que foi bastante simples a análise, e poderia dar mais informações sobre o tipo de vestimentas, como também os acessórios utilizados.

###### 11. Após o término nas análises, foi realizada a remoção da Workspace e do Resource Group, para evitar gastos excedentes.
