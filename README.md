# Two Dimensional Histogram Filter
 Robot Localization - 2D Histogram Filter
The Histogram Filter is the most straightforward solution to represent continuous beliefs. We simply divide 𝑑𝑜𝑚(𝑥𝑡) into 𝑛 disjoint bins 𝑏0,…,𝑏𝑛−1 such that ∪𝑖𝑏𝑖=𝑑𝑜𝑚(𝑥𝑡). Then we define a new state 𝑥′𝑡∈{0,…,𝑛−1} where 𝑥′𝑡=𝑖 if and only if 𝑥𝑡∈𝑏𝑖. Since 𝑥′𝑡 has a discrete, finite state space, we can use the discrete Bayes Filter to calculate 𝑏𝑒𝑙(𝑥′𝑡).

𝑏𝑒𝑙(𝑥′𝑡) is an approximation for 𝑏𝑒𝑙(𝑥𝑡) then: For each bin 𝑏𝑖, it gives us the probability that 𝑥𝑡 is in that bin. The more bins we use, the more accurate the approximation becomes, with the downside of increasing computational complexity.

The disadvantage of the Histogram Filter is that we are not able to tell the probability of each possible state. We are only able to tell the probability that the state is in a certain region of the state space. to oversome this disadvantage, we could use a very fine-grained decomposition of the state space, but this drastically increases the computational complexity.

## Localization Reference
- [x] [Histogram Filter](https://github.com/tooth2/HistogramFilter)
- [ ] Kalman Filter
- [x] [Particle Filter](https://github.com/tooth2/Robot_Particle_Fillter)
- [x] [Extended Kalman Filter](https://github.com/tooth2/Extended-Kalman-Filter)
- [x] [Unscented Kalman Filter](https://github.com/tooth2/Unscented-Kalman-Filter)
- [x] [SLAM](https://github.com/tooth2/Landmark-Detection-Tracking-SLAM)
