# Fuzzy-logic-implementation-without-library
Fuzzy logic implementation without library to select top 5 machine shop from 100 machine shop

***Project Description***

This project is a final assignment for the Artificial Intelligence course. The goal is to develop a Fuzzy Logic Inference system to select the top 5 machine shop from a dataset of 100 machine shop without using any external fuzzy logic libraries. The program reads input from a file named bengkel.xlsx and outputs the best 5 machine shop with information on their service quality, pricing, and a suitability score derived from the defuzzification process.

***Features***
- Read machine shop data from bengkel.xlsx.
- Evaluate each machine shop based on service quality and pricing using a custom Fuzzy Logic implementation.
- Select and display the top 5 machine shop with their IDs, service quality, pricing information, and suitability scores.

***Table of Contents***
- Installation
- Usage
- Input Data Format
- Fuzzy Logic System
  - Fuzzification
  - Inference
  - Defuzzification
- Output

***Installation***
1. Clone the repository:
git clone https://github.com/chaald/fuzzy-logic-implementation-without-library.git
2. Navigate to the project directory:
cd fuzzy-logic-implementation-without-library
3. Install the required dependencies:
pip install -r requirements.txt

***Usage***
1. Place your bengkel.xlsx file in the project directory.
2. Run the main program:
python main.py
3. The program will output the top 5 machine shop with their IDs, service quality, pricing, and suitability scores.

***Input Data Format***

The bengkel.xlsx file should have the following columns:
- id: The unique identifier for each machine shop.
- servis: The quality of service provided by the machine shop.
- harga: The cost of services offered by the machine shop.

***Fuzzy Logic System***
1. Fuzzification
Fuzzification is the process of converting crisp input values into fuzzy sets. This project defines fuzzy membership functions for service quality and pricing.
2. Inference
Inference uses predefined fuzzy rules to evaluate the input values. The fuzzy rules are stored in a dictionary and the inference process calculates the degree of membership for each rule.
3. Defuzzification
Defuzzification converts the fuzzy output into a crisp suitability score. This project uses the centroid method to calculate the final suitability score.

***Output***

The program displays the top 5 machine shop with the following information:
- id: machine shop ID.
- servis: Quality of service provided.
- harga: Cost of services offered.
- skor kelayakan: The defuzzified score representing the suitability of the machine shop.
The final ranked list of machine shop is saved to peringkat.xls.

