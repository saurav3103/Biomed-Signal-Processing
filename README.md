# Biomed-Signal-Processing

<h3>Biomedical Signal Denoising Using Spectral Subtraction</h3>

This project focuses on simulating and denoising ECG signals by applying classical signal processing techniques. The objective is to replicate common noise conditions in biomedical signals and effectively clean them for improved readability and analysis.

---

## 🔍 Overview

Electrocardiogram (ECG) signals are often affected by noise from various sources such as baseline wander, powerline interference, and white Gaussian noise. This notebook provides a complete pipeline for:

- Generating synthetic ECG signals
- Adding realistic noise
- Filtering and denoising the signal using:
  - Butterworth Bandpass Filter
  - Spectral Subtraction

---

## 🧰 Tools and Libraries

The following Python libraries are used in the project:

- `neurokit2` – for simulating ECG signals
- `numpy`, `scipy` – for signal processing
- `matplotlib` – for visualization
- `scikit-learn` – for normalization

---

## 🚀 Getting Started

### Installation

Install the required packages using pip:

```bash
pip install neurokit2 numpy scipy matplotlib scikit-learn
```

### Running the Code

Simply open the `Biomed_Project.ipynb` file in Jupyter Notebook or any compatible IDE and execute the cells in order.

---

## ⚙️ Core Functions

- **`generate_ecg_signal(duration, fs)`**  
  Simulates an ECG waveform using `neurokit2`.

- **`add_realistic_noise(ecg, fs)`**  
  Introduces baseline wander, 50 Hz powerline noise, and white Gaussian noise.

- **`bandpass_filter(data, lowcut, highcut, fs)`**  
  Filters the noisy ECG using a Butterworth bandpass filter.

- **`spectral_subtraction(signal, noise)`**  
  Reduces residual noise using a basic spectral subtraction approach.

---

## 📈 Visual Output

The notebook provides visualizations at each stage:
- Original clean ECG signal
- ECG with added noise
- Filtered ECG after bandpass
- Final denoised ECG after spectral subtraction
 ![image](https://github.com/user-attachments/assets/1a4dd779-4733-4779-95b9-7aee920bd80b)


These plots allow you to compare the signal quality before and after denoising.

---

## 📌 Future Scope

- Test with real ECG datasets (e.g., MIT-BIH Arrhythmia Database)
- Apply advanced denoising methods like wavelet transforms or adaptive filtering
- Package the pipeline for real-time or batch processing

---

## 🤝 Contributions

If you find this project useful or have suggestions for improvement, feel free to open an issue or submit a pull request. Feedback is always appreciated.

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
