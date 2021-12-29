# Autonomous Robots Kalman Filters

The Kalman Filter is an easy topic. However, many tutorials are not easy to understand. Most require extensive mathematical background which makes them difficult to understand. Also, most lack practical numerical examples.

I tried to make practical applications of Kalman filters.

We have to implement 5 matrices go through the following 2 steps.

## Predict  
![alt text](https://github.com/mftnakrsu/AutonomousRobots-Kalman-Filter/blob/main/images/1.png)

## Measure and Update  
![alt text](https://github.com/mftnakrsu/AutonomousRobots-Kalman-Filter/blob/main/images/2.png)

## Matrices

### <code>State Matrix</code> 
    •State Matrix is implemented as x  
    •Matrix defined as [Row x Column]    
    •Define n = number of state    
    •x is size n x 1  
    •n = 4  
### <code>Uncertainty Matrix</code>
    •Populate matrix with initial Uncertainty of each state.
    •Uncertainty Matrix is implemented as P
    •P is size n x n 
    •n = 4
### <code>State Transition Matrix</code>
    •State Transition Matrix is implemented as F.
    •F is size n x n.
    •n=4
    •Populate matrix so that x(t+1)=Fx(t
### <code>Measurement Matrix</code>
    •Measurement Matrix is implemented as H.
    •H is size  n(measure) x n(state)
    •n(measure) = 2
    •n(state)=4
###   <code>Measurement Uncertainty</code> 
    •R is size n x n
    •n(measure)=2
    
 You can see result of algorithm <code>"kalmanfilter.py"</code> :  
[![IMAGE ALT TEXT HERE](https://github.com/mftnakrsu/AutonomousRobots-Kalman-Filter/blob/main/images/3.png)](https://www.youtube.com/embed/sAvfaQpiEv8)
