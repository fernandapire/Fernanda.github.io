<html>
<head>
<title>Tudo sobre Ariana Grande</title>
</head>
<body>A intenção desse quiz é saber o nivel de conhecimento que você tem sobre Ariana Grande. Trago poucas informações para ajuda-los. 
Ariana Grande-Butera nascida na cidade de Boca Raton, Flórida. Nome dos pais: Joan Grande, e Edward Butera. Irmão: Frankie. Frequentou a North Broward Preparatory School e participou de diversos teatros infantis e da comunidade
  
</body>





import random

perguntas_dificil = (
    "Quantos anos tem Ariana Grande?",
    "Quantos álbuns Ariana Grande tem?",
    "Qual a extensão vocal de Ariana Grande?",
    "Em que ano Ariana Grande começou sua carreira de Cantora,atriz,compositora?",
)

respostas_dificil = (
# ["RESPOSTA CERTA","RESPOSTA ERRADA","RESPOSTA ERRADA"]
    ["21","23","20"],
    ["2","4","1"],
    ["Soprano","Tenor","Contra-alto"],
    ["2008","2005","2010"],
)

def main ():
    for índice,pergunta in enumerate(perguntas_dificil):
        print(str(índice+1) + ":" + pergunta)

        respostas_embaralhas = list(respostas_dificil[índice])
        random.shuffle(respostas_embaralhas)

        for respostas in respostas_embaralhas:
            print(respostas)

        resposta = input("Qual a resposta? ")
        if resposta == respostas_dificil[índice] [0] :
            print("++++++++++++++")
            print("Resposta Certa")
            print("++++++++++++++")
        else:
            print("-------------")
            print("Tente de novo")
            print("-------------")

if __name__=='__main__':
     main()
