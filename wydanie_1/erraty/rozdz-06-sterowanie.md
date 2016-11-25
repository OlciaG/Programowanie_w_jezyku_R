# Erraty i uwagi do rozdziału 6      #
## Modyfikacja przepływu sterowania ##


-   **s. 93, w. -4**:

    JEST: ~~*gdzie `warunek` jest wektorem logicznym (...)*~~;

    POWINNO BYĆ: *gdzie `warunek` jest taki, że `as.logical(warunek)`
    daje dokładnie jedną wartość `TRUE` albo `FALSE`*.


-   **s. 98, ciekawostka**:

    JEST: ~~*zwraca zwraca*~~;

    POWINNO BYĆ: *zwraca*.


-   **s. 100, w. -5**:

    JEST: ~~*wektorem jednoelementowym*~~;

    POWINNO BYĆ: *wektorem jednoelementowym lub pustym*

    Ponadto w kodzie moglibyśmy napisać `stopifnot(is.atomic(x), is.vector(x))`
    zamiast `stopifnot(is.numeric(x))`. Wówczas nasze sortowanie zadziała
    także np. dla wektorów napisów.


-   **s. 101, ciekawostka**:

    Maksymalna liczba dopuszczalnych zagnieżdzonych wywołań funkcji
    określona jest przez opcję globalną "expressions".
    W przypadku jej przekroczenia zgłaszany jest błąd
    `Error: evaluation nested too deeply: infinite recursion`.

    Ponadto w Lispie dostępne jest *makro* `loop` (faktycznie nie jest ono
    wyrażeniem).


-   **rozdz. 6.2.1 (wielokrotnie)**:

    JEST: ~~`warunek`~~, ~~`wyrażenie`~~;

    POWINNO BYĆ: *`warunek`*, *`wyrażenie`* (krój maszynowy pochylony)


-   **rys. 6.4**:

    W druku zniknęła strzałka łącząca romb *`warunek`* (z lewej strony,
    obok `TRUE`) oraz prostokąt *`wyrażenie`*.


-   **s. 103, funkcja moja_sum() wersja 2**:

    Drobna uwaga:
    Warunek `stopifnot(is.logical(na.rm), length(na.rm) == 1, !is.na(na.rm))`
    można ewentualnie zastąpić `stopifnot(identical(na.rm, TRUE))`
    (choć nie jest to równoważny zapis, czasem używa się go w praktyce).


-   **s. 104, w. -14**:

    JEST: ~~*Oryginalna funkcja `any()` działa tak pięknie*~~;

    POWINNO BYĆ: *Oryginalna funkcja `any()` nie działa tak pięknie*


-   **s. 106, w. -9**:

    JEST: ~~*w której wyrażeniu się ono znajduje.*~~;

    POWINNO BYĆ: *w której `wyrażeniu` się ono znajduje.* (krój maszynowy pochylony)

