Usuario = input("Enter your username ")
contraseña = input(f"Hello {Usuario} create your password ")
Saldo = 10000

Bucle = True
 
while Bucle:
 print(f"Your amount of money is {Saldo} euros")
 accion = input("What would you like to do, deposit,withdraw or exit ").lower()
 if accion == ("withdraw"):
    Cantidad = int(input("How much "))
    if (Saldo>= Cantidad):
        print("Operation is done")
        Saldo = Saldo-Cantidad
    else: print("Not enough money")
 if accion == ("deposit"):
    Cantidad2 = int(input("How much "))
    Saldo = Saldo + Cantidad2
 if accion == ("exit"):
     print("Leaving")
     Bucle = False
