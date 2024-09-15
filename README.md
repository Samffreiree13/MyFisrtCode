# MyFisrtCode

# Solicita ao usuário as horas trabalhadas e a taxa por hora
hours = float(input("Digite o número de horas trabalhadas: "))
rate = float(input("Digite a taxa por hora: "))

# Calcula o pagamento bruto
if hours <= 40:
    gross_pay = hours * rate
else:
    regular_pay = 40 * rate
    overtime_pay = (hours - 40) * (rate * 1.5)
    gross_pay = regular_pay + overtime_pay

# Exibe o pagamento bruto
print("O pagamento bruto é:", gross_pay)
