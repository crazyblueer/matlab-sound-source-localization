Sound Source Localization with a Single Microphone

This project involves sound source localization using only one microphone by employing triangulation based on recorded distances. 
The challenge lies in the fact that there is only a single microphone, and the system must rely on sound amplitude variations over distance. 
The project was implemented using MATLAB Mobile and Python.

Project Overview

The goal of this project is to determine the position of a sound source in a 2D space using a single microphone. The approach is based on:

Data Collection: Recording sound amplitudes at known distances (every 10 cm up to 1 meter).

Analysis: Using the inverse relationship between sound amplitude and distance, the data is analyzed to derive an equation.

Localization: By using triangulation from three recorded positions, the sound source's coordinates are determined.

User Interface: MATLAB Mobile was used to provide a simple user interface for real-time calculations and localization results.

Project Breakdown

1. Data Collection (Python)
Objective: The first step in the project was to collect sound amplitude data at different distances from the microphone. Measurements were taken at 10 cm intervals up to 1 meter.

Method: The data was collected by measuring the amplitude of sound at each position. The relationship between the sound amplitude and distance was expected to follow an inverse pattern, i.e., the sound amplitude decreases as the distance from the microphone increases.

Analysis: The collected data was plotted in Python, and the reciprocal of the distances was used to find the relationship. From this, an equation was derived to estimate the distance based on amplitude.
3. Triangulation (MATLAB Mobile)

Objective: Once the equation relating sound amplitude and distance was derived, MATLAB Mobile was used to implement the localization system.

Approach: The localization process relies on triangulation, where the microphone's position is fixed, and the sound source is estimated based on its distance from multiple positions (3 different positions were chosen for triangulation).

Process: The triangulation algorithm is applied by calculating the intersection point of three circles based on the distances from each microphone position.

4. User Interface (MATLAB Mobile)

Objective: To make the system more interactive and user-friendly, a simple interface was built in MATLAB Mobile.

Functionality: Users can input the distance measurements for the three microphone positions, and the program will calculate and display the estimated coordinates of the sound source.
