# En français correct s'il vous plaît!

def dictionnaire ()-> list:

 definition de la fonction dictionnaire qui prend en compte un dictionnaire...
 ... importé qui découpe les chiffres et ce qui ne correspond pas à des mots...
 ... qui ajoute à la liste vide le reste dudictionnaireet qui retourne ...
 .. une liste contenant les mpots du dictionnaire seuls.

   lexique = []
   hunspell = open("classique-fr",'r')
   hunspell.split("/","0","1","2","3","4","5","6","7","8","9")
   lexique.append (hunspell.split)
   "classique-fr".close 
   return lexique
   
   
def texte ()-> list:

 definition de la fontion texte qui ne prend pas d' argument en compte et ...
 ... qui retourne une liste constituée du texte complet importé . cette liste...
 ... retournée est appelée paragraphe 

   texte = open("texte à corriger","r")
  paragraphe = [].append(texte)
  texte.close
  return paragraphe
  
def extraction_données (t:list)-> list:

 definition de la fonction qui prend en argument une liste t et qui retourne ...
 .. une liste qui sera appelée mot. cette liste sera constituée uniquement ...
 ... des mots du texte , duquel les espaces et la ponctuation ont été decoupés

  mots = [] 
  liste_mot = texte.split(" ",";",",",".","!","?",'"',":"," ")
  mots.append(liste_mot)
  return mots
  
def recherche (mots:list)-> str:

definition de la fonction recherche qui prend en compte une liste et retourne ...
 ... une liste . cette fonction passe dans une boucle deterniministe tous... 
 ...les mots du du texte dans le dictionnaire les compare et ajoute à la liste..
 ... les mots qui ne sont pas dans le dictionnaire
 
  mal_orthographié=[]
   for m in range (len(mots)):
        for m in range ( len(dictionnaire)):
            if m not in dictionnaire:
                 mal_orthographié. append [m]
    return mal_orthographié
 
def main():

 definition de la fonction principale du programme qui comprend un texte sous...
... forme de cahine de caractère qui est importée puis analysée et qui ...
... retourne une liste de most mal othographiés.
    erreur = []
    t = texte ()    
    mots = extraction_données(t)
    resultat = recherche (mots)
    resultat = "les mots mal orthographiés sont{}".format( erreur)
    print ( resultat )



main()
