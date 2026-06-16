# Paraflection (Parallel Reflection Engine)

> "Step through the looking glass of your own chronology."

Paraflection is an advanced, text-first predictive causal engine designed to simulate and visualize the long-term, multi-step "butterfly effects" of singular, life-defining events. By entering a profile and a specific life catalyst, Paraflection maps out highly detailed, mathematically structured, and emotionally resonant parallel timelines of major future milestones.

---

## 👁️ The Vision

In an era defined by rapid disruption, humanity needs tools that convert existential uncertainty into structured, visual foresight. Paraflection moves away from static linear planning and classical conversational AI, introducing an interactive causal map of human destiny. It represents a paradigm shift from a passive chat assistant to an active narrative simulator.

---

## 🗺️ Architectural Roadmap

The evolution of Paraflection is divided into four distinct strategic horizons:


```

PHASE 1                  PHASE 2                  PHASE 3                  PHASE 4
+---------------------+  +---------------------+  +---------------------+  +---------------------+
| Structured API      |  | Interactive Map UI  |  | Multi-Agent Engine  |  | Generative Cinema   |
| (Go/Gin + Schemas)  |  | (SVG Nodes & Trees) |  | (Economic/Social)   |  | (Visual/Audio Reels)|
+----------+----------+  +----------+----------+  +----------+----------+  +----------+----------+
           |                        |                        |                        |
       [ CURRENT ]               [ NEXT ]               [ FUTURE ]               [ HORIZON ]

```

### Phase 1: The Structured Core (Current)
* **Go & Gin-Gonic API:** A highly concurrent, ultra-fast routing layer designed to manage asynchronous pipeline execution.
* **Causal LLM Orchestration:** Interfacing directly with frontier reasoning engines (Gemini 2.5 / Claude) utilizing strict JSON Schemas.
* **Deterministic JSON Output:** Forcing the LLM to act as a structured data generator returning predictable milestones, chronological ages, probabilities, and "butterfly scale" impact factors.

### Phase 2: Interactive Cartography
* **Visual Life-Tree:** A custom SVG/Canvas frontend that renders the timeline as an interactive, branching Git-like graph rather than a flat document.
* **Decision Nodes:** Allowing users to click on any generated milestone, edit the parameters, and trigger a sub-branch projection from that specific point in time.

### Phase 3: The Multi-Agent Council
* **Domain-Specific Agents:** Splitting the causal projection among multiple specialized sub-agents:
  * **The Economist Agent:** Analyzes job market trends, inflation, and career path viability.
  * **The Sociological Agent:** Projects relationship developments, community shifts, and family dynamics.
  * **The Chaos Agent:** Introduces calculated "Black Swan" events based on a user-defined entropy slider.
* **Consensus Modeling:** Merging agent outputs into a unified, logically airtight biography.

### Phase 4: Generative Cinematic Synthesis
* **Scene Promoters:** Using the `visual_prompt` metadata generated in Phase 1 to call low-latency text-to-image and text-to-video API clusters (e.g., Luma, Fal.ai).
* **Chronological Video Reels:** Stitching together short, mood-consistent video snapshots for each major life milestone into a cohesive, shareable "Life Trailer."

---

## 🛠️ Getting Started (Local Alpha)

The Paraflection backend is built with Go and Gin Gonic. It includes a built-in simulation engine that generates high-fidelity mock paths even if you do not have an active LLM API key configured.

### Prerequisites
* Go (version 1.20 or higher)

### Setup & Run
1. **Clone the repository:**
```bash
   git clone [https://github.com/yourusername/paraflection.git](https://github.com/yourusername/paraflection.git)
   cd paraflection
```

2. **Run the server:**

```bash
   go run main.go
```

3. **(Optional) Provide your API key to run actual AI projections:**

```bash
   export GEMINI_API_KEY="your-gemini-api-key-here"
   go run main.go
```

---

## 📡 API Reference

### Project Timeline

`POST /api/v1/project`

#### Request Payload

```json
{
  "age": 28,
  "occupation": "Graphic Designer",
  "seed_event": "Laid off due to AI image generation automation tools.",
  "narrative_style": "chaotic"
}

```

#### Response Structure (200 OK)

```json
{
  "input_event": "Laid off due to AI image generation automation tools.",
  "timeline": [
    {
      "age": 29,
      "title": "The Deep Pivot",
      "description": "Faced with automation, you spend 12 months learning physical design fabrication and custom 3D printing. You pivot from digital screens to tangible objects, feeling a mix of deep exhaustion and creative rebirth.",
      "visual_prompt": "A warm, dusty workshop at night. An individual wearing safety glasses watches a high-end 3D printer head deposit glowing orange filament, cinematic lighting, shallow depth of field.",
      "probability": 0.88,
      "butterfly_scale": 6
    }
  ]
}

```

---

## ⚖️ Strategic Trade-offs

* **Logic vs. Gimmickry:** Prioritize rigorous causal logic. If a user loses a job, the engine must calculate realistic struggles and gradual adaptations before projecting grand successes.
* **Privacy-First:** Future iterations will support local edge-inference models to ensure that deeply personal life reflections never leave the user's local hardware.
* **Dynamic Chaos:** Users can scale the predictability of their timelines from "Highly Realistic/Statistical" to "Extreme Butterfly Effect," adjusting how much randomness dictates their parallel reflections.
