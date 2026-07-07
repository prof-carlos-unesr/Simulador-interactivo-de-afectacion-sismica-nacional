# Simulador Web Interactivo de Afectación Sísmica Nacional

Un simulador web dinámico diseñado para la evaluación y visualización interactiva de escenarios de afectación real sísmica monitoreable desde cualquier lugar de Venezuela. Este proyecto combina metodologías académicas con desarrollo ágil asistido por Inteligencia Artificial.

# 🎓 Contexto Institucional
Institución: Universidad Nacional Experimental Simon Rodriguez (UNESR)
Autor: Prof. Carlos Duarte
Especialidad: Prompt Engineering / Ingeniería de Prompts

🧠 Metodología de Desarrollo (Prompt Engineering)
Este software fue diseñado, estructurado y refinado aplicando técnicas avanzadas de Ingineering de Prompts. El autor actuó como arquitecto de software y director lógico del proyecto, guiando a modelos de IA para la generación precisa del código mediante:
   Estructuración de instrucciones de contexto técnico-académico.
   Refinamiento iterativo de lógica y algoritmos sísmicos.
   Control de calidad y ensamblaje de la arquitectura web.

   🛠️ Tecnologías Utilizadas
   HTML5 / CSS3 (Interfaz de usuario responsiva)
   JavaScript (Lógica interactiva de simulación)

   ⚖️ Licencia y Propiedad Intelectual
Este proyecto está protegido bajo la Licencia Pública General de GNU v3.0 (GPLv3).

Copyright (c) 2026 Carlos Duarte / prof-carlos-unesr@gmail.com

   Condiciones clave:
   Atribución: Cualquier copia o derivado de este proyecto debe dar crédito obligatorio al autor original (Carlos Duarte).
   Copyleft Obligatorio: Si modificas, mejoras o creas un producto comercial basado en este código, estás obligado por ley a liberar tus mejoras bajo esta misma licencia GPLv3. Está prohibido privatizar este código.

   markdown
# Simulador Sísmico Nacional V3.2 🗺️⚡
### Evaluación Interactiva de Vulnerabilidad Estructural y Mitigación de Riesgo Sísmico en Superficie (Normas COVENIN 1756 / FUNVISIS)

![Licencia](https://shields.io)
![Plataforma](https://shields.io)
![Estatus](https://shields.io)

El **Simulador Sísmico Nacional V3.2** es una aplicación web independiente (Single-File App), ligera y de código abierto desarrollada bajo licencia **GPLv3**. Su propósito fundamental es democratizar el acceso a la geofísica aplicada, traduciendo datos instrumentales macros (magnitud y epicentro) en diagnósticos dinámicos de resistencia de materiales directamente en teléfonos inteligentes, promoviendo una cultura preventiva de apropiación social de la ciencia.

---

## 🌐 1. Complementariedad Institucional: ¿Cómo aporta valor?

Las redes de monitoreo sísmico nacionales y globales proveen reportes instrumentales de macro-parámetros esenciales. Esta aplicación **complementa de forma inercial dichos sistemas**, ya que procesa algoritmos sismorresistentes específicos en superficie, permitiendo al ciudadano común, escuelas y cuerpos de bomberos simular el impacto real sobre las tipologías constructivas del territorio nacional.

### Algoritmos Científicos Integrados en el Código:
1. **Interpolación Matemática IDW (Inverse Distance Weighting):** El motor en JavaScript calcula en un enrejado bidimensional de 64 ejes compass el coeficiente de suelo continuo, deduciendo la degradación de la onda de forma asimétrica según la topografía regional.
2. **Superposición Inercial de Dobletes Sísmicos:** Ante secuencias sísmicas complejas múltiples (rupturas sucesivas de precursores o réplicas mayores), el código ejecuta una raíz cuadrada de la suma de cuadrados (SRSS) para modelar la transferencia de estrés tectónico y estimar la aceleración horizontal combinada (PGA).
3. **Física del Retardo de Onda S:** Basándose en una velocidad promedio de propagación cortical en el norte de Sudamérica de 3.5 km/s, el software calcula el desfase de viaje para estimar en segundos la duración de la sacudida por atrapamiento de ondas en cuencas.

---

## 📊 2. Tabla Unificada de Umbrales en Roca Firme (Marco COVENIN 1756)

La aplicación automatiza el comportamiento de los materiales basándose en la Aceleración Máxima del Suelo (PGA). El daño estructural severo en construcciones promedio inicia al superar el umbral del **10% de la gravedad (0.10g)**.

| Magnitud (Mw) | Categoría de Profundidad | Rango Sísmico (h) | Radio de Daño Base* | Sistema Constructivo Vulnerable en Venezuela | Método de Refuerzo Normado (FUNVISIS) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **6.0 a 6.4** | Superficial | 0 a 30 km | **Hasta 18 km** | Casas coloniales/tradicionales de adobe, tapia y bahareque. | Malla electrosoldada unida por conectores pasantes y mortero. |
| **6.5 a 6.9** | Superficial | 0 a 30 km | **Hasta 32 km** | Paredes de bloques de arcilla hueca o tabelones sin amarrar. | Confinamiento perimetral obligatorio con machones y vigas. |
| **7.0 a 7.4** | Superficial | 0 a 30 km | **Hasta 60 km** | Edificios antiguos de concreto o con plantas de "Piso Blando". | Encamisado (chaqueteado) de columnas (acero/CFRP) y muros de corte. |
| **7.5 a 7.9** | Superficial | 0 a 30 km | **Hasta 95 km** | Estructuras informales altas (barriadas) y losas sin vigas. | Rigidización con pórticos de acero en diagonales (Cruces de San Andrés). |

*\*Nota Geológica:* Los radios en kilómetros representan la medición base sobre roca firme. El software deforma y amplifica este radio en tiempo real aplicando coeficientes locales de **Efecto de Sitio (Suelos)** y **Directividad** de la falla.

---

## 📍 3. Caso de Estudio Inicial: Empezó siendo monitor local/regional  Eje Cojedes (Tinaquillo y Tinaco) pero en esta última version se ha extendido el monitoreo a las principales localidades estadales de Venezuela

El simulador posee un HUD analítico estratégico para Venezuela para modelar el comportamiento del sismo costero de **7.5 Mw**:
*   **Límite Crítico Interno:** Demuestra como ejemplo, que Tinaquillo y Tinaco se ubicaron a ~90 km de distancia, en la frontera misma del radio destructivo de 95 km. Debido a su factor de suelo aluvial intermedio (~1.1), experimentaron una leve amplificación local, provocando las fisuras documentadas en mampostería informal y en la Iglesia Nuestra Señora del Socorro.
*   **Vector de Directividad:** Justifica científicamente por qué Cojedes evitó una catástrofe total: la ruptura de la Falla de San Sebastián empujó el vector principal de energía hacia el Este (causando el desastre por resonancia y "Efecto Gelatina" en el Valle de Caracas y La Guaira).
*   **Alerta de Peligro Absoluto:** El software advierte por ejemplo que, si bien la zona resistió el evento de la costa, una activación del tramo central de la **Falla de Boconó** (localizada a solo ~15 km en línea recta de Tinaquillo) los colocaría plenamente en el epicentro de destrucción, obligando a priorizar el reforzamiento estructural preventivo.

---

## 🛠️ 4. Instrucciones para Ejecución Local e Implementación

Al ser una aplicación diseñada en un único archivo plano e independiente (`index.html`), no requiere servidores pesados, bases de datos SQL complejas ni dependencias locales de Node.js, garantizando su portabilidad en zonas de desastre con baja conectividad.

### Requisitos Previos:
Tener instalado un navegador web moderno compatible con HTML5/ES6 (Google Chrome, Mozilla Firefox, Safari).

### Pasos para clonar y ejecutar:
```bash
# 1. Clonar el repositorio desde GitHub
git clone https://github.com

# 2. Ingresar al directorio del proyecto
cd TU_REPOSITORIO

# 3. Abrir el archivo index.html en tu navegador predeterminado
# (En Windows)
start index.html
# (En Mac)
open index.html
```

---

## 📝 5. Nota Informativa, Autoría y Descargo de Responsabilidad

*   **Autoría:** Hecha por Carlos Duarte con apoyo de la IA Gemini de Google.
*   **Control de Calidad:** Verifique la información antes de usarla o compartirla.
*   **Descargo de Responsabilidad Legal:** Esta aplicación tiene un carácter estrictamente educativo (educacion antisismica), didáctico y de concientización preventiva para fomentar una cultura antisísmica resiliente; no pretende bajo ningún concepto sustituir las informaciones de organismos oficiales del Estado (FUNVISIS / Protección Civil) o dictámenes de ingenieros estructurales colegiados, ni mi formación profesional está relacionada con este tema. 
*   **Propósito del Proyecto:** Ayudar a comprender la física de los eventos sísmicos recientes y entender el contexto de vulnerabilidad de las pricipales localidades venezolanas entre las principales zonas sísmicas a nivel nacional, demostrando que con el apoyo de la IA es rápidamente factible la apropiación y traducción social de cualquier evento científico complejo. 

---
*Desarrollado en Venezuela como un aporte a la gestión de riesgo civil comunitario. Licencia GPLv3 - Software Libre.*
Usa el código con precaución.


