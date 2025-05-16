mermaid
flowchart TD
    A[Inicio] --> B[Leer n]
    B --> C[Para i = 2 hasta n]
    C --> D[EsPrimo = verdadero]
    D --> E[Para j = 2 hasta i - 1]
    E --> F{¿i % j == 0?}
    F -- Sí --> G[EsPrimo = falso]
    F -- No --> H[j++]
    G --> I[Fin Para j]
    H --> E
    I --> J{¿EsPrimo?}
    J -- Sí --> K[Imprimir i]
    J -- No --> L[i++]
    K --> L
    L --> M[¿i <= n?]
    M -- Sí --> C
    M -- No --> N[Fin]
    