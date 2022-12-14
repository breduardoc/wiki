# Como Gerar Executáveis no Linux / Window:
Programa Teste (IMC)
```python
peso = float(input('Digite seu peso (kg): '))
altura = float(input('Digite sua altura (m): '))
imc = peso / (altura * altura)

println('Seu IMC é {}'.format(imc))
println('menor que 18.5 - Abaixo do peso')
println('de 18.5 até 24.9 - Saudável')
println('de 25 até 29.9 - Sobrepeso ')
println('maior 29.9 - Obeso')

```
##
## Para o Linux: <strong>x_Freeze[^1]</strong>
Instalação do pacote:
* ```pip install cx_Freeze```

Compilando via terminal Linux:
* ```cxfreeze imc.py --target-dir calculadora-imc```

Saída esperada no Linux:
```
yan@linux-flrj:~/imc/calculadora-imc> ls
arquivo<imc> pasta<lib> biblioteca<libpython3.6m.so.1.0>
yan@linux-flrj:~/imc/calculadora-imc>
```

Executando no Linux:
```
yan@linux-flrj:~/imc/calculadora-imc> ./imc
Digite seu peso (kg): 90
Digite sua altura (m): 1.80
Seu IMC é 27.777
yan@linux-flrj:~/imc/calculadora-imc>
```

<b>Ps.: Executar com todos os arquivos na mesma pasta</b>
##



## Para o Windows: <strong>pyinstalller[^2]</strong>
Instalação do pacote:
* ```pip install pyinstaller```

Compilando via terminal:
* ```pyinstaller –onefile imc.py```

Saída esperada:
* ```imc.exe```

##
### Refs.:
[^1]: Linux <strong>x_Freeze</strong> :
[ALURA](https://www.alura.com.br/artigos/criando-um-executavel-a-partir-de-um-programa-python)

[^2]: Windows <strong>pyinstaller</strong> :
[HASHTAGTREINAMENTOS](
https://www.hashtagtreinamentos.com/arquivo-executavel-python?gclid=Cj0KCQjwqc6aBhC4ARIsAN06NmNM1X9DDkTDFJLiLAxtMviabn5dPDyabWBFlkYcCoid9VEBxbtGKMIaAn77EALw_wcB)
