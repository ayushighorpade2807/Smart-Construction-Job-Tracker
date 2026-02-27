# Smart-Construction-Job-Tracker

Smart Contractor Matching System
This is a recommendation system for contractors based on AI technology, which can match contractors to job requirements based on skills, location, rating, availability, and type of job.

This is a simulated version of a real-world job allocation system for contractors based on a ranking system using vector similarity and business logic improvements.

# Project Overview

The system:
Processes contractor skills and locations
Converts skills into vectors using PyTorch
Calculates the similarity between job requirements and contractors
Applies location boost, rating factors
Simulates the probability of contractors accepting the job
Calculates the invoice estimate based on job complexity and rating
Offers an interactive interface using Gradio

This project shows the following real-world use cases for the following techniques:

Vector similarity
Feature engineering
Business rule application
Probabilistic simulation
Simple pricing model

# How It Works
1️⃣ Data Preprocessing
Cleans and tokenizes skills and locations
Creates skill-to-index and location-to-index mappings
Converts contractor data into numerical matrices

2️⃣ Vector Representation
Each contractor is represented as a normalized skill vector
Job requirements are converted into a job skill vector
Cosine similarity is used for matching

3️⃣ Matching Logic
Final score considers:
Skill similarity
Location match (boosted factor)
Contractor rating
Availability
Top-K contractors are returned based on ranking.

4️⃣ Acceptance Simulation
Acceptance probability is calculated based on:
Match score
Availability
Controlled probabilistic scaling

5️⃣ Invoice Generation
Invoice pricing depends on:
Base rate
Job complexity
Contractor rating
VAT calculation

# Tech Stack

Python
PyTorch (vector operations & normalization)
Pandas (data handling)
Gradio (interactive UI)
CSV-based dataset
