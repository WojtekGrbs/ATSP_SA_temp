# Asymmetric Travelling Salesman Problem optimization project
Authors:
# Opis problemu
Problem asymetrycznego komiwojażera polega na znalezieniu najkrótszej trasy dla podróżującego handlowca, gdzie odległość między dwoma miastami może się różnić w zależności od kierunku podróży. Jest to rozszerzenie klasycznego problemu komiwojażera, które wprowadza dodatkowe wyzwania związane z nierównością kosztów podróży w poszczególnych kierunkach.
# Podejście optymalizacyjne i jego implementacja
#### Symulowane wyżarzanie
Symulowane wyżarzanie to metaheurystyczna technika optymalizacji, inspirowana procesem wyżarzania metali, która pozwala na rozwiązywanie problemów optymalizacji globalnej. Algorytm wykorzystuje losowe ruchy w przestrzeni rozwiązań, akceptując czasami gorsze rozwiązania, aby uniknąć utknięcia w lokalnym minimum. Stopniowo zmniejsza się temperatura, co prowadzi do zmniejszenia prawdopodobieństwa akceptacji gorszych rozwiązań, umożliwiając znalezienie lepszego rozwiązania.
#### Implementacja
Zespół projektowy zaimplementował algorytm symulowanego wyżarzania, gdzie przy początkowej losowej ścieżce Hamiltona losowo zamieniane są miejscami wierzchołki w kontekście kolejności, dla nowo powstałego rozwiązania badany jest jego koszt i na podstawie przyjętej funkcji prawdopodobieństwa i aktualnie panującej temperatury w algorytmie nowe rozwiązanie przyjmowane jest bądź nie.
# Symulowane wyżarzanie
