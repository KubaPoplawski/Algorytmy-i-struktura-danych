lista_zakupow: list[str] = []


def dodaj_produkt(produkt: str) -> None:
    if produkt in lista_zakupow:
        print(f"'{produkt}' jest już na liście zakupów.")
    else:
        lista_zakupow.append(produkt)


def usun_produkt(produkt: str) -> None:
    if produkt in lista_zakupow:
        lista_zakupow.remove(produkt)
    else:
        print(f"'{produkt}' nie znaleziono na liście zakupów.")


def posortuj_liste() -> None:
    lista_zakupow.sort(key=str.lower)


def wyswietl_liste() -> None:
    if not lista_zakupow:
        print("Lista zakupów jest pusta.")
        return

    print(f"Lista zakupów ({len(lista_zakupow)} produkty/ów):")

    for i, produkt in enumerate(lista_zakupow, start=1):
        print(f"{i}. {produkt}")
