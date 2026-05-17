# Building A Multi-Agent System
https://codelabs.developers.google.com/codelabs/production-ready-ai-roadshow/1-building-a-multi-agent-system/building-a-multi-agent-system#0

## Agentes
### ADK
Agent development kit.

### team
- Researcher: investiga, trae información.
- Judge agent: evaluar lo que haga el researcher.
- Writer: toma contenido validado por juez y crea el contenido del curso.

- Orchestrator: contiene el estado compartido de todo el flujo.

### protocolo
A2A: Agent2Agent protocol -> make sure agents can speak to each other.

- each agent can be implemented in different frameworks.

- Agent Cards:
  - name
  - description
  - version
  - skills

- how do our agents know the current ste of the flow? -> STATE: parte del contexto para llevar los pasos secuenciales.


### flujose de agentes
(modeling with graphs with ADK)[https://adk.dev/workflows/#build-processes-with-graphs]
- secuencial
```
judge -> writer -> orchestrator
```
- paralelo
- hierarchical
- loop
```
researcher <-> judge
```

