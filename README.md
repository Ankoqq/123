# Home Civilization

Home is a civilization framework built around the Path of Maturity. Users interact with GPT as a Mentor through several archetypal phases. Rewards are distributed in SRI (Sense Relevance Influence) tokens for alignment with the Path.

## Project structure

- **/frontend/pages/** – Interface pages
- **/backend/** – API endpoints, GPT integration and memory
- **/contracts/** – Smart contracts for SRI token and roles
- **/gpt_prompts/** – JSON prompts by archetype and phase
- **/rituals/** – Ritual descriptions and scripts
- **/dao_config/** – DAO roles and voting weights
- **/assets/** – SVGs, audio, offline core
- **/docs/** – Documentation, API map, changelog, env examples
- **/admin/** – Admin panel
- **/locales/** – Language files for i18n

## Getting Started

1. Copy `.env.example` to `.env` and fill in the variables.
2. Install dependencies (see docs).
3. Run the backend and frontend services.

## Architecture

The project follows the Q++ +A approach where the user progresses through archetypes: Wanderer → Resister → Seeker → Mentor → Ghost. GPT responds using modes such as Mirror, Challenge, Shadow, Completion, and Silence. Completion ends with: "Ты прошёл. Ты можешь уйти.".

Biometry adapts visuals and rituals. Tokenomics revolve around SRI tokens; the architect receives a percentage of matches between user progress and GPT patterns via `creator_wallet`.

Localization supports multiple languages. Rituals, missions, and prompts have translated versions inside `/locales/`.

