from colorama import init, Fore, Style

# Inicializa o Colorama
init(autoreset=True)

# Lista com os níveis do reservatório
niveis = [
    "Nível 1 - Muito baixo (crítico)",
    "Nível 2 - Baixo",
    "Nível 3 - Médio",
    "Nível 4 - Alto",
    "Nível 5 - Muito alto (alerta)"
]

# Função que define a cor de acordo com o nível
def definir_cor(nivel):
    if nivel == 1:
        return Fore.RED
    elif nivel == 2:
        return Fore.YELLOW
    elif nivel == 3:
        return Fore.GREEN
    elif nivel == 4:
        return Fore.CYAN
    elif nivel == 5:
        return Fore.BLUE
    else:
        return Fore.WHITE

# Simulação dos níveis do reservatório
for i in range(len(niveis)):
    cor = definir_cor(i + 1)
    print(cor + niveis[i])

# Restaura o estilo padrão do terminal
print(Style.RESET_ALL)
