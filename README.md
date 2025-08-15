# Hangman Solver: Hybrid Ensemble of Specialized Experts  

An AI agent that dynamically blends multiple neural experts to solve Hangman with high precision.  

## Overview  
This project implements a **hybrid ensemble of five specialized models** (Transformers and CANINE) to play Hangman optimally at every stage. The system adapts its strategy based on the game's ambiguity, transitioning from statistical heuristics to neural expert voting as letters are revealed.  

## Key Features  
- **Five specialized experts**:  
  - Three custom Transformers (early/mid/late-game).  
  - Two fine-tuned CANINE models (high/low ambiguity).  
- **Dynamic inference engine**: Blends expert predictions using mask-aware weighting.  
- **Fallback mechanisms**: Ensures guesses are always logical (dictionary frequency → English letter frequency).  

