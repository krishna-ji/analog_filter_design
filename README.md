# Analog Filter Design Project

This project contains Jupyter notebooks for designing and analyzing various types of analog filters using Python and SciPy. The notebooks demonstrate different filter types, their frequency responses, and practical applications in signal processing.

## Project Structure

```
analog_filter_design/
├── README.md
├── bode_plot_custom.ipynb          # Custom Bode plot implementation
├── lab2_filter_analysis.ipynb      # Filter analysis with various input signals
├── lab2_filter_degine.ipynb        # Filter design implementations
└── NORMALIZED_template_all_filters.ipynb  # Normalized filter templates
```

## Notebooks Overview

### 1. `bode_plot_custom.ipynb`

- **Purpose**: Demonstrates custom Bode plot generation for Chebyshev Type-I filters
- **Features**:
  - 4th-order Chebyshev Type-I normalized lowpass filter design
  - Manual frequency response calculation
  - Linear scale magnitude and phase plots
  - Custom plotting without using built-in Bode functions

### 2. `lab2_filter_analysis.ipynb`

- **Purpose**: Comprehensive analysis of Butterworth filters with various input signals
- **Signal Types Analyzed**:
  - Square wave filtering
  - Sine wave filtering
  - Triangular wave filtering
  - Random pulse signal filtering
  - Sine wave with noise filtering
  - High-frequency noise filtering
- **Features**:
  - Time-domain analysis
  - Filter response visualization
  - Comparison of input vs. filtered output signals

### 3. `lab2_filter_degine.ipynb`

- **Purpose**: Design and implementation of various filter types
- **Filter Types**:
  - **Low-pass Butterworth Filter** (100 Hz cutoff)
  - **High-pass Chebyshev Filter** (10 Hz cutoff)
  - **Band-pass Butterworth Filter** (200 Hz - 20 kHz passband)
  - **Band-pass Butterworth Filter** (100 Hz - 500 Hz passband)
  - **Elliptic Low-pass Filter** (100 Hz cutoff)
  - **Band-stop Butterworth Filter** (100 Hz - 500 Hz stopband)
- **Features**:
  - Bode plot generation for all filter types
  - Transfer function display
  - Frequency response analysis

### 4. `NORMALIZED_template_all_filters.ipynb`

- **Purpose**: Template for normalized filter designs
- **Filter Types**:
  - Normalized Butterworth Filter
  - Normalized Chebyshev Type-I Filter
  - Normalized Bessel Filter
  - Normalized Elliptic Filter
- **Features**:
  - All filters normalized to 1 rad/s cutoff frequency
  - Comparative analysis of different filter characteristics
  - Template code for easy filter selection

## Key Features

- **Multiple Filter Types**: Butterworth, Chebyshev, Bessel, and Elliptic filters
- **Various Filter Configurations**: Low-pass, high-pass, band-pass, and band-stop
- **Comprehensive Analysis**: Both frequency domain (Bode plots) and time domain analysis
- **Signal Processing Applications**: Real-world signal filtering examples
- **Educational Content**: Well-commented code suitable for learning filter design

## Requirements

```python
numpy
matplotlib
scipy
jupyter
```

## Installation

1. Clone or download the project directory
2. Install required packages:
   ```bash
   pip install numpy matplotlib scipy jupyter
   ```
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Usage

### Getting Started

1. Start with `NORMALIZED_template_all_filters.ipynb` to understand basic filter characteristics
2. Explore `lab2_filter_degine.ipynb` for practical filter design examples
3. Use `lab2_filter_analysis.ipynb` to see how filters behave with different input signals
4. Check `bode_plot_custom.ipynb` for custom plotting techniques

### Filter Design Workflow

1. **Choose Filter Type**: Based on your application requirements (ripple tolerance, transition band, etc.)
2. **Set Specifications**: Define cutoff frequencies, order, and other parameters
3. **Design Filter**: Use appropriate SciPy functions (`buttap`, `cheb1ap`, `ellipap`, etc.)
4. **Analyze Response**: Generate Bode plots and analyze frequency response
5. **Test with Signals**: Apply filter to various input signals to verify performance

## Filter Characteristics Summary

| Filter Type  | Passband Ripple | Stopband Attenuation | Transition Band | Phase Response |
| ------------ | --------------- | -------------------- | --------------- | -------------- |
| Butterworth  | Flat            | Monotonic            | Moderate        | Good           |
| Chebyshev I  | Ripple          | Sharp                | Narrow          | Fair           |
| Chebyshev II | Flat            | Ripple               | Narrow          | Fair           |
| Elliptic     | Ripple          | Sharp                | Narrowest       | Poor           |
| Bessel       | Flat            | Gradual              | Wide            | Excellent      |

## Applications

- **Audio Processing**: Removing unwanted frequencies from audio signals
- **Communication Systems**: Channel filtering and signal conditioning
- **Biomedical Engineering**: ECG/EEG signal processing
- **Control Systems**: Noise reduction and signal conditioning
- **Instrumentation**: Measurement signal processing

## Learning Objectives

- Understanding different analog filter types and their characteristics
- Hands-on experience with filter design using Python/SciPy
- Frequency domain analysis using Bode plots
- Time domain analysis of filtered signals
- Practical applications of filters in signal processing

## License

This project is for educational purposes.
