# Validador Curricular ITI

**Motor de verificación formal para trayectorias académicas** en la carrera de Ingeniería en Tecnologías de Información.

## Modelo Matemático

El sistema transforma el reglamento curricular en un modelo ejecutable:

| Componente | Descripción |
|---|---|
| **Conjuntos** | U, K, F, Pk, S, A, C, hab(A) |
| **Relaciones** | R1 (prerrequisito), Rv (inscripción válida), Rd (dependencia), Rf (facultad), Rs (carrera) |
| **Funciones** | req(m), pct(A), hab(A), val(C) |
| **Lógica** | V(p,q,r) = p ∧ q ∧ r, tabla de verdad, leyes lógicas |
| **Autómata** | AFD M = ⟨Q, Σ, δ, q₀, F⟩ con 5 estados y cortocircuito lógico |
| **Lenguajes** | Σ = {INS(m), APR(m), REP(m)}, L ⊆ Σ*, L3 ⊆ 𝒫(Pk) |

## Contenido

- `index.html` — Aplicación interactiva (100% generada por IA)
- `data/malla_ITI.json` — Malla curricular ITI (41 materias, 8 niveles)
- `docs/` — Documentación del modelo formal

## Funcionalidades

- **Grafo de prerrequisitos** (R1) con visualización interactiva D3.js
- **Simulador AFD** con 5 estados y cortocircuito lógico
- **Diagrama de conjuntos** (A, C, hab(A)) con métricas en tiempo real
- **Validador de inscripción** con chequeo de prerrequisitos y créditos
- **Tabla de verdad y leyes lógicas** aplicadas al dominio académico
- **44 materias** reales de la malla ITI con 8 niveles y prerrequisitos reales

## Uso

Abre `index.html` en cualquier navegador web. No requiere servidor ni instalación.

## Licencia

MIT
