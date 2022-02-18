# Optimizing_Human_Robot_Collaboration_Frontiers
A paper based on these experiments has been published in Frontiers in Robotics and AI. It is titled "General Framework for the Optimization of the Human-Robot Collaboration Decision-Making Process Through the Ability to Change Performance Metrics"<a href="#note1" id="note1ref"><sup>1</sup></a>, and it is written by Mélodie DANIEL<a href="#note2" id="note2ref"><sup>2</sup></a>, Sébastien LENGAGNE<a href="#note2" id="note2ref"><sup>2</sup></a>, Juan CORRALES<a href="#note3" id="note3ref"><sup>3</sup></a>, and Youcef MEZOUAR<a href="#note2" id="note2ref"><sup>2</sup></a>.

We have conducted experiments in simulation on a construction game to prove the optimization of Human-Robot Collaboration (HRC). To do this, we optimize the HRC by considering performance metrics (time completion and the number of human errors) in the reward values of the utility function of the decision-making process. 

Experiment conditions:
- The human can choose one among three actions : A<sub>h,g</sub> with a probability P(A<sub>h,g</sub>) = I<sub>1</sub>, A<sub>h,w</sub> with a probability P(A<sub>h,w</sub>) = I<sub>2</sub>, and  A<sub>h,b</sub> with a probability P(A<sub>h,b</sub>) = I<sub>3</sub> = 1-(I<sub>1</sub> + I<sub>2</sub>).
- We tested for I<sub>1</sub> =(0:0.1:1) and I<sub>2</sub> =(0:0.1:1) except for I<sub>1</sub> = I<sub>2</sub> = 0.
- We tested the ratio between the time taking by the human do make an action t<sub>A<sub>h</sub></sub> and the one taken by the robot t<sub>A<sub>r</sub></sub> for 1/1, 1/1.5, 1/2, 1/3, 1/4, 1/5.
- We tested the number of cubes required to solve the puzzle for 2, 3, 4, and 5.
- We conducted 10000 simulations to calculate the average time and the standard variation. 

Experiment parameters:
experiment parameters are written in the file "experiment_parameters.txt".

Experiment resulting data:
For each experiment, we got the following data:
- A Table ("results.txt") that contains the average time (in seconds) calculated, among 10000 simulations, for the C<sub>3</sub> (our utility function) and the one for C<sub>1</sub> (state-of-the-art utility function). We calculated the percentage improvement of the time for C<sub>3</sub> in comparison to C<sub>1</sub>. We calculated the percentage of the number of human errors reduction between the predicted probability that the human will make errors (I<sub>3</sub>) and the measured one. It contains also the standard variation of the time, its maximum value, and the minimum one for the C<sub>3</sub> and the C<sub>1</sub>.
- "Figure 1": a 2D figure that presents the difference between the average output time (in seconds) obtained by cases 1 and 3 over 10000 simulations.
- "Figure 2": a 3D figure that presents the difference between the average output time (in seconds) obtained by cases 1 and 3 over 10000 simulations.
- "Figure 3": a 2D figure that presents the percentage of the time improvement.
- "Figure 4": a 3D figure that presents the percentage of the time improvement.
- "Figure 5": a 2D figure that presents the percentage of the reduction of the number of human errors.
- "Figure 6": a 3D figure that presents the percentage of the reduction of the number of human errors.


<a id="note1" href="#note1ref"><sup>1</sup></a>Full citation: Zakaria, M. H. D., Lengagne, S., Ramón, J. A. C., & Mezouar, Y. (2021). General Framework for the Optimization of the Human-Robot Collaboration Decision-Making Process Through the Ability to Change Performance Metrics. Frontiers in Robotics and AI, 8. 

<a id="note2" href="#note2ref"><sup>2</sup></a>CNRS, Clermont Auvergne INP, Institut Pascal,  Université Clermont Auvergne, Clermont-Ferrand, France.  
<a id="note3" href="#note3ref"><sup>3</sup></a>Centro Singular de Investigación en Tecnoloxías Intelixentes (CiTIUS), Universidade de Santiago de Compostela, Santiago de Compostela, España.

