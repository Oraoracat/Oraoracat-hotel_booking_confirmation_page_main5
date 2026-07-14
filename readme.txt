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
9.Jak zrobić cień? 
                    box-shadow: h-offset v-offset blur spread color;

                    box-shadow: -5px 10px 10px var(--Neutral400);
10.Jak zrobić Animacje? 
                    .booking_cards:hover .receipt_card
                    {
                    position: relative;
                    animation-name: NaLewo;
                    animation-duration: 2s;
                    animation-fill-mode: forwards;
                    }

                    @keyframes NaLewo {
                    0%   {right:0px;}
                    100%  {right:100px; transform: rotate(5deg);}
                    }
Szczerze niektóre nazwy już kojarzę ale 33% wciąż stanowi zagadkę.
11. Miałem problem z przyciskami i tutaj wykorzystałem AI Gemini za co mi trochę wstyd. Nie wiedziałem jak po zaznaczeniu przycisk miałby się podświetlać.
                        <script>
                        // I had to help myself with AI here, because I dont remember JS
                        const buttons = document.querySelectorAll('.option-btn');

                        // 2. Dodajemy zdarzenie kliknięcia do każdego z nich
                        buttons.forEach(button => {
                            button.addEventListener('click', function() {
                            
                            // 3. Usuwamy klasę 'active' ze wszystkich przycisków w grupie
                            buttons.forEach(btn => btn.classList.remove('active'));
                            
                            // 4. Dodajemy klasę 'active' do klikniętego przycisku
                            this.classList.add('active');
                            
                            });
                        });
                        </script>
Na marginesie każdy z przycisków jest w klasie .option-btn lub .option-btn active.












































