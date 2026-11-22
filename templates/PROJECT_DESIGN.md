# PROJECT_DESIGN.md

## Project name
[Short, clear name]

## 1. Problem and evidence
- Target user: [Who has this problem?]
- Situation: [When does it happen?]
- Current workaround: [What do people do today?]
- Impact: [Time, money, confusion, risk]
- Evidence: [Interviews, observations, screenshots, measurements]
- Assumptions still unverified: [List]

## 2. Goal and success metric
- User outcome: [Observable improvement]
- MVP success metric: [Example: 4/5 testers finish the task]

## 3. MVP scope
### In scope
- [One end-to-end user flow]
- [Only essential features]
### Out of scope
- [Payments, real phone calls, or complex integrations unless essential]

## 4. User journey
1. User [starts with ...]
2. System [shows or asks ...]
3. AI [assists with ...]
4. User [reviews or confirms ...]
5. System [reports the real result or clear failure]

## 5. AI and data design
- Model and why: [Name, version, trade-offs]
- Inputs and data sources: [Where data comes from]
- Data freshness: [Live, cached, or simulated]
- Tools/API calls: [Tool, permission, expected result]
- Voice pipeline (if applicable): [STT -> LLM -> TTS or speech-to-speech]
- Privacy and retention: [What is stored and for how long]

## 6. Architecture
[Frontend] -> [Backend / agent] -> [Model / tools] -> [Result]

## 7. Risks and fallback
- Missing or stale data: [How the app responds]
- Hallucinated answer: [Verification or disclaimer]
- API or voice failure: [Retry / text fallback / human handoff]
- Paid API or external action: [Require user confirmation]

## 8. Acceptance criteria
- [ ] One working happy path
- [ ] User can tell verified from simulated information
- [ ] Failure cases handled clearly
- [ ] Mobile and keyboard use tested
- [ ] Basic cost and latency measured
- [ ] Demo and README explain limitations

## 9. Implementation plan
Day 1: [Research and scope]
Day 2: [Flow and data]
Day 3: [Prototype]
Day 4: [First working path]
Day 5: [Failure testing]
Day 6: [Polish and accessibility]
Day 7: [Publish and document]

## 10. Open questions
- [What needs user research or technical validation?]
