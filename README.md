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
  PHASE 1                  PHASE 2                  PHASE 3                  PHASE 4                  PHASE 5
+---------------------+  +---------------------+  +---------------------+  +---------------------+  +---------------------+
| Structured API      |  | Interactive Map UI  |  | Multi-Agent Engine  |  | Generative Cinema   |  | Proprietary Causal  |
| (Go/Gin + Schemas)  |  | (SVG Nodes & Trees) |  | (Economic/Social)   |  | (Visual/Audio Reels)|  | (Self-Hosted Model) |
+----------+----------+  +----------+----------+  +----------+----------+  +----------+----------+  +----------+----------+
           |                        |                        |                        |                        |
       [ CURRENT ]               [ NEXT ]               [ FUTURE ]               [ HORIZON ]              [ ULTIMATE ]
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

### Phase 5: Proprietary Independence (The Singularity)
* **Custom Open-Weights Fine-Tuning**: Extracting the corpus of thousands of high-fidelity, user-approved historical timelines generated in prior phases.
* **Self-Hosted Inference**: Training and deploying a private fine-tuned LLM (e.g., Llama-3-8B / Qwen-2.5) on secure private GPU cloud infrastructure.
* **Zero Dependency Operations**: Moving entirely away from third-party APIs (OpenAI, Anthropic, Google) to guarantee ultimate user privacy, zero rate limits, and zero external costs.
---

## 🛠️ Getting Started (Local Alpha)

The Paraflection backend is built with Go and Gin Gonic. It includes a built-in simulation engine that generates high-fidelity mock paths even if you do not have an active LLM API key configured.

### Prerequisites
* Go (version 1.20 or higher)

### Setup & Run
1. **Clone the repository:**
```bash
   git clone [https://github.com/XaiPhyr/paraflection.git](https://github.com/XaiPhyr/paraflection.git)
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
  "input_event":"Laid off due to AI image generation automation tools.",
  "starting_age":28,
  "starting_occupation":"Graphic Designer",
  "root":{
    "id":"node_0",
    "age":28,
    "title":"The Severance",
    "description":"The email arrives on a Tuesday morning: 'Your department is being consolidated.' You walk out with 3 months' severance and a portfolio of digital assets that feel suddenly obsolete.",
    "visual_prompt":"An empty desk in a modern open-plan office, sunlight streaming through towering windows casting long shadows across an abandoned mechanical keyboard, cinematic mood.",
    "probability":1.0,
    "butterfly_scale":10,
    "branches":[
      {
        "id":"node_1a",
        "choice_trigger":"Pivot to Physical Craft",
        "age":29,
        "title":"The Deep Pivot",
        "description":"Faced with automation, you spend 12 months learning physical design fabrication and custom 3D printing. You pivot from digital screens to tangible objects, feeling a mix of deep exhaustion and creative rebirth.",
        "visual_prompt":"A warm, dusty workshop at night. An individual wearing safety glasses watches a high-end 3D printer head deposit glowing orange filament, cinematic lighting, shallow depth of field.",
        "probability":0.55,
        "butterfly_scale":6,
        "branches":[
          {
            "id":"node_2a_1",
            "choice_trigger":"Scale Up Production",
            "age":33,
            "title":"The Industrial Atelier",
            "description":"You partner with a local boutique manufacturer to scale your 3D printed physical designs. Your hybrid digital-physical sculptures catch the eye of high-end interior designers.",
            "visual_prompt":"A bright, clean minimalist gallery showroom. Tall concrete walls, spotlights illuminating geometric, smooth printed physical sculptures, elegant crowd talking.",
            "probability":0.40,
            "butterfly_scale":7,
            "branches":[
              {
                "id":"node_3a_1a",
                "choice_trigger":"SaaS Platform Acquisition",
                "age":42,
                "title":"The Legacy Acquisition",
                "description":"A major home decor conglomerate acquires your design workshop. You step down from active management to consult, securing lifetime wealth while leaving your physical workshop behind.",
                "visual_prompt":"An older designer standing next to a wall of press clippings, shaking hands with executives in a sun-drenched architectural office, warm golden hour tones.",
                "probability":0.35,
                "butterfly_scale":8,
                "branches":[
                  
                ]
              },
              {
                "id":"node_3a_1b",
                "choice_trigger":"Weather a Market Saturation",
                "age":40,
                "title":"The Supply Chain Squeeze",
                "description":"As industrial printing becomes commoditized, you struggle to maintain premium margins. You downsize operations to stay afloat, returning to direct hands-on assembly.",
                "visual_prompt":"A crowded warehouse workspace, pallets of packaged inventory stacked high, a single worker under a fluorescent light looking tired while inspecting a catalog.",
                "probability":0.65,
                "butterfly_scale":5,
                "branches":[
                  
                ]
              }
            ]
          },
          {
            "id":"node_2a_2",
            "choice_trigger":"Keep Craft Small & Bespoke",
            "age":33,
            "title":"The Slow Craft Sanctuary",
            "description":"Rejecting mass production, you establish a small, quiet studio workshop in the countryside. You produce only ten custom pieces a year, finding peace in manual labor and localized clients.",
            "visual_prompt":"A rustic log-cabin style studio surrounded by tall trees in autumn. Warm light spilling from windows, wooden shelves packed with raw clay and intricate printed molds.",
            "probability":0.60,
            "butterfly_scale":4,
            "branches":[
              {
                "id":"node_3a_2a",
                "choice_trigger":"Teach the Next Generation",
                "age":45,
                "title":"The Master Craftsman",
                "description":"You establish a seasonal apprenticeship program. Young digital artists, burnt out by hyper-virtual interfaces, travel to your cabin to learn the art of tangible fabrication.",
                "visual_prompt":"A sunlit wooden patio workshop, an older mentor guiding a young apprentice who is filing down a 3D physical mock, dust motes dancing in the air, nostalgic atmosphere.",
                "probability":0.85,
                "butterfly_scale":5,
                "branches":[
                  
                ]
              },
              {
                "id":"node_3a_2b",
                "choice_trigger":"Existential Solitude",
                "age":45,
                "title":"The Hermit's Gallery",
                "description":"You cut off almost all commercial contacts, choosing to create artwork purely for your own personal satisfaction, leaving a cryptic and highly valuable collection behind.",
                "visual_prompt":"An older, long-haired artist sitting quietly on a porch holding a carved cup, overlooking misty mountains at dawn, deep serenity.",
                "probability":0.15,
                "butterfly_scale":3,
                "branches":[
                  
                ]
              }
            ]
          }
        ]
      },
      {
        "id":"node_1b",
        "choice_trigger":"Lean Into AI Automation",
        "age":29,
        "title":"The Automation Alchemist",
        "description":"Instead of running from AI, you master it. You study prompt engineering, custom fine-tuning, and automated workflows, offering hyper-efficient creative direction to mid-tier corporations.",
        "visual_prompt":"A sleek dual-monitor setup glowing with nodes, visual pipeline charts, and generated vector patterns. A sharp reflection of a determined designer in the glass.",
        "probability":0.45,
        "butterfly_scale":8,
        "branches":[
          {
            "id":"node_2b_1",
            "choice_trigger":"Launch Automated Creative Agency",
            "age":34,
            "title":"The Algorithmic Director",
            "description":"You launch 'Synapse Design Co.', an agency run by just you and three specialized AI agent stacks. You do the creative output of a traditional 50-person agency, achieving extreme profitability.",
            "visual_prompt":"An executive office in a towering skyscraper at golden hour. A single glass desk with a slim laptop, the digital dashboard showing skyrocketing revenue lines.",
            "probability":0.30,
            "butterfly_scale":9,
            "branches":[
              {
                "id":"node_3b_1a",
                "choice_trigger":"Retire Early & Pivot to Philosophy",
                "age":40,
                "title":"The Post-Work Thinker",
                "description":"With your agency running completely on autopilot, you exit daily operations. You spend your time writing books and giving lectures on how automation can liberate, rather than enslave, the human workforce.",
                "visual_prompt":"A massive wood-paneled library. A comfortable leather armchair by a fireplace, a cup of tea resting next to a half-written manuscript on an antique desk.",
                "probability":0.75,
                "butterfly_scale":9,
                "branches":[
                  
                ]
              },
              {
                "id":"node_3b_1b",
                "choice_trigger":"A Corporate Tech Buyout",
                "age":42,
                "title":"The Golden Cage",
                "description":"A tech giant buys your automated systems, but traps you in a restrictive 5-year golden handcuff contract. You make massive money, but your creative soul feels completely drained.",
                "visual_prompt":"A modern, cold blue-lit sterile hallway, a person in an executive suit looking out a massive window overlooking a rain-slicked neon metropolis.",
                "probability":0.25,
                "butterfly_scale":7,
                "branches":[
                  
                ]
              }
            ]
          },
          {
            "id":"node_2b_2",
            "choice_trigger":"Enter Enterprise Leadership",
            "age":34,
            "title":"Chief of Synthetic Creative",
            "description":"A global tech company hires you to spearhead their synthetic assets division. You spend your days managing enterprise prompts, legal guidelines, and human-AI collaborative guardrails.",
            "visual_prompt":"A massive, futuristic boardroom with interactive wall displays showing global brand metrics. A person in a sleek charcoal suit leading a hybrid presentation.",
            "probability":0.70,
            "butterfly_scale":5,
            "branches":[
              {
                "id":"node_3b_2a",
                "choice_trigger":"Ascend to Executive Suite",
                "age":50,
                "title":"The Chief AI Officer",
                "description":"You climb the ladder to become CAIO. You sit at the helm of strategic technology, steering the company through structural post-human labor transformations.",
                "visual_prompt":"A high-end modern glass-walled board room, an older executive commanding attention at the head of a massive conference table, futuristic minimalist design.",
                "probability":0.80,
                "butterfly_scale":8,
                "branches":[
                  
                ]
              },
              {
                "id":"node_3b_2b",
                "choice_trigger":"Resign in Protest",
                "age":48,
                "title":"The Ethical Dissident",
                "description":"Troubled by corporate choices regarding mass synthetic disinformation, you resign. You join an international non-profit group fighting for digital provenance and original human authorship.",
                "visual_prompt":"A press conference setup, microphones crowded on a podium, a serious-looking individual speaking into them under bright media flashing lights.",
                "probability":0.20,
                "butterfly_scale":9,
                "branches":[
                  
                ]
              }
            ]
          }
        ]
      }
    ]
  }
}

```

---

## ⚖️ Strategic Trade-offs

* **Logic vs. Gimmickry:** Prioritize rigorous causal logic. If a user loses a job, the engine must calculate realistic struggles and gradual adaptations before projecting grand successes.
* **Privacy-First:** Future iterations will support local edge-inference models to ensure that deeply personal life reflections never leave the user's local hardware.
* **Dynamic Chaos:** Users can scale the predictability of their timelines from "Highly Realistic/Statistical" to "Extreme Butterfly Effect," adjusting how much randomness dictates their parallel reflections.
