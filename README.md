# potencia-R
def potencia(base, exp):
    if exp == 0:
        return 1
    else:
        r = base
        for x in range(1, exp):
            r = base * r
        return r


def main():
    try:
        base = float(input("Ingrese el valor de la base: "))
        exp = int(input("Ingrese el valor del exponente: "))
        resultado = potencia(base, exp)
        print(f"{base}^{exp} es igual a {resultado}")
    except ValueError:
        print("Por favor, ingrese valores numéricos válidos.")


if __name__ == "__main__":
    main()
