<img width="2485" height="635" alt="image" src="https://github.com/user-attachments/assets/8b209f8c-829c-44af-82b5-5d5e6913c1a8" />

```bash
@startuml
' --- Configuración ortogonal y anti-distorsión ---
skinparam linetype ortho
skinparam shadowing false
skinparam nodesep 70
skinparam ranksep 70
skinparam dpi 150
skinparam backgroundColor #FFFFFF

title Módulo: Archivística audiovisual y humanidades digitales

' --- NÚCLEO CENTRAL ---
node "Memoria colectiva" #FEF9E7

' --- PILAR 1: COMPROMISO SOCIAL ---
package "Plano socio-comunitario" #E8F8F5 {
    [Interacción con colectivos] as Social
    [Autenticidad] as Confianza
    [Alfabetización digital crítica] as Alfabet
}

' --- PILAR 2: CAPACIDAD TÉCNICA (Metodología) ---
package "Plano técnico" #EBF5FB {
    [Gestión de obsolescencia] as Obsol
    [IA, RAG, aprendizaje automático] as IA
    [Estándares (OAIS / W3C)] as Estandares
}

' --- PILAR 3: EVIDENCIA PRÁCTICA (Casos en GitHub) ---
package "Casos de estudio" #F5EEF8 {
    [Archivos de memoria social] as GH_Social
    ["#BlackLives", colecciones AV racializadas] as GH_Black
    [Enriquecimiento Watson @ BBC] as GH_Watson
}

' --- RELACIONES ORTOGONALES (Soporte multidireccional) ---

' Conexiones superiores
Social -down- "Memoria colectiva"
Confianza -down- "Memoria colectiva"
Alfabet -down- "Memoria colectiva"

' Conexiones inferiores
Obsol -up- "Memoria colectiva"
IA -up- "Memoria colectiva"
Estandares -up- "Memoria colectiva"

' Conexiones laterales
GH_Social -left- "Memoria colectiva"
GH_Black -left- "Memoria colectiva"
GH_Watson -right- "Memoria colectiva"

footer Profesor Jose Velazquez, MA - Universidad Pablo de Olavide (2025-26)
@enduml
```
