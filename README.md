# restaurante


Elabore um algoritmo que possa descobrir, através de perguntas e respostas, em qual área de um restaurante uma pessoa ou grupo de pessoas precisa ser alocada.
O restaurante tem três áreas: térreo, 1ro andar, e área externa.
Clientes fumantes ou com animais de estimação precisam ser alocadas na área externa.
Grupos de 5 ou mais precisam ser alocados no 1º andar, pois não dá para juntar mesas no térreo.
Qualquer outro grupo de pessoas pode ser alocado no térreo





Algoritmo de Alocação no Restaurante

Inicialize a variável grupo_completo como falso
Inicialize a variável area_alocada como vazio

Escreva "Bem-vindo ao restaurante!"

Escreva "Quantas pessoas estão no grupo?"
Leia numero_pessoas

Escreva "Algum membro do grupo é fumante ou possui animais de estimação? (S/N)"
Leia resposta_fumante_animais

Se resposta_fumante_animais = "S" então
    area_alocada <- "área externa"
Senão
    Se numero_pessoas >= 5 então
        area_alocada <- "1º andar"
        grupo_completo <- verdadeiro
    Senão
        area_alocada <- "térreo"
    Fim Se
Fim Se

Se grupo_completo = verdadeiro então
    Escreva "O grupo deve ser alocado no", area_alocada, "do restaurante."
Senão
    Escreva "O grupo pode ser alocado no", area_alocada, "do restaurante."
Fim Se

Fim do Algoritmo
Nesse algoritmo, primeiro perguntamos ao usuário quantas pessoas estão no grupo e se algum membro do grupo é fumante ou possui animais de estimação. Em seguida, com base nas respostas, determinamos a área de alocação de acordo com as regras estabelecidas: grupos com fumantes ou animais de estimação serão alocados na área externa, grupos com 5 ou mais pessoas serão alocados no 1º andar e os demais grupos serão alocados no térreo.






