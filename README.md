# Rock_Paper_Scissors
Rock Paper Scissors in Python
def rootFunction():
 import random
 import sys
 def mainFunction():
  global cho1, cho2
  print "========== Choice =========="
  cho1 = raw_input(p1 + "'s Choice: ")
  cho2 = random.choice(comp)
  print "Computer: ", cho2
  main()
 def winCheck():
     global p1, p2
     if p1s == 5:
         print p1, "Is The Winner!!"
         pla = raw_input("Do You Want to Play Again? (Y / N) ")
         if pla == "Y":
             rootFunction()
         elif pla == "N":
             sys.exit()
     elif p2s == 5:
         print p2, "Is The Winner!!"
         pla2 = raw_input("Do You Want to Play Again? (Y / N) ")
         if pla2 == "Y":
             rootFunction()
         elif pla2 == "N":
             sys.exit()
 def main():
  global p1s, p2s
  if cho1 == cho2:
      p1s = p1s + 0
      p2s = p2s + 0
      print "========== Score =========="
      print p1, ":", p1s
      print p2, ":", p2s
      winCheck()
      mainFunction()
  elif cho1 == "R" and cho2 == "P":
      p2s = p2s + 1
      print "========== Score =========="
      print p1, ":", p1s
      print p2, ":", p2s
      winCheck()
      mainFunction()
  elif cho1 == "R" and cho2 == "S":
      p1s = p1s + 1
      print "========== Score =========="
      print p1, ":", p1s
      print p2, ":", p2s
      winCheck()
      mainFunction()
  elif cho1 == "P" and cho2 == "R":
      p1s = p1s + 1
      print "========== Score =========="
      print p1, ":", p1s
      print p2, ":", p2s
      winCheck()
      mainFunction()
  elif cho1 == "P" and cho2 == "S":
      p2s = p2s + 1
      print "========== Score =========="
      print p1, ":", p1s
      print p2, ":", p2s
      winCheck()
      mainFunction()
  elif cho1 == "S" and cho2 == "R":
      p2s = p2s + 1
      print "========== Score =========="
      print p1, ":", p1s
      print p2, ":", p2s
      winCheck()
      mainFunction()
  elif cho1 == "S" and cho2 == "P":
      p1s = p1s + 1
      print "========== Score =========="
      print p1, ":", p1s
      print p2, ":", p2s
      winCheck()
      mainFunction()

 global p1s, p2s
 global p1, p2
 p1s = 0
 p2s = 0
 comp = ["R", "P", "S"]
 p2 = "Computer"
 p1 = raw_input("Input Your Name: ")
 print "=============== Welcome to Rock Paper Scissors ==============="
 print "Rock - R"
 print "Paper - P"
 print "Scissors - S"
 print p1, 'vs', p2
 mainFunction()
rootFunction()

