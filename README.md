## 1. Context of the project

In this project, we are going to analyze data from an experiment about honesty. Oftentimes, we are asked to confirm our honest intentions by signing at the end of a document. For example, in tax returns or insurance policy forms, we are often asked to sign our names under a text that reads something like "I hereby certify that the above statements are true and correct to the best of my knowledge."

However, when individuals sign after lying in the form, they may not feel the need to correct the falsehoods they have reported. In that context, it could be that signing at the beginning rather than at the end of the document would decrease dishonesty, as those who are filling the form would be aware of the ethical requirements before they provide the information in the form.

This intuition has led researchers to partner up with a motorcycle insurance company to run a randomized experiment. In this insurance company (as well as in many others), customers had to report the exact odometer kilometrage¹ in order for the company to adjust the insurance premiums. Note that motorcycles with lower kilometrage are less likely to have issues, and thus will result in a lower insurance premium². Therefore, customers have an incentive to lie, reporting a kilometrage lower than the real value, in order to save money.

In the experiment, two different forms were created: one where the signing was done at the end, and another where the signing was done at the beginning. The insurance company then randomized these forms (i.e., each customer received exactly one form, each with probability 50%) and sent back the data that customers had provided. Some noteworthy details on the experiment are that :

* All customers involved in the experiment already had a contract with the company and were simply renewing it. In the data that the company provided, they also report the odometer kilometrage for their previous contract. Each policy, therefore, contains two contracts: the "updated" contract —where the experiment was conducted— and the "baseline" contract, which was the previous contract customers had with the company.
* A single insurance policy can insure up to 4 distinct motorcycles.

In this project we take the role of the researcher and work analyzing this data!


## 2. Libraries Used
- `pandas`
- `numpy`
- `seaborn`
- `scipy`
- `matplotlib`

## 3. Conclusion 

* We show that more than half of the data were created. First, the updated data were made for the difference between the updated and the baseline odometer to fit a uniform distribution from 0 to 50 000. I also think that the baseline data are not all authentic. It seems that they were duplicated : the values are slightly different (on the last three digits) but they both have the same distribution at large scale.

* As for the honesty experiment, it is hard to obtain certain result with tampered in data. The analysis suggests that signing at the top increases dishonesty, yet, given all the concerns raised above, we can't conclude that this is really the case since the data is **not trustworthy**.
