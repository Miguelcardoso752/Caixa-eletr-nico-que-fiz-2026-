# Caixa-eletr-nico-que-fiz-2026-
o objetivo é você falar quanto dinheiro quer retirar e o programa irá mostrar as notas que você receberá.
print('='*30)
print('{:^30}'.format('BANCO MASTER '))
print('='*30)
valor = int(input('Que valor você quer sacar?: '))
total = valor
ced = 50
totced = 0
while True:
    if total >= ced:
        total -= ced
        totced += 1
    else:
        if totced > 0:
           print(f'{totced} nota de R$ {ced:.2f}')
        elif ced == 50:
            ced = 20
        elif ced == 20:
            ced = 10
        elif ced == 10:
            ced = 1
        if total == 0:
            break
print('-'*30)
print('Volte sempre ao BANCO MASTER!')
print('-'*30)
