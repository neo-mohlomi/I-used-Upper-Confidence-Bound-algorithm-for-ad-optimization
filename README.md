# Advertisement Optimization using Upper Confidence Bound (UCB)
## Project Overview

In digital marketing, businesses often need to determine which advertisement is most likely to attract customer engagement. Continuously showing the same advertisement may overlook potentially better performing alternatives, while testing all advertisements equally can be inefficient and costly.

In this  project I applt the **Upper Confidence Bound (UCB)** Reinforcement Learning algorithm to identify the advertisement that maximizes customer clicks while balancing exploration and exploitation.

I used  dataset containing interactions from **10,000 customers** across **10 different advertisements**, the model learns over time which advertisement generates the highest click-through rate.

---

## Business Problem

Organizations invest significant resources in digital advertising campaigns. Selecting the most effective advertisement is critical for maximizing customer engagement and marketing return on investment (ROI).

The bussines challenge:

* Which advertisement receives the highest number of clicks?
* How can customer interactions be used to improve ad selection over time?
* How can businesses reduce the cost of testing ineffective advertisements?

The UCB algorithm addresses these challenges by intelligently balancing the exploration of different advertisements with the exploitation of the best-performing option.

---

## Dataset

The dataset contains:

* **10,000 customer observations**
* **10 advertisements**
* Binary outcomes:

  * 1 = Customer clicked on the advertisement
  * 0 = Customer did not click on the advertisement

Each row represents a customer interaction and each column represents a different advertisement.

---

## Methodology

### Upper Confidence Bound (UCB)

The UCB algorithm selects advertisements based on:

1. The historical performance of each advertisement.
2. The uncertainty associated with the advertisement's estimated performance.
3. A balance between exploring new options and exploiting known successful advertisements.

The model continuously updates its confidence estimates after each customer interaction.

---

## Results

The model successfully identified **Advertisement 4** as the highest-performing advertisement.

Key observations:

* During the early stages, the model explored multiple advertisements to gather information.
* As more customer interactions were observed, confidence estimates improved.
* From approximately **1000 customer observations onwards**, the algorithm consistently recognized Advertisement 4 as the optimal choice.
* Beyond this point, the model increasingly allocated traffic to Advertisement 4, maximizing overall clicks.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Reinforcement Learning
* Upper Confidence Bound (UCB)

---

## Business Impact

This approach can help organizations:

* Increase click-through rates (CTR)
* Improve advertising efficiency
* Reduce marketing costs
* Make data-driven advertising decisions
* Optimize customer engagement strategies

---

## Future Improvements

* Compare UCB against Thompson Sampling.
* Evaluate performance using real-world advertising data.


---

## Author

Neo Mohlomi

Data Scientist | Machine Learning Enthusiast

GitHub: https://github.com/neo-mohlomi
