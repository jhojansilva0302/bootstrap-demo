```mermaid
graph TD
    A([Inicio]) --> B[/Mostrar Menú y Precios/]
    B --> C[/Leer cantidades de panes y pasteles/]
    C --> D[subtotal = suma de (cantidades * precios)]
    D --> E{subtotal > 10000}
    E -- Sí --> F[descuento = subtotal * 0.20]
    E -- No --> G[descuento = 0]
    F --> H
    G --> H[total_final = subtotal - descuento]
    H --> I[/Mostrar subtotal, descuento y total_final/]
    I --> J([Fin])
