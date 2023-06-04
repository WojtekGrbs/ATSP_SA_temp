# Asymmetric Travelling Salesman Problem optimization project
Authors:
# Opis problemu
Problem asymetrycznego komiwojażera polega na znalezieniu najkrótszej trasy dla podróżującego handlowca, gdzie odległość między dwoma miastami może się różnić w zależności od kierunku podróży. Jest to rozszerzenie klasycznego problemu komiwojażera, które wprowadza dodatkowe wyzwania związane z nierównością kosztów podróży w poszczególnych kierunkach.
# Podejście optymalizacyjne i jego implementacja
#### Symulowane wyżarzanie
Symulowane wyżarzanie to metaheurystyczna technika optymalizacji, inspirowana procesem wyżarzania metali, która pozwala na rozwiązywanie problemów optymalizacji globalnej. Algorytm wykorzystuje losowe ruchy w przestrzeni rozwiązań, akceptując czasami gorsze rozwiązania, aby uniknąć utknięcia w lokalnym minimum. Stopniowo zmniejsza się temperatura, co prowadzi do zmniejszenia prawdopodobieństwa akceptacji gorszych rozwiązań, umożliwiając znalezienie lepszego rozwiązania.
#### Implementacja
Zespół projektowy zaimplementował algorytm symulowanego wyżarzania, gdzie przy początkowej losowej ścieżce Hamiltona losowo zamieniane są miejscami wierzchołki w kontekście kolejności, dla nowo powstałego rozwiązania badany jest jego koszt i na podstawie przyjętej funkcji prawdopodobieństwa i aktualnie panującej temperatury w algorytmie nowe rozwiązanie przyjmowane jest bądź nie.
# Dobór parametrów algorytmu
1. Na podstawie odgórnie ustalonego zestawu funkcji chłodzenia oraz prawdopodobieństwa i pewnej puli parametrów badane były osiągi algorytmu dla każdej kominacji z powyższego zestawu. Wszystkie kombinacje parametrów generowane są przez ```Dictionaries_Generators.py``` i zawarte w nim dwie funkcje.
2. Za pomocą skryptu ```1_Gridsearch.py``` uzyskiwane były kolejne wyniki parametrów dla ustalonego zestawu plików-problemów, które zapisywane były w rozszerzeniu ```.csv```
3. Przy pomocy skryptu ```2_najlepszy_zestaw.py``` dla ustalonego problemu tworzony był ranking zestawów parametrów, które pozwoliły wyłonić globalnie najlepszy układ.
# Wyścig
