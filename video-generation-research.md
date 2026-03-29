# Investigacion: Generacion de Videos con IA

> Fecha: 2026-03-29
> Objetivo: Evaluar herramientas de IA para generar videos animados (cuentos infantiles artisticos) y videos pedagogicos (explicacion de procesos y tramites).

---

## Resumen Ejecutivo

El ecosistema de generacion de video con IA ha madurado significativamente. La recomendacion principal es usar un enfoque **multi-herramienta** segun el caso de uso:

| Caso de Uso | Herramienta Recomendada | Alternativa |
|---|---|---|
| **Cuentos infantiles animados** | AnimateAI + Neolemon | Mootion, MagicLight AI |
| **Videos pedagogicos con avatar** | HeyGen / Synthesia | Colossyan |
| **Videos explicativos animados** | Runway Gen-4 + ElevenLabs | Veo 3.1 |
| **Estilos artisticos variados (anime, ilustracion)** | MiniMax Hailuo 2.3/2.5 | Kling 3.0 |
| **Alto volumen / bajo costo** | Kling 2.6 / 3.0 | MiniMax Hailuo (Unlimited) |
| **Integracion con Claude (MCP)** | MiniMax MCP (oficial) | Kling MCP, Video Agent MCP |

---

## Parte 1: Cuentos Infantiles Animados

### Desafio Principal: Consistencia de Personajes

El mayor reto en la generacion de cuentos animados es el **character drift** (los personajes cambian de apariencia entre escenas). Las herramientas especializadas resuelven esto con "character locking".

### Herramientas Especializadas para Cuentos Infantiles

#### 1. AnimateAI (animateai.pro)
- **Que es**: Plataforma todo-en-uno que integra multiples IAs (GPT-4, Claude, Gemini para texto; FLUX y MidJourney para imagenes; ElevenLabs para voces; Suno para musica; Runway/Kling/Minimax para video).
- **Fortaleza clave**: Permite disenar y personalizar personajes unicos con estilos, vestuario y voces, y guardarlos para reutilizacion instantanea. Esto garantiza **consistencia entre episodios**.
- **Ideal para**: Series de cuentos con personajes recurrentes.

#### 2. Neolemon (neolemon.com)
- **Que es**: Plataforma especializada en storytelling animado con IA.
- **Fortaleza clave**: Resuelve el problema de consistencia de personajes "bloqueando" la identidad visual del personaje en cada imagen generada. Soporta estilos cartoon, anime y 3D tipo Pixar.
- **Precio**: Desde $29/mes con prueba gratuita de ~20 creditos.
- **Ideal para**: Autores de libros infantiles que quieran convertir manuscritos en videos animados.

#### 3. Mootion (mootion.com)
- **Que es**: Creador de videos de cuentos infantiles con IA.
- **Fortaleza clave**: Supera a competidores en velocidad (video de 3 min en menos de 2 min). Ofrece estilos de animacion suaves, voces narradoras calmadas y efectos visuales relajantes.
- **Ideal para**: Videos de cuentos para dormir, contenido para padres y educadores.

#### 4. MagicLight AI (magiclight.ai)
- **Que es**: Generador de videos largos con IA (hasta 50 minutos).
- **Fortaleza clave**: Genera animaciones multi-escena con movimiento natural y **consistencia visual durante todo el video**. Incluye plantillas para cuentos infantiles.
- **Ideal para**: Videos largos de cuentos completos.

#### 5. Krikey AI (krikey.ai)
- **Que es**: Generador de animaciones 3D con IA.
- **Fortaleza clave**: Certificado Clever para uso en aulas. Permite crear avatares 3D personalizados con lip-sync. Plataforma basada en navegador, sin necesidad de codigo.
- **Ideal para**: Contenido educativo infantil en escuelas.

---

## Parte 2: Videos Pedagogicos y Explicativos

### Para explicar procesos de documentacion y tramites

#### 1. HeyGen (heygen.com) - RECOMENDADO
- **Que es**: Plataforma de creacion de video con avatares IA ultra-realistas.
- **Fortaleza clave**: Avatar IV es el sistema mas fotorrealista disponible comercialmente (2026). Puede crear videos explicativos desde documentos, URLs o scripts.
- **Caracteristicas**:
  - 175+ idiomas y dialectos (incluido espanol)
  - Clonacion de voz: puedes crear un avatar que luce y suena como tu
  - Calidad 1080p o 4K
  - Convierte ideas complejas en historias visuales claras
- **Ideal para**: Videos de capacitacion, explicacion de tramites, tutoriales de procesos.

#### 2. Synthesia (synthesia.io) - RECOMENDADO para empresas
- **Que es**: Plataforma #1 de video IA para empresas (usada por la mayoria del Fortune 100).
- **Fortaleza clave**: Orientada a capacitacion empresarial, onboarding y L&D. Sistema de diapositivas ideal para explicaciones paso a paso.
- **Caracteristicas**:
  - 120+ idiomas
  - Reportan "100 horas de traduccion en 10 minutos"
  - Exportacion SCORM para LMS
  - Seguridad empresarial (SOC 2, ISO 42001)
  - Herramientas de colaboracion y brand kit
- **Ideal para**: Grandes organizaciones con contenido repetible y estructurado.

#### 3. Colossyan (colossyan.com)
- **Que es**: Plataforma de video IA enfocada en capacitacion laboral.
- **Fortaleza clave**: Funcion **Doc2Video** que convierte documentos estaticos en cursos de video, con marcadores de animacion y quizzes interactivos.
- **Ideal para**: Convertir SOPs, manuales PDF y documentacion de procesos en videos interactivos.

#### 4. X-Pilot (x-pilot.ai)
- **Que es**: Generador gratuito de videos explicativos con IA.
- **Fortaleza clave**: Organiza escenas en orden pedagogico siguiendo frameworks probados (Problema -> Solucion -> Como Funciona). Convierte manuales PDF en animaciones de procesos.
- **Ideal para**: Explicaciones de tramites y procesos burocraticos de forma simple.

---

## Parte 3: APIs y Modelos de Video Generativo (nivel tecnico)

### Modelos Principales en 2026

#### Runway Gen-4 / Gen-4.5
- **Mejor para**: Calidad profesional y control creativo
- **Fortaleza**: Mejor consistencia temporal y control de movimiento. Ecosistema de edicion (masking, motion brushes, compositing, inpainting)
- **Precio**: Desde ~$15/mes
- **API**: Disponible

#### Google Veo 3 / Veo 3.1
- **Mejor para**: Alta resolucion con audio nativo
- **Fortaleza**: Genera a 1080p y upscalea a 4K con IA (no es 4K nativo puro). Integra con Google Drive, YouTube Studio, Google Ads via Gemini API
- **Limitaciones**: Clips max 8 seg, 4K solo en preview/Ultra ($249.99/mes), upscaling no lossless
- **Precio**: $0.15/seg (Fast) - $0.40/seg (Standard). 4K solo en tier Ultra
- **API**: Via Gemini API / Vertex AI

#### Kling 2.6 / 3.0 (Kuaishou)
- **Mejor para**: Relacion precio-calidad
- **Fortaleza**: Calidad equivalente a ~40% del costo. Kling 3.0 introduce secuencias multi-toma con consistencia de sujeto entre angulos de camara
- **Precio**: $0.07-$0.10/segundo
- **API**: Disponible

#### MiniMax / Hailuo AI (Destacado)
- **Mejor para**: Fisica realista, estilos artisticos variados y relacion costo-rendimiento
- **Modelo actual**: Hailuo 2.3 (oct 2025) / Hailuo 2.5 (2026) con motor de fisica avanzado
- **Arquitectura**: MiniMax-M1 con 456 mil millones de parametros y ventana de contexto de 1M tokens
- **Resolucion**: 768p y 1080p (1080p limitado a 6 seg)
- **Benchmarks**: #2 global en Artificial Analysis, supera a Google Veo 3 en varias metricas de calidad
- **Puntuacion**: 8.5/10 en reviews independientes
- **Fortalezas**:
  - **Motor de fisica excepcional**: Simulacion de fluidos, deteccion de colisiones, iluminacion global con ray-tracing (v2.5)
  - **Estilos artisticos amplios**: Anime, ilustracion, pintura china con tinta, CG de videojuegos - ideal para cuentos infantiles artisticos
  - **Micro-expresiones mejoradas**: Expresiones faciales realistas y matices emocionales
  - **Control de camara**: Interpreta instrucciones complejas ("paneo a la derecha", "zoom dinamico", "saltar y girar")
  - **Variante Fast**: 50% mas barato manteniendo buena fidelidad
- **Precios**:
  - Gratis: Videos de 6 seg en 1080p con marca de agua
  - Standard: $9.99/mes (1,000 creditos, ~40 videos) = ~$0.25/clip
  - Unlimited: $94.99/mes (creditos ilimitados) = ~$0.15-0.20/video
  - API: $0.10/M tokens via plataforma MiniMax; tambien en fal.ai, Replicate, Segmind, WaveSpeedAI
- **Debilidades**:
  - Creditos "usar o perder" (no se acumulan)
  - Clips cortos (6-10 seg max)
  - Menos tutoriales y comunidad en Occidente vs Runway/Kling

##### Hailuo Video Agent (Nuevo - en Beta)
- **Que es**: Agente autonomo que genera videos completos de principio a fin usando lenguaje natural
- **Innovacion**: Rompe con workflows de nodos rigidos. Un LLM invoca herramientas automaticamente en cada etapa (ideacion, storyboard, assets, edicion, voiceover)
- **Fases de lanzamiento**:
  1. Plantillas pre-construidas (un click)
  2. Semi-personalizable (editar cualquier parte del proceso)
  3. Agente totalmente autonomo (end-to-end)
- **Transparencia**: Muestra el proceso de pensamiento paso a paso del agente en tiempo real
- **Potencial para cuentos infantiles**: Alto - permite generar videos completos describiendo la historia en lenguaje natural

##### MiniMax MCP Server Oficial (integracion con Claude)
- **Repo**: [MiniMax-AI/MiniMax-MCP](https://github.com/MiniMax-AI/MiniMax-MCP)
- **Capacidades**: Text-to-Speech, clonacion de voz, generacion de imagen y video
- **Setup en Claude Desktop**:
```json
{
  "mcpServers": {
    "MiniMax": {
      "command": "uvx",
      "args": ["minimax-mcp"],
      "env": {
        "MINIMAX_API_KEY": "tu-api-key-aqui",
        "MINIMAX_MCP_BASE_PATH": "/ruta/local",
        "MINIMAX_API_HOST": "https://api.minimax.io",
        "MINIMAX_API_RESOURCE_MODE": "url"
      }
    }
  }
}
```
- **Requisitos**: API key de MiniMax + `uv` (gestor de paquetes Python)

#### Sora 2 (OpenAI) - Solo via ChatGPT
- **Nota**: La app y API standalone de Sora se cerraron el 24 de marzo 2026
- **Acceso**: Solo a traves de ChatGPT Plus ($20/mes) o Pro ($200/mes)
- **Fortaleza**: Calidad cinematografica, excelente adherencia al prompt

### Tendencias Clave 2026
1. **Audio nativo**: Sora 2, Veo 3.1 y Kling 2.6 generan efectos de sonido y dialogo sincronizado
2. **Resolucion 4K nativa** y videos de 20+ segundos
3. **Gateways API unificados**: Plataformas como **fal.ai** ofrecen acceso a multiples modelos desde un solo endpoint

---

## Parte 4: Integracion con Claude via MCP

Existen servidores MCP que permiten generar video directamente desde Claude:

### MCP Servers Disponibles

| Servidor MCP | Modelos Soportados | Funcionalidades |
|---|---|---|
| **Kling MCP** (199-mcp/mcp-kling) | Kling v1.0-v1.6, KOLORS | 13+ herramientas: video, imagen, efectos, lip-sync |
| **Video Agent MCP** (h2a-dev) | Kling 2.1, Hailuo 02 | Crear proyectos, agregar escenas, generar musica |
| **FAL.ai MCP** | Luma Ray2 Flash, Kling v1.6 Pro | Video desde texto, control de parametros |
| **Pictory MCP** | Pictory engine | Pipeline completo de video desde Claude |
| **MiniMax MCP** | MiniMax-Hailuo-02 | Video 6s/10s, 768P/1080P, diseno de voz |
| **Veo2 MCP** | Google Veo 2 | Generacion de video como agente autonomo |
| **Scenario MCP** | 344+ modelos | Imagen, video, 3D y audio |

### Recomendacion de MCP para Claude
- **Para cuentos infantiles**: Kling MCP (consistencia de personajes + bajo costo) o Video Agent MCP (flujo multi-escena)
- **Para videos explicativos**: Pictory MCP (pipeline completo) o Scenario MCP (variedad de modelos)

---

## Parte 5: Recomendaciones Finales

### Para Cuentos Infantiles Artisticos

**Opcion A - Todo en uno (mas facil)**:
1. Usar **AnimateAI** o **Mootion** para generar el video completo desde un script
2. Ventaja: Flujo simple, personajes consistentes
3. Costo: Variable segun plataforma

**Opcion B - Pipeline personalizado (mejor calidad)**:
1. Escribir guion con Claude
2. Generar imagenes consistentes con **Neolemon** (character locking)
3. Animar con **Runway Gen-4** o **Kling 3.0** (image-to-video)
4. Agregar voz con **ElevenLabs**
5. Agregar musica con **Suno**
6. Editar y ensamblar final

### Para Videos Pedagogicos de Tramites/Procesos

**Opcion A - Avatar presentador (recomendada para tramites)**:
1. Usar **HeyGen** o **Synthesia**
2. Escribir guion paso a paso del proceso/tramite
3. La IA genera un video con avatar que explica cada paso
4. Ventaja: Profesional, multi-idioma, facil de actualizar

**Opcion B - Video animado explicativo**:
1. Usar **Colossyan** Doc2Video o **X-Pilot**
2. Subir documentacion del proceso (PDF, doc)
3. La IA convierte automaticamente en video con animaciones
4. Ventaja: Directo desde documentacion existente

**Opcion C - Integracion con Claude (para desarrolladores)**:
1. Configurar **Kling MCP Server** o **Pictory MCP** en Claude
2. Describir el proceso en lenguaje natural
3. Claude genera el video directamente
4. Ventaja: Automatizable, integrable en flujos de trabajo

---

## Parte 6: Guia de Compra - Modelos Chinos (MiniMax y Kling)

Los modelos chinos (MiniMax/Hailuo y Kling) tienen **3 formas de comprar**, cada una para un perfil diferente:

### Forma 1: Suscripcion Web (La mas facil - para creadores individuales)

Pagas mensual, recibes creditos, usas la interfaz web. Como Netflix pero para generar videos.

**MiniMax / Hailuo:**
| Plan | Precio/mes | Creditos | Videos aprox. | Costo por video |
|---|---|---|---|---|
| Gratis | $0 | Limitados | ~5-10/dia con marca de agua | $0 |
| Standard | $9.99 | 1,000 | ~40 videos (6seg/1080p) | ~$0.25 |
| Unlimited | $94.99 | Ilimitados | Sin limite | ~$0.15-0.20 |

**Kling AI:**
| Plan | Precio/mes | Creditos | Videos aprox. | Costo por video |
|---|---|---|---|---|
| Gratis | $0 | 66/dia | ~6 videos/dia (5seg) con marca de agua | $0 |
| Standard | $10 | 660/mes | ~66 videos (modo estandar) | ~$0.15 |
| Pro | $37 | 3,000/mes | ~150 videos (720p/1080p) | ~$0.25 |
| Premier | $92 | 8,000/mes | ~400 videos (1080p) | ~$0.23 |
| Ultra | $180 | 26,000/mes | ~1,300 videos | ~$0.14 |

> **OJO con creditos**: En MiniMax los creditos NO se acumulan (los pierdes al final del mes). En Kling los creditos de planes pagados duran 2 anos. Puedes comprar creditos extra en Kling desde $5 (330 creditos, validos 2 anos).

> **OJO con generaciones fallidas**: En Kling, si el video falla igual te cobran los creditos. En MiniMax no.

> **Descuento anual**: Kling ofrece ~34% descuento pagando anual.

**Cuando elegir suscripcion web:**
- Eres creador individual o equipo pequeno
- Usas la interfaz visual (no necesitas programar)
- Generas menos de ~100 videos/mes
- Quieres empezar rapido sin configuracion tecnica

---

### Forma 2: API Directa (Para desarrolladores y automatizacion)

Pagas por uso (tokens o unidades). Necesitas programar o usar herramientas como MCP.

**MiniMax API Directa:**
| Concepto | Precio |
|---|---|
| Video Hailuo-02 (512p, 10seg) | 0.5 unidades por video |
| Texto M2.5 | $0.10-0.20 por millon de tokens |
| TTS (voz) | Variable por uso |

**MiniMax Token Plan (NUEVO - marzo 2026):**
- Suscripcion unificada que da acceso a TODOS los modelos (texto, video, voz, musica, imagen) con una sola API key
- Starter $10/mes: 1,500 req M2.7 (solo texto)
- Plus $20/mes: 4,500 req M2.7 + 50 imagenes/dia + 4,000 chars TTS/dia + resource packs de video
- Las cuotas de video/imagen/voz son INDEPENDIENTES del texto (no se consumen entre si)
- ~20% descuento vs pay-as-you-go en modelos premium (Hailuo 2.3, Speech 2.8)
- Ideal si usas MiniMax para multiples tareas (PDF a MD, imagenes, video, voz)

**Kling API Directa (Enterprise):**
| Concepto | Precio |
|---|---|
| Paquete minimo | ~$4,200 (30,000 unidades, 90 dias) |
| Precio por unidad | $0.14 |
| 1 unidad = | 1 video de 5 seg (modo estandar) |

> **IMPORTANTE**: La API oficial de Kling es solo enterprise ($4,200 minimo). No es accesible para proyectos pequenos. La de MiniMax si es accesible individualmente.

**Cuando elegir API directa:**
- Necesitas automatizar la generacion (app, bot, flujo de trabajo)
- Quieres integrar con Claude via MCP
- Para MiniMax: cualquier volumen funciona
- Para Kling: solo si generas a gran escala (enterprise)

---

### Forma 3: API via Terceros (La mejor opcion para desarrolladores)

Plataformas intermediarias dan acceso a MULTIPLES modelos con una sola cuenta y API key. Es como un "supermercado de APIs de video".

**fal.ai (RECOMENDADO para desarrolladores):**
| Modelo | Precio por clip | Notas |
|---|---|---|
| Hailuo 2.3 (MiniMax) 1080p | ~$0.28-0.49/video | 6 seg |
| Kling 3.0 Pro (sin audio) | $0.112/seg (~$0.56/5seg) | |
| Kling 3.0 Pro (con audio+voz) | $0.196/seg (~$0.98/5seg) | |
| PixVerse v5.5 720p | $0.20/video | 5 seg |
| Luma Ray2 | ~$0.50/video | |

**Otras plataformas terceras:**
| Plataforma | Ventaja | Modelos disponibles |
|---|---|---|
| **fal.ai** | Mas barato, arranque en frio 5-10seg | MiniMax, Kling, Luma, PixVerse, LTX |
| **Replicate** | Mejor documentacion | MiniMax Hailuo 2.3, Wan, LTX |
| **Segmind** | Pay-as-you-go sin compromisos | MiniMax, Kling |
| **PiAPI** | Kling a $0.13/video | Kling (mas barato que oficial) |
| **WaveSpeedAI** | Alternativa a Hailuo | MiniMax, otros |
| **ModelsLab** | 400+ modelos en una API | Todo |

**Cuando elegir terceros:**
- Quieres probar multiples modelos sin crear cuentas en cada uno
- No quieres pagar $4,200 por la API de Kling
- Quieres pagar solo por lo que usas (sin suscripcion)
- Necesitas una sola API key para todo

---

### Resumen: Cual forma elegir segun tu perfil

| Tu perfil | Forma recomendada | Servicio sugerido |
|---|---|---|
| **Creador individual, pocos videos** | Suscripcion web | MiniMax Standard ($9.99) o Kling Standard ($10) |
| **Creador de volumen** | Suscripcion web | MiniMax Unlimited ($94.99) o Kling Premier ($92) |
| **Desarrollador, quiere automatizar** | API via terceros | fal.ai (pay-as-you-go) |
| **Desarrollador, usa Claude/MCP** | API directa MiniMax | MiniMax Token Plan + MCP Server |
| **Empresa/alto volumen** | API directa | Kling Enterprise ($4,200+) o MiniMax Token Plan |
| **Solo quiere probar** | Gratis | MiniMax gratis o Kling gratis (66 cred/dia) |

---

## Parte 6b: Precios de API - Todas las plataformas (Referencia Rapida)

| Herramienta | API Self-Serve | Modelo de Precio | Costo Minimo |
|---|---|---|---|
| Google Veo 3.1 | Si (Gemini API) | Por segundo | $0.15/seg (Fast) - $0.60/seg (4K+audio) |
| Runway Gen-4 | Si (REST API) | Por credito | ~$0.05/seg (Turbo) |
| Kling AI | Solo Enterprise | Por paquete | ~$4,200 min (30K unidades) |
| Kling AI (Web) | N/A | Suscripcion | $6.99-$25.99/mes |
| Pika 2.2 | Via fal.ai | Por generacion | ~$0.45/clip |
| Luma Ray3 | Si | Por tarea | $0.20/tarea |
| MiniMax/Hailuo | Si | Por token | $0.10/M tokens |
| Synthesia | Plan Creator+ | Por minuto | $89/mes |
| HeyGen | Si (pay-as-you-go) | Por credito (1=1min) | Desde $5, $0.50-$0.99/min |
| D-ID | Si | Por credito | $18/mes (Build) |
| Seedance | Si | Por segundo | $0.0247/seg (mas barato) |

> **NOTA**: Sora cerro su app y API standalone el 24 de marzo 2026. No construir sobre Sora.

---

## Parte 7: Alternativas Open Source (Auto-hospedadas)

Para equipos con recursos de GPU propios:

| Modelo | Licencia | VRAM Minima | Fortaleza |
|---|---|---|---|
| **Wan 2.2/2.6** (Alibaba) | Apache 2.0 (gratis) | 8 GB | Mejor calidad open-source, control de camara cinematografico |
| **LTX-Video 2.3** (Lightricks) | Gratis <$10M rev | 12 GB (48 recomendado) | 18x mas rapido que Wan, hasta 4K a 50 FPS |
| **Seedance 2.0** (ByteDance) | Open weights | Variable | Rating Elo mas alto (1,269), fine-tunable |
| **Stable Video Diffusion** (Stability) | Community License | 8 GB | Enorme comunidad ComfyUI |

### Workflow con ElevenLabs Flows
ElevenLabs ofrece un canvas basado en nodos que encadena Veo, Kling, Wan y Seedance con voces, musica y efectos de sonido en un solo flujo visual.

---

## Parte 8: Consistencia de Personajes - El Problema Clave

El **character drift** es el mayor desafio. Solucion por capas:

1. **Crear "biblia de personaje"** con especificaciones visuales detalladas
2. **Generar imagenes de referencia** desde multiples angulos
3. **Usar herramientas de character locking**: Neolemon, LTX Studio (sistema Elements con @tagging)
4. **Encadenar fotogramas**: Ultimo frame del clip N = referencia para clip N+1
5. **Clips cortos (3-4 seg)** para minimizar drift
6. **Avanzado**: Fine-tuning LoRA con 20-30 imagenes del personaje (mas consistente pero requiere GPU)

---

## Fuentes

- [Best Video Generation AI Models 2026 - Pinggy](https://pinggy.io/blog/best_video_generation_ai_models/)
- [After Sora: Best AI Video Generators 2026](https://www.digitalapplied.com/blog/after-sora-best-ai-video-generators-2026-runway-kling-veo)
- [7 Best AI Video Generation API Alternatives After Sora](https://help.apiyi.com/en/sora-shutdown-7-best-ai-video-generation-api-alternatives-guide-en.html)
- [Best AI Video Model 2026 Comparison Guide](https://blog.laozhang.ai/en/posts/best-ai-video-model)
- [10 Best AI Video Generators 2026 - fal.ai](https://fal.ai/learn/tools/ai-video-generators)
- [15 AI Video Models Tested - TeamDay.ai](https://www.teamday.ai/blog/best-ai-video-models-2026)
- [Kling vs Sora vs Veo vs Runway Comparison](https://invideo.io/blog/kling-vs-sora-vs-veo-vs-runway/)
- [7 Best AI Tools for Animated Storytelling 2026](https://www.neolemon.com/blog/best-ai-tools-for-animated-storytelling/)
- [AnimateAI](https://animateai.pro/)
- [Mootion - AI Children's Story Video Maker](https://www.mootion.com/use-cases/en/ai-childrens-story-video-maker)
- [MagicLight AI](https://magiclight.ai/)
- [HeyGen AI Video Explainer](https://www.heygen.com/tool/ai-video-explainer)
- [Synthesia](https://www.synthesia.io/)
- [HeyGen vs Synthesia 2026 - Colossyan](https://www.colossyan.com/posts/heygen-vs-synthesia)
- [AI Explainer Video Tools 2026](https://mypromovideos.com/blog/ai-explainer-videos-examples/)
- [X-Pilot Free Explainer Video Generator](https://www.x-pilot.ai/products/free-explainer-video-generator)
- [Kling MCP Server - GitHub](https://github.com/199-mcp/mcp-kling)
- [Video Agent MCP Server](https://mcpservers.org/servers/h2a-dev/video-gen-mcp-monolithic)
- [FAL.ai MCP Server](https://mcp.so/server/fal-mcp-server/el-el-san)
- [Pictory MCP Server](https://pictory.ai/ai-video-script-generator-8)
- [MiniMax MCP Server](https://mcpservers.org/servers/github-com-minimax-ai-minimax-mcp)
- [Veo2 MCP Server Deep Dive](https://skywork.ai/skypage/en/video-generation-ai-engineer/1981550286026633216)
