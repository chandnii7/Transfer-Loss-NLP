# Transfer Loss Across Domain

Program to analyze tranfer loss across domains using example of books and electronics.

### Dataset:
1. Source Domain: Books
   * number of positive reviews =  1000
   * number of negative reviews =  1000
   * source domain training set vector:  (2000, 4500)

2. Target Domain: Electronics
   * number of positive reviews =  1000
   * number of negative reviews =  1000
   * target domain training set vector:  (1600, 4500)
   * target domain test set vector:  (400, 4500)
<br />

### Result:
1. Direct Transfer:
   * Training a logistic regression classifier on the Electronics training dataset.
   * Evaluating it on the Electronics test dataset.
<br />
   <img src="https://github.com/chandnii7/TransferLossNLP/blob/main/Data/img1.jpg" height="300" width="400"/>
<br />

2. Cross-domain Transfer:
   * Training a logistic regression classifier on the Books training dataset. 
   * Evaluating it on the Electronics test dataset.
<br />
   <img src="https://github.com/chandnii7/TransferLossNLP/blob/main/Data/img2.jpg" height="300" width="400"/>
<br />

3. Transfer Loss Across Domains:
   * LOSS = direct_transfer_accuracy - cross_domain_transfer_accuracy
   * LOSS = 0.39
