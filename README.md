# Galileo Ferraris Contest

Comparing data-driven methodologies for the  multi-physics simulation of traction electrical machines

- <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Presentations/01_motivation.pdf" target="_blank">Motivation
- <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Presentations/02_contest.pdf" target="_blank">Contest
- <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Presentations/03_organization.pdf" target="_blank">Organization
- <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Presentations/04_rules.pdf" target="_blank">Rules
- <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Presentations/05_dataset.pdf" target="_blank">Dataset
- <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Presentations/Advisory_Board.pdf" target="_blank">Advisory Board

Who was <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Presentations/GalFer_Comic.pdf" target="_blank">Galileo Ferraris

## 2025/01/22 - Save the date!!! 2025/02/05, 13:00 CET, GalFer Contest second webinar - <a href="https://polito-it.zoom.us/j/89722170077?pwd=8VXGau7r91mBu6HrkIFd9NJFcUbfqx.1"> Link to Zoom meeting 
Agenda of the webinar:
- Presentation of the interim evaluation results
- Update on data format request
- Discussion
# 2025/01/02 - Interim evaluation assessment

Dear Teams,

We are looking forward to our next steps in the GalFer Contest!

To smooth out possible problems in communication and evaluation, we would like to make an intermediate step comparing and assessing your preliminary results.

Providing the material described below is **not mandatory**, but it can help to check your advancements.

We propose this detailed timeline:

## By January 15th, 2025 

Each team will provide:
*   a short document (maximum two pages IEEE format) where the preliminary results obtained in the "Interpolation" problem (Motor A) on the 3D_1 problem (Torque, Von Mises, Temperature, described in the *Ranking* document) are shortly presented and described.
*   a file, in csv format, containing a set of inputs and the corresponding outputs computed by the surrogate model. The set of points can be either:
    1. an approximation of the Pareto Front obtained by the Team running its own multi-objective optimization procedure;
    2. a set of points (maximum 100) generated in the Motor A feasibility range.

In case of point i. the "official" Contest ranking procedure will be used. In case of point ii. a feedback on the average error on the "true" values evaluated by FEM procedure will be given.

This material will be **"strictly confidential"** and will be used by the Organizing Committee only to assess the status of the Contest Teams.

## By the end of January 2025
The second Contest workshop will be organized and results in an **"anonymous"** form will be presented. In the workshop, possible problems and questions will be discussed.
Each Team will anyway receive a feedback on its results in a **"private"** mail.

The exact date of the workshop will be announced in a few days.

## 2024/11/19 - Save the date!!! 2024/12/11, 13:00 CET, GalFer Contest first webinar <a href="https://polito-it.zoom.us/rec/share/jl5_9bvTBTOyD-7xLD5OduNucjCaGmWuh1xuahruI2dmrGSQ10Bw0DJUWyLTvpYV.Y6oLFlLEGtoLgNoC?startTime=1733918770000">(Link to recording <a href="https://github.com/cadema-PoliTO/GalFer_contest/tree/main/2024_12_11_webinar_presentations">- Link to presentations)
Agenda of the webinar:
1. GalFer Contest introduction: operative details and focus on the contest rules
2. Workflow process creating the datasets
	- Dr. S. Ferrari: magnetic
	- Dr. C. Anerdi: elastostatic
	- Dr. R. Torchio: thermal 
3. Multicriteria evaluation of electric motors
	- Dr. L. Solimene
4. Ranking procedure and Awards
	- Prof. M. Repetto
5. Focus on preliminary teams' work and possible problems emerging in dataset handling: free discussion

## For information on contest rules and awards, please refer to this <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/Ranking_rules/Ranking%26Awards.pdf" target="_blank">link.  

## List of participants (final)

- Altair E-Motor Team, Altair Engineering France, Grenoble, France
- Brainwave Bulided, Shenzhen MSU-BIT University, Shenzhen, China
- CAD Lab Team, University of Pavia, Pavia, Italy
- CREATORs, TU Darmstad - TU Graz - Siemens AG, Darmstad, Germany
- DK-TIC, DAIKIN Industry, Osaka, Japan
- EATUB, TU Berlin, Berlin, Germany
- ECAD, Dongguk University, Soonchunhyuang University and Hanyang University, Seoul, Republic of Korea
- ELECTA, KU Leuven/Energyville, Leuven, Belgium
- Electric System Design Lab, Hosei University, Tokyo, Japan
- e-Machine Learners, University of Wisconsin-Madison, Madison, United States of America
- GTR, University of Lille, Lille, France
- GTB-ULille, University of Lille, Lille, France
- i3@EPFL, Sonceboz SA, Lausanne, Switzerland
- IEML, Amirkabir University of Technology, Tehran, Iran
- Kangaroos, University of Technology Sydney, Sydney, Australia
- LASEteam, The University of British Columbia, Vancouver, Canada
- Machinery warriors, Rajiv Gandhi University of Knowledge Technology, Nuzvid, India
- ManTriS, Politecnico di Torino, Torino, Italy
- McGill MagNets, McGill University, Montreal, Canada
- MELSUR, Mitsubishi Electric Corporation, Hyogo, Japan
- MLotors, Indian Institute of Technology Bhubaneswar, Jatni, India
- MotorAI, Ritsumeikan University, Shiga, Japan
- Motorplus, Motorplus, Teheran, Iran
- Nature-Inspired Computational Intelligence Lab, Brock University, St Catharines, Canada 
- SHIME-PARFAIT, Aoyama Gakuin University, Kyoto, Japan
- The overfitters, Virtual Vehicle Research GmbH, Graz, Austria
- Torque Titans, CG Power and Industrial Solutions Limited, Bhopal, India

### 2024/10/17 - First release of the dataset for Motor "A"

- the dataset containing input and output data on Motor "A" configuration (details in file "04_Rules.pdf" on main page) has been made available to the teams enrolled in the contest;

- the dataset contains 4096 records obtained sampling an 8-dimensional space of degrees of freedom (input) and computing 7 objectives (output);

<div align="center">
	<img width = "50%" src="./Images/tab_input.png">
</div>

- the design objectives are: torque $$(T)$$, torque ripple $$(TR)$$, copper mass $$(M_\mathrm{Cu})$$, magnet mass $$(M_\mathrm{mag})$$, power factor $$(cos(\varphi))$$, Von Mises equivalent stress $$(VM)$$, and maximum temperature on the winding $$(Temp)$$

- results are computed applying the workflow described in file "02_contest.pdf";

- sampling is performed using a Sobol procedure covering the whole hypercube of inputs;

- all 4096 results are reported in datasets, even if some of them should be ruled out due to "unphysical" motor conditions. Advised filtering values are $$VM\leq455 \mathrm{MPa}$$ , $$Temp\leq180 \mathrm{C}$$. If these values are used, a number of 2765 feasible configurations should be obtained;

- in order to produce graphs with a similar setup, it is advised that all the objectives have to be minimised. As maximum torque and power factor are requested, this implies that the minimum of -Torque and $$-(cos(\varphi))$$ are sought;

- four different Pareto optimal subproblems are defined:
    - $$2D_1 \rightarrow$$ $$O_1=-T$$, $$O_2=TR$$
    - $$2D_2 \rightarrow$$ $$O_1=-T$$, $$O_2=VM$$
    - $$2D_3 \rightarrow$$ $$O_1=-T$$, $$O_2=Temp$$
    - $$3D_1 \rightarrow$$ $$O_1=-T$$, $$O_2=VM$$, $$O_3=Temp$$

### Timeline

1. the datasets will be available in **September 2024**;  
2. research groups planning to take part in the Contest are invited to submit their intention to join the Contest using the <a href="https://github.com/cadema-PoliTO/GalFer_contest/blob/main/GalFer_letter_of%20_intent.docx">letter of intent</a> following the template provided by mailing it to the address [**galfercontest@gmail.com**](mailto:galfercontest@gmail.com), at last by **November 15th, 2024**;  
3. sharing of the preliminary results from the research teams and first informal evaluation, by **January 15th, 2025**;
4. publication of the *partial* dataset on the third machine by **January 31st, 2025;**  
5. final results and procedures must be submitted by the research teams by **April 15th, 2025**;  
6. award ceremony will be held in a dedicated *free* workshop during the COMPUMAG 2025 Conference in Naples, **June 22-26, 2025**.


