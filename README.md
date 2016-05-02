# En français correct s'il vous plaît!
definition du titre du correcteur d'orthographe.

--- il faut importer un dictionnaire en lecture seule ---( myspell peut etre)

def dictionnaire (str)-> list:
   dictionnaire = []
   hunspell = open("classique-fr",'r')
   
   
def texte (str)-> list:
   texte = open(fichier,"r")
  paragraphe = [].append(texte)
  fichier.close
  return paragraphe
  
def extraction_données (list)-> list:
  mots = [] 
  liste_mot = texte.split(" ",";",",",".","!","?",'"',":")
  mots.append(liste_mot)
  return mots
  
def recherche (list)-> str:
  mal_orthographié=[]
  for m in range (len(mots)):
    mal_orthographié. append [i]
  return mal_orthographié
  
def main():
  erreurs=[]
  texte = str(input("Entrer le texte à corriger:{}".format(paragraphe)))
  erreurs.append (mal_orthographié)
  resultat = les mots mal orthographié



main()
