## Overview

This repository contains raw data and visualization tools for CISBAT paper "Enhancing urban digital twin interfaces to support thermal comfort planning."

## About BEAM Urban Digital Twin platform

[BEAM](https://www.coolnus-beam.sg/) (Baselining, Evaluating, Action, Monitoring) is a campus-wide microclimate assessment initiative for urban heat island mitigation at the National University of Singapore. The BEAM team has developed an urban digital twin for monitoring and testing mitigation strategies, and this paper aims to understand the usability challenges that exists within the platform.

### Dataset Integration

BEAM covers the entire NUS campus and integrates the following datasets:

| Dataset Type           | Details                                                  |
| ---------------------- | -------------------------------------------------------- |
| Weather Stations       | 40 total (32 ground, 8 rooftop)                          |
| Meteorological Towers  | 3 towers                                                 |
| Thermal Cameras        | 6 cameras                                                |
| Microclimate Maps      | Current year and averages of past years                  |
| Tree Census            | Complete campus inventory                                |
| Temperature Sensors    | 12 sensors under different greenery conditions           |
| Street View Images     | Segmented 360° imagery                                   |
| Building Energy Models | 362 campus buildings                                     |
| Thermal Walks          | 9 walks with climate sensor data and participant surveys |
| Simulations            | ENVI-Met simulations for different mitigation scenarios  |

## Usability Studies

This study recruited ten participants, five based in the US and five in Singapore, through
personal referrals, LinkedIn outreach, and email correspondence. Each participant completed a 60-minute interview that included five components: background questions, exploration phase, guided tasks, survey, and open-ended discussion. You can find a transcript of the conversations and descriptions of user actions during the exploration phase, guided tasks, and open-ended discussion in [Exploration_And_Guided_Tasks.csv](/Exploration_And_Guided_Tasks.csv).

### Guided Tasks

The specific questions asked during guided tasks were:

<ol>
  <li>
    Basic Navigation
    <ol type="a">
      <li>Please click on one weather station and navigate to the outdoor thermal comfort data. What was the most uncomfortable times of the day?</li>
      <li>Switch between the other tabs (air temperature, humidity, solar irradiation), do you notice any relationships? For example, which parameter has the strongest correlation to discomfort? And which one the weakest?</li>
    </ol>
  </li>
    <li>
    Thermal Vulnerability
    <ol type="a">
      <li>Please open current microclimate map, can you describe what you are seeing?</li>
      <li>Compare the daytime microclimate maps across different months. Can you identify some areas that are most prone to heat stress? How might the underlying urban morphology or landscape factors contribute to these conditions.</li>
    </ol>
  </li>
      <li>
    Community Comfort Analysis
    <ol type="a">
      <li>Open the thermal walk survey data by going to collaborative studies > thermal walk. This is a study where people were asked to answer thermal comfort surveys along a route, there was also objective data collected for temperature/ views. Play a walk, and click open one of the watch icons. What information does the modal contain?</li>
      <li>Do you see some patterns between person comfort levels and objective measurements or 360 views? </li>
    </ol>
  </li>
</ol>

### Survey

Users completed a two-part survey on Google Form, with the first part being the User Experience Questionnaire (UEQ) and the second part on questions adapted from Gemini Principles. The results are in [SurveyResponses.csv](/SurveyResponses.csv).

The questions for UEQ can be found in [UEQ_English.pdf](/UEQ_English.pdf). And the eight questions that were adapted from Gemini Principles are as follow:

<ol>
<li>Do you think a tool like this delivers public benefit?</li>
<li>Does it provide value?</li>
<li>Does it provide insights into the built environment?</li>
<li>Do you find this platform secure?</li>
<li>How would you rate the openness of data for this tool?</li>
<li>Do you think this platform can be adapted for your workflow?</li>
<li>Is there a clear ownership of this platform? That is, do you know who curates the data and manages this ecosystem?</li>
<li>Do you think this platform has the ability to adapt and develop as technology and society evolves?</li>
</ol>

### Open-ended discussion

In addition to giving general feedback, participants were asked to rank these four categories in importance with regards to what they value in a digital platform for their work:

Data Integration & Comprehensiveness

- breadth of data sources
- frequency of data updates
- integration of real-time and historical data
- ability to cross-reference multiple data types

User Interface & Navigation

- intuitiveness of platform layout
- speed of platform performance
- color coding and visual hierarchy
- ease of switching between different data layers
- comprehensibility of complex data representations

Analytical Tools & Capabilities

- scenario modeling capabilities
- predictive analysis features
- comparative analysis tools
- ability to generate reports or exportable insights

Community & Stakeholder Engagement

- visualization of community feedback
- tools for participatory planning
- accessibility for non-technical stakeholders
- mechanism for incorporating qualitative data

### Results and Visualization

Analysis on quantitative data and visualization can be found in [Visualization.ipynb](/Visualization.ipynb).
