def avaliador_temperatura():
    try:
        temp_max = float(input("Informe a temperatura máxima do dia: "))
        temp_min = float(input("Informe a temperatura mínima do dia: "))
        
        media = (temp_max + temp_min) / 2
        variacao = abs(temp_max - temp_min)

        print(f"Média das temperaturas: {media:.2f}°C")
        print(f"Variação de temperatura: {variacao:.2f}°C")

    except ValueError:
        print("Erro: Informe apenas números válidos (inteiros ou decimais).")
