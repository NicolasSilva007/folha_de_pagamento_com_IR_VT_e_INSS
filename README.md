import math
salarioB = float(input("Sálario: "))
vale = str(input("Vale Transporte S/s: "))

if salarioB <1320.00:
    inss = (salarioB*0.075)
    print (f"Calculo do INSS R${inss}")
    salarioL =  (salarioB-inss)
    print (f"Seu salario Liquido é R${salarioL}")
    
elif salarioB > 1320 and salarioB < 2571.29:
    inss = (salarioB - 1320)* 0.09 + 99
    print (f"Salario do inss R${inss}")
    salarioL = (salarioB - inss)
    print (f"Seu salario liquido R${salarioL}")

elif salarioB >= 2571.30 and salarioB <= 3856.94:
    inss = (salarioB - 2571.29)*0.12 + 112.62 +99
    print (f"Salario do inss R${inss}")
    salarioL = (salarioB - inss)
    print (f"Seu salario Liquido R${salarioL}")
    
elif salarioB >= 3856.94 and salarioB <= 7507.49:
    inss = (salarioB - 3856.94)*0.14 + 112.64 + 154.28 + 99
    print (f"Salario do inss R${inss}")
    salarioL = (salarioB - inss)
    print (f"Seu salario Liquido R${salarioL}")
    
else:
    salarioB >= 7507,49
    inss (salarioB - 7507.49)*0.14 + 112.64 + 154.28 + 99
    print (f"Salario do inss R${inss}")
    salarioL = (salarioB - inss)
    print (f"Seu salario Liquido R${salarioL}")
    
if salarioL > 2112.00 and salarioL < 2826.65:
    ir = (salarioL*0.075)-158.40
elif salarioL > 2826.66 and salarioL < 3751.05:
    ir = (salarioL*0.15)-370.40
elif salarioL > 3751.06 and salarioL < 4664.68:
    ir = (salarioL*0.225)-651.73
else:
    salarioL > 4664.68
    ir = (salarioL*0.275)-884.96

if vale == "S" or "s":
    valvale = (salarioL * 0.06)
    print (f"Seu VT: R${valvale}")
    print (f"Seu salario liquido é: R${salarioL}") 
    
print (f"Seu salario com IR INSS e VALE: R${salarioL-ir-inss-valvale}")
    
