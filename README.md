agua=600
azucar=1200
aceite=1500
arroz=1250
fideos=790
bebida=1780
chocolate=2500
pan_molde=1340

contador=0

print('responda las siguientes preguntas con si:no')

p1 = input('¿quiere llevar Agua?')
if(p1=='si'):
  n1= int(input('cuanto quiere llevar?'))
  contador = contador+(agua*n1)

p2 = input('¿quiere llevar Azúcar?')
if(p2=='si'):
  n2= int(input('cuanto quiere llevar?'))
  contador=contador+(azucar*n2)

p3 = input('¿quiere llevar Aceite?')
if(p3=='si'):
  n3= int(input('cuanto quiere llevar?'))
  contador=contador+(aceite*n3)

p4 = input('¿quiere llevar Arroz?')
if(p4=='si'):
  n4= int(input('cuanto quiere llevar?'))
  contador=contador+(arroz*n4)

p5 = input('¿quiere llevar Fideos?')
if(p5=='si'):
  n5= int(input('cuanto quiere llevar?'))
  contador=contador+(fideos*n5)

p6 = input('¿quiere llevar Bebida?')
if(p6=='si'):
  n6= int(input('cuanto quiere llevar?'))
  contador=contador+(bebida*n6)

p7 = input('¿quiere llevar Chocolate?')
if(p7=='si'):
  n7= int(input('cuanto quiere llevar?'))
  contador=contador+(chocolate*n7)

p8 = input('¿quiere llevar Pan_molde?')
if(p8=='si'):
  n8= int(input('cuanto quiere llevar?'))
  contador=contador+(pan_molde*n8)

Preferencial =input('es cliente preferencial?')
if(Preferencial=='si'):
  print(f'su total es de : {contador*0.25}')
else:
  print(f'su total es de : {contador}')

efectivo= int(input('indique el efectivo a pagar'))
vuelto=(efectivo-contador)

if(efectivo>=contador):
  print(f' su vuelto es de: {vuelto}')
else:
  print('Dinero insuficiente, Guardias!')
