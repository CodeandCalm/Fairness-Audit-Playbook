graph TD
    A["Inicio: Seleccionar formulación matemática de equidad"] --> B{"¿Cuál es el contexto de aplicación?"}
    
    B --> C["Salud"]
    B --> D["Finanzas"]
    B --> E["Justicia/Legal"]
    B --> F["Recursos Humanos"]
    B --> G["Otro contexto"]
    
    C --> C1{"¿Cuál es la dirección del daño?"}
    D --> D1{"¿Cuál es la dirección del daño?"}
    E --> E1{"¿Cuál es la dirección del daño?"}
    F --> F1{"¿Cuál es la dirección del daño?"}
    G --> G1{"¿Cuál es la dirección del daño?"}
    
    C1 --> C2["Falso Negativo: Daño al paciente"]
    C1 --> C3["Falso Positivo: Recursos desperdiciados"]
    
    D1 --> D2["Falso Positivo: Daño a la institución"]
    D1 --> D3["Falso Negativo: Daño al solicitante"]
    
    C2 --> H["Analizar datos de entrenamiento"]
    C3 --> H
    D2 --> H
    D3 --> H
    E1 --> H
    F1 --> H
    G1 --> H
    
    H --> I{"¿Los datos reflejan sesgos estructurales?"}
    
    I -->|Sí| J["Identificar origen del sesgo"]
    I -->|No| K["Evaluar representatividad"]
    
    J --> L{"¿Qué tipo de justicia priorizar?"}
    K --> L
    
    L --> M["Corregir sesgo histórico"]
    L --> N["Reflejar realidad existente"]
    
    M --> O["Seleccionar métrica de equidad"]
    N --> O
    
    O --> P["Demographic Parity"]
    O --> Q["Equal Opportunity"]
    O --> R["Equalized Odds"]
    O --> S["Predictive Parity"]
    
    P --> T["Medir propiedades estadísticas entre grupos"]
    Q --> T
    R --> T
    S --> T
    
    T --> U["Comparar: Tasas de error, precisión, PPV"]
    
    U --> V{"¿Las métricas son similares entre grupos?"}
    
    V -->|Sí| W["Sistema considerado equitativo"]
    V -->|No| X["Implementar estrategias de mitigación"]
    
    X --> Y["Re-evaluar y ajustar modelo"]
    Y --> V
    
    W --> Z["Monitoreo continuo"]
