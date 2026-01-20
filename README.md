# NumPy Universal Functions - Mechanical Engineering Assignment

## 📋 Instructions

Complete all 10 functions in `mechanical_problems.py` using NumPy universal functions (ufuncs).

### ⚠️ Requirements
- ✅ Use NumPy ufuncs (np.sin, np.cos, np.sqrt, np.power, etc.)
- ✅ Work with arrays - **NO LOOPS allowed!**
- ✅ Return NumPy arrays unless specified otherwise
- ✅ All angles input/output in degrees (convert internally to radians)

## 🚀 Setup
```bash
pip install -r requirements.txt
```

## 📝 Questions (100 points total)

### Q1: Von Mises Stress (10 points)
Calculate von Mises stress from principal stresses.
- **Formula:** σ_vm = √(σ₁² - σ₁σ₂ + σ₂²)
- **Input:** Arrays of principal stresses (MPa)
- **Output:** Array of von Mises stress (MPa)

### Q2: Projectile Trajectory (10 points)
Calculate x, y coordinates for projectile motion at multiple angles.
- **Equations:** x = v₀cos(θ)t, y = v₀sin(θ)t - ½gt²
- **Input:** Initial velocity, angles array, time array
- **Output:** Tuple of (x_positions, y_positions) as 2D arrays

### Q3: Force Resultant (10 points)
Calculate magnitude and direction of resultant force vectors.
- **Input:** x and y force components (N)
- **Output:** Tuple of (magnitude, angle_degrees)

### Q4: Thermal Expansion (10 points)
Calculate length change due to thermal expansion.
- **Formula:** ΔL = α × L₀ × ΔT
- **Input:** Original lengths, thermal coefficients, temperature changes
- **Output:** Tuple of (delta_L, L_final) in mm

### Q5: Angular Velocity Conversion (10 points)
Convert RPM to rad/s and calculate angular displacement after 5 seconds.
- **Conversion:** ω = RPM × (2π/60)
- **Input:** RPM values
- **Output:** Tuple of (omega in rad/s, theta in rad after 5s)

### Q6: Beam Deflection (10 points)
Calculate deflection of simply supported beam with uniform load.
- **Formula:** y = (w/24EI) × x × (L³ - 2Lx² + x³)
- **Input:** Position array, beam length, load, Young's modulus, moment of inertia
- **Output:** Deflection array (negative for downward)

### Q7: Velocity Components (10 points)
Resolve velocities into x and y components.
- **Input:** Velocity magnitudes, angles (degrees)
- **Output:** Tuple of (vx, vy) components

### Q8: Power to Torque (10 points)
Calculate torque from power and angular velocity.
- **Formula:** τ = P / ω
- **Input:** Power (W), angular velocity (rad/s)
- **Output:** Torque (N⋅m)

### Q9: Spring System (10 points)
Calculate spring force and potential energy.
- **Formulas:** F = -kx, U = ½kx²
- **Input:** Spring constants, displacements
- **Output:** Tuple of (force in N, potential_energy in J)

### Q10: Damped Oscillation (10 points)
Calculate displacement for damped harmonic motion.
- **Formula:** x(t) = A × e^(-bt) × cos(ωt)
- **Input:** Amplitude, damping coefficient, angular frequency, time array
- **Output:** Displacement array

## 📤 Submission

1. Complete all functions in `mechanical_problems.py`
2. Commit and push:
```bash
   git add mechanical_problems.py
   git commit -m "Complete assignment"
   git push
```
3. GitHub Actions will automatically test your code
4. Check the **"Actions"** tab to see results

## 📊 Grading

- Each question: 10 points
- Total: 100 points
- Autograding runs on every push
- You'll see ✅ or ❌ for each test group

## 💡 Tips

- Read docstrings carefully
- Test with simple inputs first
- Use `np.` functions, not loops
- Pay attention to array shapes (especially Q2)
- Convert degrees to radians for trig functions

## ❌ Common Errors

- Using Python loops instead of ufuncs
- Forgetting degree/radian conversions
- Wrong output array shapes
- Returning lists instead of arrays
- Not using broadcasting

Good luck! 🎯
