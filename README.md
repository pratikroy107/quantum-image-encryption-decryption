# 🧠🔐 Quantum-Inspired Chaotic Neural Network (QCaNN) for Image Encryption & Decryption

This project implements a **Quantum-Inspired Chaotic Neural Network (QCaNN)** system to encrypt and decrypt grayscale images using a multi-stage pipeline based on **quantum image principles**, **chaotic dynamics**, **neural networks**, and **probabilistic decoding**.

It simulates quantum computation behavior in a classical system for robust and nonlinear image security.

---

## 📌 Key Features

- ✅ Quantum-style grayscale image representation (NEQR-inspired)
- 🧠 Neural encryption using QCaNN and chaotic sine maps
- 🔄 Multi-layer security: diffusion, quantum gate simulation, Lorenz chaos, 5D hyperchaotic shuffling
- 🔐 Decryption using CNOT logic, probabilistic measurement, and inverse modeling
- 🧪 Supports both RGB and Grayscale image with variable dimensions

---

## 🔄 Encryption Workflow (Step-by-Step)

### 🔹 Step 1: Quantum Image Generation

- The grayscale image is converted into a quantum-inspired representation.
- Uses NEQR-like structure to map pixel intensity and position into qubit-like states.

---

### 🔹 Step 2: QCaNN – Quantum-Inspired Chaotic Neural Network

- A 3-layer chaotic neural network simulates quantum superposition and transformation:
  \[
  a_1 = \text{sigmoid}(w_1 \cdot x),\quad
  a_2 = \text{sigmoid}(w_2 \cdot a_1),\quad
  a_3 = \text{sigmoid}(w_3 \cdot a_2)
  \]
- Chaotic weights \( w_1, w_2, w_3 \) are initialized using a **sine map**:
  \[
  x_{n+1} = r \cdot \sin(\pi x_n)
  \]

---

### 🔹 Step 3: Pixel Diffusion

- Pixel intensities are further modified using chaotic diffusion mechanisms.
- Typical operations: XOR with chaotic sequences, modulo transformation, key mixing.

---

### 🔹 Step 4: Quantum Rotation Simulation

- Rotation gates (Rx, Ry, Rz) are simulated on the quantum-inspired pixel vectors.
- This introduces quantum-like transformations in pixel value distributions.

---

### 🔹 Step 5: Lorenz Chaotic Pixel Shuffling

- Uses Lorenz system to shuffle pixel positions (row and column wise).
- Lorenz equations:
  \[
  \frac{dx}{dt} = \sigma(y - x),\quad
  \frac{dy}{dt} = x(\rho - z) - y,\quad
  \frac{dz}{dt} = xy - \beta z
  \]

---

### 🔹 Step 6: 5D Hyper-Chaotic System (5D-HCS)

- Applies a five-dimensional chaotic system for final encryption.
- Adds an extra nonlinear, deeply randomized transformation layer over the image.

---

### 🔹 Step 7: Final Encrypted Image

- The final image is highly random, secure, and visually unrecognizable.
- All layers are dependent on initial keys and weights—making brute-force decryption infeasible.

---

## 🔐 Decryption Workflow

Decryption is performed by applying the **inverse** of each encryption stage using chaos-based keys and quantum-inspired logic.

---

### 🔹 Step 1: CNOT Gate with 5D-HCS and Encrypted Image

- A simulated **CNOT gate** operation is performed between:
  - Encrypted image (target)
  - 5D-HCS chaotic matrix (control)
- This cancels out the hyperchaotic scrambling and retrieves the **Lorenz-shuffled image**.

---

### 🔹 Step 2: Inverse Quantum Rotation

- The quantum-rotated image is passed through **inverse gate simulations** to cancel previous transformations.
- Effectively reverses Rx, Ry, Rz rotations applied during encryption.

---

### 🔹 Step 3: CNOT Gate with QCaNN Image

- Another **CNOT operation** is applied between:
  - Output of previous step (target)
  - QCaNN output (control)
- This operation retrieves the original **quantum image representation**.

---

### 🔹 Step 4: Measurement and Probabilistic-Based Decoding

- A simulated quantum **measurement** is applied to the quantum image.
- Probabilistic encoding (e.g., based on qubit amplitudes) is decoded to obtain the **original classical grayscale image**.
- Measurement collapses the quantum-like state back to pixel values.


---

## 🛡️ Security Strength

### 🔐 Why This Scheme is Strong:

- **Multi-Layer Defense**: Combines multiple non-linear transformations including chaotic neural encoding, quantum gate simulation, and high-dimensional chaotic scrambling.
- **Chaotic Sensitivity**: Even minor changes in initial conditions or key values lead to drastically different encrypted outputs—demonstrating high key sensitivity.
- **Quantum-Inspired Behavior**: Uses simulated quantum measurement, entanglement-like dependency, and probabilistic decoding, making classical cryptanalysis difficult.
- **Statistical Robustness**: Output histograms show uniform distribution, and NIST randomness tests can be passed with high success rates.
- **No Redundancy**: Pixel correlation, structural similarity, and spatial relationships are thoroughly destroyed in the encrypted image.

---

