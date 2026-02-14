# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 1 - Modelado de Proceso del Cliente con BPMN_

## 👥 Integrantes del equipo
- David Santiago Medina (davidmebu@unisabana.edu.co)
- Santiago Navarro (santiagonacu@unisabana.edu.co)
- Jacobo Pacheco (jacobopama@unisabana.edu.co)
- Juan Diego Martínez (juandmaes@unisabana.edu.co)

## 🧠 Descripción general del trabajo

Modelar el proceso de negocio de dos clientes mediante la notación BPMN, tomando como base las actividades realizadas, los actores involucrados y el flujo del proceso. Dicho modelo se representará a través de eventos, compuertas (gateways) y actividades, con el fin de obtener una comprensión general y estructurada del proceso.

## 🔧 Proceso de desarrollo

Se inició socializando el funcionaminto paso a paso del proceso del negocio, identificando los distintos elementos del BPNM presentes en el proceso.
Se utilizó la plataforma draw.io para generar el diagrama de decisión.
En un primer instante, modelamos las acciones que el usuario podía realizar y fuimos agregando los elementos de la arquitectura que fueran necesarios para estas acciones.

# Análisis del Modelo Propuesto

## 1. Estructura del modelo

El modelo se estructura a partir de dos actores principales representados en diferentes *pools* del diagrama BPMN:

- **Empresa cliente**, responsable de solicitar los servicios médicos ocupacionales para sus candidatos o trabajadores.
- **ACR Vital Laboral S.A.S.**, entidad encargada de ejecutar los exámenes médicos requeridos.

El proceso inicia cuando la empresa cliente realiza la redacción y envío de la orden de servicios. Posteriormente, ACR recibe la solicitud, confirma la asistencia y registra la información en la plataforma externa **Biofile**, utilizada para la gestión de historias clínicas y la generación de certificados médicos.

El flujo contempla tiempos de espera asociados al agendamiento y realización de los exámenes, así como una compuerta inclusiva que permite la ejecución de uno o varios tipos de exámenes según la necesidad del caso (ocupacional, optometría, fonoaudiología, laboratorio y psicológico). Finalmente, los resultados son revisados y se determina si existe alguna solicitud o problema que requiera solución antes del cierre del proceso.

---

## 2. Representación de las necesidades del cliente

El modelo refleja las necesidades del cliente mediante un flujo donde:

- La empresa cliente envía a sus trabajadores o candidatos para la realización de exámenes médicos.
- ACR Vital Laboral gestiona integralmente el proceso clínico y administrativo.
- Los resultados quedan disponibles para que la empresa cliente pueda revisarlos y tomar decisiones relacionadas con procesos de contratación, renovación laboral o seguimiento ocupacional.

De esta manera, el diagrama evidencia que la necesidad principal del cliente es obtener evaluaciones médicas ocupacionales confiables, delegando la ejecución operativa y técnica a la empresa prestadora del servicio.

---

## 3. Supuestos considerados en el modelo

Para la construcción del modelo se establecieron los siguientes supuestos:

- Se asumió que el cliente principal corresponde a una empresa que agenda previamente el servicio para una fecha específica, aunque en la realidad también puedan atenderse pacientes particulares sin programación previa.
- Se consideró que los requerimientos médicos del cliente son generales y no incluyen necesidades altamente especializadas o procesos personalizados fuera del flujo estándar.
- Se asumió el uso obligatorio del software externo **Biofile** como sistema central para el registro, almacenamiento y generación de certificados médicos.
- El proceso modelado representa un flujo estándar, sin contemplar excepciones complejas como reprogramaciones múltiples, cancelaciones o evaluaciones médicas extraordinarias.


El modelo propuesto ...

## 📈 Diagrama final entregado
<img width="1861" height="985" alt="image" src="https://github.com/user-attachments/assets/3c7594e6-6b23-49a7-9e56-1c41cee96342" />

[>enlace al modelo-final.drawio](https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=Untitled%20Diagram.drawio&dark=auto#R%3Cmxfile%3E%3Cdiagram%20name%3D%22Page-1%22%20id%3D%22VaXwmf848Cjp3PBgjqG1%22%3E7V1bc6O4Ev41rjrnIS7E3Y%2BT28xUzWyyycPuPp2SQbF1gpEP4MTZX38kQDYIGStYYLw1yUOgjQB3t75u9UWZWDer7dcErpc%2FSYiiiWmE24l1OzFN07YA%2FcMoHwUFWLZRUBYJDkvanvCM%2F0YlkV%2B2wSFKaxdmhEQZXteJAYljFGQ1GkwS8l6%2F7IVE9aeu4QI1CM8BjJrUP3CYLQuq7xh7%2BjeEF0v%2BZGCUn6wgv7gkpEsYkvcKybqbWDcJIVlxtNreoIhxj%2FOlGHd%2F4NPdiyUozlQGZLb7%2FhP9fPvf6s3%2B%2Bvsfj4%2Fe6vZKcpeSlGYfnAcJ2cQhYrcxJtb1%2BxJn6HkNA%2FbpOxU7pS2zVUTPAD0sRr%2FBaFOOLgkoydC28oTyJb8iskJZ8kEvWVb4aHI1ed8zHbhuSSzv45WnXLf4GFjKfLG7954t9KDkzCe45Bf3RWFDV9rYhuLwC9NAehaTmBKvQ5gucz6COs%2FqDKa3TD7%2BZCdTYM844a%2BcYACPE2631etvP%2FjZFme1wfScjQVTw7DL8%2F1QdlId%2BYgSTHmGkuq9RaJUxO3y5PMlQRHM8FudjRUZOy0izJ9AOQo%2FKhesCY6ztPICj4yw1xHg15XEdF1BHYo7qo22PK%2F%2BfinZJAEqR1Un35EbNXQ1g8kCZY0b5eq642l3DQaWisbSGZrVNVM22dMsIa%2FohkQk2av2C44igQQjvIjpaUCfyHTnmmEAptD6pfxghcOQPVrQ%2F4Z63a3WCUohJd5EmN2sE6QAIIEU0IoopuH0hCjAVUKQKKJ2Dh0HXZiuC%2BP3greMj9eLBIaMVS1SihhrrkKYvP5rYlr3%2Bc%2FEpF%2FHMoz7e8v6tzYwd5qMd%2Bp8Nw2B8ZYGxge3CMz%2FfHHW%2FzGurp6enDefpFecy0pYnk%2FuFinuTHtFZPS%2Bz%2BUpSbIlWZAYRnd7qqDs%2B2t%2BELIuxflflGUfpS8ENxmpC7tiH5yadThiGYp3LYCmeNntt%2Bv18mqTxdcPL8Cxf%2Ft9vn29AgckKoVubTht2U4daUVv5nPX13G9A4pKlce9fOVRVQL7HEpg26KxbleCI9efrAStclP1mQ%2BZUe0%2Bsyuxb6aAszMRZ%2Ftymfl3uEiH4wmFMAgwiSmZJCFif0PEXh0lb5h%2BkHYSkNUUkLCi4Si2k4%2Fdlx10bZ1QZo8DyqTf9FQkO20a2JcLFo6ojJY51aCOUntzyWhxF79hwhFijZKUaTFjEnv7TbBJUnaqBy%2FEBYtj1t0g0%2FZ6kxEohVSG2uCcy0XJIC4oF9d6dPf4ekLEURtosHMt3nL9y7dyT8vyrnc%2BaueTZL2ryqZ0CdfscIXSNI%2FWVllTOSSbLMIxnfk8EsxmawTnKHokKc6YOZfM9h%2FCBXOSZWSlgg8Zs1O64p1NUfAlMA9NTOszHfQ2zS86VFRiMffa1vQpDLGSBBFdGCz6bEJozzY1zCG5z1ZK5rM%2BW8sK73yxi3pcexfIUI5dtLhbAzh7rSxtnznpK8qCZfm98hUxSu7eEFsYFzzaJYqMasrAqDPy6MyaUAAx2O9JICjHPCnSNubwDre3C5YcnJKXFxygKXUfArTO0mkQkeBVG4LylVJlotp1BG1EC3rLFykh6IVk1exZX1xyu6FZG8f1Zt8MrwpSV5Rg%2BMrZt2JwmXwzprOZqTP5dhQJLanGnD1JdziU59bVzjOEh6hm2hxQv5Ervm3fmTYlIzBS9%2BnLzVMnYOmQW3Oc3lI8n0nXHw1tSZBlPFH6gbydVs70Gdp6Qm84LeKwuTt%2FUzryBo7TDGcbFqPtGFxRiZb79SWX4%2Ffl2Zuzbip7WCtGqrHOQBrbxphf7vlFuOeOryWUKZ1vfFWvZb45I55v4KwTzunfQkxMN2KeVIjf6OGCHVK9f8HJCpYJvDwsD1OcZigOMMwVrKSiLVyhGKWTIlifIDpJ%2FoYJvyf9zpXb9mVlRIe1PyvDi3H1WJmzqL2%2B%2BJGUQ0M5VK0c7dehWmBmm7hDtaZfDL4QOlvoyTUm1ER1q66TKbpVV3RXXAHoUHQ5J5Wq67gBDD6otQxRYh3n57xg%2Fo%2F5jgCD10UukofC6HL7XygwcLQZUP9oIBoYQhWdryN0I2fwTIXBI13k3l4zXf%2F%2BcP%2F9x10nURzPCTREMdMhisOQdRQ0lmQ136RDxRkluurXGbRroOBY4PXFH7ujqydfp43J5nmajJ51IDSo3erJ5dPRKRm%2FfHSJxzqreMx%2Fqni0TZ%2Bhco5y%2BXTMCY9HPqps9s7K5o7lkuNhc98o5Z9TPKaKE3T2cqtd%2BWQ1l7Yjcs%2FItRg01RdKe5J21nk6%2FaOzJEsO9cMAPZp9agTtSEZUnsUElpiG99pbIYDhtA7opyFmgBTQMwvULVCMEhaiCDBKEkbJ43dLnGYkwbBbOb5CbA5YgwXnXEfjPBxzPf5QEek2xvxKAY0yBeQbYjV7X7NtgFBrss9d52AVMEFR%2FlLVYQmHojJ1hcJK70A1GDs%2FJRjrSTwNMRw7E3vBTL8%2FL8PtuIXCeLtp95VezqSyy8KkrcjrLJ6EyQs1hPrkg56Ew4UlH3BsywSqSEKpujlrZHKV901wXLHwvWGC9RV0yQOsak7OsBFWr%2Bm7eILrAhrzu798ulrRW%2FcFmNq%2BBff3Bv0Zct%2BChpuupaFWzmIlkzXSlMu3ArKixSbOu%2BJIhAOcbUJ6zKzfOiHzCOVmr%2Fy4qOyij7zvJDlLYv5A3dcAprBgMvtL0SilI0cqOkmBxW8PhyokGpdy0jwRKRqKKxTycI2Gd7M3CPQuWMjP3%2FsSABDqui0dfWtyF%2FMzNZQX4WJO1BbU4NQEUTe%2F0nXrfplreO2unDiA74l1cIBptg445oi6pvwFP%2B%2BE7tozdyhii65U306or6LLJ0baSrPLl6OHrXRPwbbhKuHAZ7DiWIsAN%2B%2Fy5qMggmmKg0lby1G5lOSLx0pi5nC%2FUM%2BNlIbEERhB%2F5B8gjb2bWvbB6g5Wig8tlzh%2FVRxQnQ2LHHXgZ5BwuwYQm7d2OBSTWVLz8q5gs%2BOzhC%2FZZ5XPqfCjjw8f2oW%2BYABB4IBd8Xuwp5nJhdWn%2Bb7Li9mp7SHYLOGJ3RGybadEUz1TCzl1bG%2FinzOmDrnzEia%2BfrR%2FdN6AwZI5T6ss%2FxtcTcXsote6tjPRq6XOuuurLPla3uAWluE2sauYX2D7QB7rt2TmMBNiElEFgOqc48tcY7OCjfL%2B%2BWc6AZopfjiaVr9A85JAllJjbbNko6ptNtbwsTpuL9IS3njL4XWqdADhLQeUxzkEB0Mp9Buj23Ll9x29VR011YjjPTd88jiilXwVbpxNUnKqEvKtwRr2tsm87aaao%2BtKavhuzmulh1f5TxS0uXLqNkGwGkWbXvutLdko9Nxi5tWSZwt0mfYZt2%2BWb51xMIpbo11uGj5bDFArTu9XFQPvqLMWjq6h85xegIezqwBaup59mHEeWwwUQzN50jZIvnBk9Zivdas3BPjcFtF%2B4BjOWjLnU1nlZ96ZaUrKblVTkobbuPNGgan50iLq3OJdVFYpmhqTi7NOK0ixtMoHnDu3i7DrYvI1WRvWgpazyU47%2FL%2FOcellMc7YunAzGqFXfF6x5t9wh40Rg9cy%2B4pLUxHGkC4o0u8vAlwCdOM%2FS3%2B12y%2BpRdcoDiEobYoj19CJ9%2BbjhcMHe5o0Df5O64QWgV%2BGZNfAZi9s8YsfSVXfOzzp2hH20QrHNfCcboDcMIk8nx7sEnkm%2F8EQZ0f6Fy7SwSQnu7%2Fr3Vhu%2Fb%2FHty6%2Bz8%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E)

## 📋 Tabla de actores, entidades o componentes (si aplica)

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Empresa Cliente | Actor | Organización que solicita la realización de exámenes médicos ocupacionales para sus trabajadores o candidatos. | Cliente |
| ACR Vital Laboral S.A.S. | Actor | Empresa encargada de realizar los exámenes médicos y gestionar el proceso clínico y administrativo. | ACR Vital Laboral |
| Biofile | Sistema | Plataforma externa utilizada para registrar historias clínicas y generar certificados médicos. | ACR Vital Laboral |
| Orden de servicios | Entidad | Documento enviado por el cliente para solicitar los exámenes médicos. | Empresa Cliente |
| Correo institucional | Medio de comunicación | Canal mediante el cual se recibe la orden de servicio. | Empresa Cliente / ACR |
| Personal evaluado | Entidad | Trabajadores o candidatos que serán sometidos a evaluaciones médicas. | Empresa Cliente |
| Exámenes médicos | Proceso | Conjunto de evaluaciones médicas realizadas según necesidad. | ACR Vital Laboral |
| Certificado médico | Entidad | Documento final con el concepto de aptitud laboral del trabajador. | ACR Vital Laboral |
| Solución de solicitud o problema | Proceso | Actividad realizada cuando se detecta una novedad o inconsistencia. | ACR Vital Laboral |


## 🔍 Investigación complementaria
### Tema investigado:
Buenas prácticas en el diseño de diagramas BPMN

Importancia del modelo de amenazas STRIDE

Comparación entre TOGAF y C4


### Resumen:
## Buenas prácticas en el diseño de diagramas BPMN

El diseño de un diagrama BPMN debe priorizar la simplicidad, claridad y facilidad de comprensión, utilizando los estándares oficiales de notación para garantizar una correcta interpretación por parte de todos los interesados. Es importante emplear etiquetas claras y una estructura organizada que permita dividir el proceso en procesos principales y subprocesos cuando exista mayor complejidad. Asimismo, se debe documentar adecuadamente el modelo, validar su funcionamiento y definir con precisión los eventos de inicio y fin del proceso. El uso de pools y carriles permite establecer responsabilidades entre los participantes, mientras que la correcta aplicación de compuertas de decisión facilita representar la lógica del proceso, incluyendo tanto los flujos principales como los alternativos o excepcionales.

## Importancia del modelo de amenazas STRIDE

El modelo de amenazas STRIDE constituye una guía práctica para fortalecer la seguridad del software a lo largo de todo su ciclo de vida, mejorando la trazabilidad y la protección de la información sensible. Este enfoque permite analizar sistemáticamente seis categorías de amenazas: suplantación de identidad, manipulación de datos, repudio, divulgación de información, denegación de servicio y elevación de privilegios, ayudando a anticipar posibles riesgos antes de que el sistema llegue a producción. Su integración en prácticas modernas como DevSecOps y procesos CI/CD facilita la detección temprana de vulnerabilidades en el código, los pipelines, las dependencias y las configuraciones, contribuyendo a reducir incidentes de seguridad y costos asociados a correcciones tardías.

## Comparación entre TOGAF y C4

| Aspecto | TOGAF | C4 Model |
|----------|--------|-----------|
| Propósito | Marco de arquitectura empresarial para planificar, diseñar y gobernar sistemas organizacionales completos. | Modelo visual para describir y comunicar la arquitectura de software de forma clara. |
| Enfoque | Estratégico y organizacional (nivel empresa). | Técnico y de desarrollo (nivel software). |
| Alcance | Arquitectura empresarial completa: negocio, datos, aplicaciones y tecnología. | Arquitectura de software y sistemas informáticos. |
| Nivel de detalle | Alto nivel metodológico y de gobernanza. | Diferentes niveles visuales progresivos (Contexto, Contenedores, Componentes y Código). |
| Público objetivo | Arquitectos empresariales, gerentes TI y líderes estratégicos. | Desarrolladores, arquitectos de software y equipos técnicos. |
| Metodología | Incluye el ciclo ADM (Architecture Development Method). | No es metodología; es una técnica de documentación visual. |
| Complejidad | Alta, requiere formación y adopción organizacional. | Baja a media, fácil de aprender y aplicar. |
| Uso principal | Definir cómo la tecnología soporta los objetivos del negocio. | Explicar cómo está construido un sistema de software. |
| Tipo de diagramas | Arquitectura empresarial y modelos de gobernanza. | Diagramas estructurados en 4 niveles (C1–C4). |




## 📚 Referencias

- The Open Group. (s.f.). *TOGAF® Standard – Enterprise Architecture Framework*.  
  https://www.opengroup.org/togaf

- C4 Model. (s.f.). *The C4 model for visualising software architecture*.  
  https://c4model.com/

- QflowBPM. (s.f.). *BPMN: Mejores prácticas para modelar procesos*.  
  https://qflowbpm.com/es/bpmn-mejores-practicas-2/

- Xygeni. (s.f.). *STRIDE Threat Model: The “What Can Go Wrong?” Framework*.  
  https://xygeni.io/es/blog/stride-threat-model-the-what-can-go-wrong-framework/


---

_Este documento hace parte de la entrega del taller 1 del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
