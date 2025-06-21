# Hopfield Networks & Associative Memory

## Project Overview
This project explores **Hopfield networks** as **autoassociative memory systems**, analyzing their capabilities for **pattern completion, noise resistance, and energy-based convergence**. The study also investigates storage limitations and the differences between **synchronous (Little model) and asynchronous (sequential) updates**.

## Technologies & Tools Used
- **Programming Language**: Python
- **Libraries**: NumPy, Matplotlib, Google Colab
- **Training Rule**: Hebbian Learning
- **Update Methods**: Synchronous vs. Asynchronous (Random Order)
- **Evaluation Metrics**: Energy Function Analysis, Convergence Rate, Pattern Recall Accuracy

## Key Features

### Pattern Recall & Noise Resistance
- **Tested recall with noisy inputs** and analyzed attractor stability.
- Measured **network robustness** by introducing **1-bit to 5-bit distortions**.
- **Spurious Attractors**: Investigated unexpected network states beyond stored patterns.

### Energy Function Analysis
- Tracked **energy evolution** to validate network convergence.
- Compared energy behavior under **random weight matrices vs. symmetric weight matrices**.

### Storage Capacity & Scaling
- **Tested storage limits** by increasing the number of patterns.
- Observed **degradation in recall accuracy** beyond optimal capacity (~0.138N).
- **Sparse Encoding**: Evaluated how sparsity influences memory efficiency.

## Results
- **Hopfield networks can restore patterns with up to ~30% noise** but fail beyond 50%.  
- **Sequential updates improve convergence stability** but may lead to **pathological attractors**.  
- **Random weight matrices fail to converge**, whereas **symmetric matrices ensure stability**.  
- **Pattern recall accuracy decreases sharply beyond storage capacity limits**.  
- **Sparse encoding improves recall efficiency**, reducing interference between stored patterns.  
