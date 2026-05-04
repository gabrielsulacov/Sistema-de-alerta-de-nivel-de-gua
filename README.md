# Sistema-de-alerta-de-nivel-de-gua
**from colorama import Fore, Style

# Lista de níveis e situações do reservatório
niveis_reservatorio = [
    {"nivel": 1, "situacao": "Muito baixo (crítico)"},
    {"nivel": 2, "situacao": "Baixo"},
    {"nivel": 3, "situacao": "Médio"},
    {"nivel": 4, "situacao": "Alto"},
    {"nivel": 5, "situacao": "Muito alto (alerta)"}
]

def definir_cor_alerta(nivel):
    # Retorna a cor correspondente ao nível informado
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

print("=== SISTEMA DE MONITORAMENTO DO RESERVATÓRIO ===\n")

# Percorre a lista para exibir cada nível com sua respectiva cor
for dado in niveis_reservatorio:
    nivel_atual = dado["nivel"]
    mensagem = dado["situacao"]
    
    cor = definir_cor_alerta(nivel_atual)
    
    print(cor + f"Nível {nivel_atual}: {mensagem}")

# Restaura o estilo padrão do terminal após a execução
print(Style.RESET_ALL)**
