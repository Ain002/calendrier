# calendrier
date ={"jours":0,"mois":0,"année":0}

list_de_mois = {"janvier":1,"fevrier":2,"mars":3,"avril":4,"mai":5,"juin":6,"juillet":7,"aout":8,"septembre":9,"octobre":10,"novembre":11,"decembre":12}


   

#test de saisie
while True:
    try :
        date["jours"] = int(input("ecriver le jours : "))
        break
    except ValueError:
        print("le jours n'est pas bon")

while True:
    try :
        m = input("écriver le mois : ")
        if  m in list_de_mois:
            date["mois"] = m
        else :
            m in map(str,list_de_mois.values())
            date["mois"] = m
        break
    except ValueError:
        print("oups le mois saise n'est pas bon")
