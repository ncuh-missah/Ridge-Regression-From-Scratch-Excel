# Ridge-Regression-From-Scratch-Excel
https://img.shields.io/badge/License-MIT-yellow.svg

A step-by-step implementation of ridge regression performed manually in Excel, showing all matrix operations and the effect of the biasing constant (λ).

📊 Overview
This Excel workbook demonstrates ridge regression from first principles using a dataset of cigarette characteristics (tar, nicotine, weight, and carbon monoxide). All calculations are done manually with visible formulas—no built-in regression functions or black-box methods.

🧮 Dataset
The data consists of 25 observations with:

X1: Tar (mg)

X2: Nicotine (mg)

X3: Weight (g)

Y: Carbon Monoxide (mg)

📋 Step-by-Step Process
STEP 1: Standardization
Calculates means and standard deviations for all variables

Standardizes predictors (X) and response (Y) to have mean 0 and variance 1

Shows squared differences and standardization formulas

STEP 2: Matrix Algebra
Constructs the standardized matrices:

X* matrix (predictors)

Y* vector (response)

Computes:

Xᵀ X (correlation-like matrix)

Xᵀ Y (vector)

X* Y* (alternative calculation)

STEP 3: Ridge Point Estimates
Adds the identity matrix × λ (biasing constant)

Demonstrates how the penalty term affects the Xᵀ X matrix

Computes the inverse of (Xᵀ X + λI)

STEP 4: Ridge Parameter Estimates
Calculates standardized ridge coefficients: β̂* = (Xᵀ X + λI)⁻¹ Xᵀ Y

Transforms back to original scale to obtain b₀, b₁, b₂, b₃

🔧 Features
Visible formulas: Every cell shows its calculation—no hidden steps

Adjustable λ: Change the biasing constant to see its effect on coefficients

Educational focus: Designed for learning how ridge regression works under the hood

Complete workflow: From raw data to final coefficient estimates

📁 File Structure
Ridge Regression.xlsx - Main workbook with all calculations

README.md - This documentation

🚀 How to Use
Download the Excel file

Explore each step by clicking on cells to see formulas

Modify the biasing constant (cell B66) to observe how coefficients shrink

Trace calculations from raw data through to final estimates

📚 Key Formulas
Component	Formula
Standardized X	(X - μₓ) / (σₓ × √(n-1))
Xᵀ X	Matrix multiplication of standardized predictors
Ridge solution	β̂* = (X*ᵀ X* + λI)⁻¹ X*ᵀ Y*
Original scale bⱼ	β̂* × (σᵧ / σₓⱼ)
Intercept b₀	Ȳ - b₁X̄₁ - b₂X̄₂ - b₃X̄₃
🎯 Learning Objectives
Understand how ridge regression modifies ordinary least squares

See the effect of the L2 penalty on coefficient estimates

Learn the relationship between standardized and original-scale coefficients

Gain intuition about matrix operations in regression

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

👤 Author
Ncumisa Fakade

🙏 Acknowledgments
Built for educational purposes to demonstrate ridge regression mechanics

Cigarette dataset commonly used in regression textbooks

