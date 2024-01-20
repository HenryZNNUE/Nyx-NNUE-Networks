# Nyx-NNUE-Networks
This repository stores NNUE networks for Nyx chess engine trained by Grapheus
Nyx NNUE are trained by converted Stockfish master NNUE datasets

Network Name Format: Engine Name-L1-L2-L3(-L4)-Stage Number-Activation Function-Training Dataset-Epochs-Version.nnue

## Architecture 1: 
1024 -> 1024 -> 1
800 to 1000 Epochs
1 Stage

## Architecture 2:
2560 -> 16 -> 32 -> 1

Stage 1: 400 Epochs, Lambda 1.0 means only use evaluation score instead of WDL score to train NNUE, LR 975e-4, gamma 0.995

Stage 2: 800 Epochs, Start Lambda 1.0, End Lambda 0.75, LR 4.375e-4, gamma 0.995

Stage 3: 800 Epochs, Start Lambda 1.0, End Lambda 0.725, LR 4.375e-4, gamma 0.995

Stage 4: 800 Epochs, Start Lambda 1.0, End Lambda 0.7, LR 4.375e-4, gamma 0.995

Stage 5: 800 Epochs, Start Lambda 1.0, End Lambda 0.7, LR 4.375e-4, gamma 0.995


There may be more Networks with different Arch later
