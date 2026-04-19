##ZADANIE 1

LICZBA_DNI = 7
DNI_TYGODNIA = ["Poniedziałek", "Wtorek", "Środa", "Czwartek",
                "Piątek", "Sobota", "Niedziela"]

temperatury: list = [None] * LICZBA_DNI


def wpisz_temperatury() -> None:
    przykladowe_temp = [12.5, 14.0, 9.8, 11.3, 16.7, 20.1, 18.4]

    for i in range(LICZBA_DNI):
        temperatury[i] = przykladowe_temp[i]


def oblicz_srednia() -> float:
    suma = sum(temperatury)
    srednia = suma / len(temperatury)
    return round(srednia, 2)


def najcieplejszy_dzien() -> tuple[str, float]:
    maks_temp = max(temperatury)
    indeks = temperatury.index(maks_temp)

    return (DNI_TYGODNIA[indeks], maks_temp)


if __name__ == "__main__":
    wpisz_temperatury()

    print("=== Temperatury w tygodniu ===")
    for i in range(LICZBA_DNI):
        print(f"  {DNI_TYGODNIA[i]:<14}: {temperatury[i]} °C")

    srednia = oblicz_srednia()
    print(f"\nŚrednia temperatura: {srednia} °C")

    dzien, temp = najcieplejszy_dzien()
    print(f"Najcieplejszy dzień: {dzien} ({temp} °C)")
