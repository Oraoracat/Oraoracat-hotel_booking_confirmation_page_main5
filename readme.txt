1.Jak dodać obrazek wewnątrz przycisku?
                <button><img src="./assets/images/icon-bed.svg" alt="">Your stay</button>
2.Jak wyrównać ikonę/obrazek w przycisku tak by był na równi z tekstem?
                    display: flex;
                    align-content: center;
3.jak wstawić obrazek w prawym górnym rogu bloku tak aby obrazek był widoczny tylko w 
części (jakdyby wychodził poza blok ale tylko ćwiartka tego obrazka została w bloku a reszta
obrazka była niewidzialna)
                    background-image: url(./assets/images/icon-weather.svg);
                    background-repeat: no-repeat;
                    background-position-y: -70%;
                    background-position-x: 105%;
4.Jak sprawić aby jeden element bloku trzymały się  górnej ściany a drugi dolnej ściany bloku?
                    display: grid;
                    align-content: space-between;
5.Co robi position: fix?
                    Sprawia że blok jest niezależny względem układu strony. Trochę
                    jak wyskakujące reklamy bądź te wszystkie ciasteczka na stronach.

                    Ignoruje scrollbar
6.Jak ustawić wysokość bądź szerokość na całe okno przeglądarki?
                    width: 100vw;
                    height: 100hw;

                    width: 95vw; <-- 95% szerokości okna przeglądarki
                    width: 67hw; <-- 67% wysokości przeglądarki będzie szerokością przeglądarki
7.Jak sprawić aby jeden element bloku trzymały się  lewej ściany a drugi prawej ściany bloku?
                    display: flex;
                    justify-content:space-between;
8.Jak dać bloku możliwość wykorzystania całej reszty miejsca które zostało na stronie?
                    flex-grow: 0;
9.









































