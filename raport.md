# Raport Projektu: Rozpoznawanie Ręcznie Pisanych Tekstów

## Wyniki Testowe i Treningowe

Podczas treningu modelu Convolutional Recurrent Neural Network (CRNN) uzyskaliśmy następujące wyniki:

- Dokładność na zbiorze Testowym: 94.21%
- Metryki dodatkowe: W trakcie treningu monitorowaliśmy wartości funkcji straty dla zbioru treningowego i walidacyjnego oraz porównywaliśmy je, aby uniknąć nadmiernego dopasowania modelu.

## Uzasadnienie Wyboru Techniki/Modelu

Zastosowana architektura CRNN ze względu na jej zdolność do efektywnego przetwarzania sekwencji danych, co jest kluczowe w zadaniu rozpoznawania tekstu. CRNN łączy zalety konwolucyjnych sieci neuronowych (CNN) do ekstrakcji cech z rekurencyjnymi sieciami neuronowymi typu LSTM (Long Short-Term Memory), co pozwala uwzględnić kontekst sekwencji podczas predykcji.

## Strategia Podziału Danych

Dane zostały podzielone na trzy zestawy:

- Zestaw Treningowy: Wykorzystany do trenowania modelu. Składał się z 80% wszystkich dostępnych danych.
- Zestaw Walidacyjny: Wykorzystany do monitorowania procesu trenowania i wyboru najlepszego modelu. Składał się z 10% dostępnych danych.
- Zestaw Testowy: Wykorzystany do ostatecznej oceny wydajności modelu. Składał się z 10% dostępnych danych.

## Opis Danych Wejściowych

Dane wejściowe to obrazy ręcznie pisanych tekstów, w formacie grayscale, o rozmiarze 256x64 pikseli. Zbiór danych zawierał różnorodne rodzaje pisma oraz różne warunki oświetleniowe i jakościowe.

## Analiza Wyników

Analiza wyników wykazała, że uzyskana dokładność modelu na zbiorze walidacyjnym wynosiła 93.15%. Istnieje jednak margines na poprawę, zwłaszcza poprzez dalsze eksplorowanie technik regularyzacji modelu, takich jak dropout, oraz optymalizację hiperparametrów, takich jak współczynnik uczenia się.

W przyszłości proponujemy rozważyć zastosowanie bardziej zaawansowanych technik przetwarzania wstępnego danych, takich jak augmentacja danych, aby zwiększyć różnorodność zbioru treningowego i poprawić generalizację modelu.
