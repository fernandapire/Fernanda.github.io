<html>
<head>
<title><p><h1>Tudo sobre Ariana Grande</h1></p></title>
</head>
<img src="http://www.etonline.com/media/photo/2014/10/24107907/425_ariana_grande_lionneckl.jpg"/>
<body><p>A intenção desse quiz é saber o nivel de conhecimento que você tem sobre Ariana Grande. Trago poucas informações para ajuda-los.</p> 
<p>Ariana Grande-Butera nascida na cidade de Boca Raton, Flórida. Nome dos pais: Joan Grande, e Edward Butera. Irmão: Frankie. Frequentou a North Broward Preparatory School e participou de diversos teatros infantis e da comunidade.</p>
  
</body>





import random

perguntas_fáceis = (
    "Quantos anos tem Ariana Grande?",
    "Quantos álbuns Ariana Grande tem?",
    "Qual a extensão vocal de Ariana Grande?",
    "Em que ano Ariana Grande começou sua carreira de Cantora,atriz,compositora?",
    "No filme Swindle qual é o nome de seu personagem?",
    "Qual é o nome do grupo de jovens cantores que Ariana fundou aos 10 anos de idade?",
    "Qual é o personagem de terror favorito dela quando criança",
)

respostas_fáceis = (
# ["RESPOSTA CERTA","RESPOSTA ERRADA","RESPOSTA ERRADA"]
    ["21","23","20"],
    ["2","4","1"],
    ["Soprano","Tenor","Contra-alto"],
    ["2008","2005","2010"],
    ["Amanda Benson","Cat Valentine","Princesa Diaspro"],
    ["Kids Who Care","All helping","Kids all helping"],
    ["Freddy Krueger","Jason","Chuck"],
)

def main ():
    for índice,pergunta in enumerate(perguntas_fáceis):
        print(str(índice+1) + ":" + pergunta)

        respostas_embaralhas = list(respostas_fáceis[índice])
        random.shuffle(respostas_embaralhas)

        for respostas in respostas_embaralhas:
            print(respostas)

        resposta = input("Qual a resposta? ")
        if resposta == respostas_fáceis[índice] [0] :
            print("++++++++++++++")
            print("Resposta Certa")
            print("++++++++++++++")
        else:
            print("-------------")
            print("Tente de novo")
            print("-------------")

if __name__=='__main__':
     main()
