---
terms: ["scalability"]
summary: "Потенциал роста Monero, требуемые ресурсы и методы повышения эффективности"
---

### Основная информация

У Monero нет жёстко закодированного максимального размера блока, что означает, что в отличие от Bitcoin, у этой криптовалюты нет предельного размера блока, составляющего 1 MB, что препятствует масштабированию. Тем не менее в протокол встроен механизм наложения штрафа на вознаграждение за блок, что позволяет избежать появления блоков слишком большого размера. Размер нового блока (new block's size — NBS) сравнивается со средним размером M100 последних 100 блоков. Если NBS > M100, размер вознаграждения за блок снижается в квадратической зависимости от того, насколько NBS превышает M100. Например, если NBS на [10%, 50%, 80%, 100%] больше M100, номинальный размер вознаграждения за блок снижается на [1%, 25%, 64%, 100%]. В целом запрещается генерировать блоки, размер которых превышает 2*M100, а на вознаграждение за блоки, размер которых меньше либо равен 60 kB, обычно не налагается какого-либо штрафа.
