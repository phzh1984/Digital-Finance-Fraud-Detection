# Digital-Finance-Fraud-Detection

Context

There is a shortage of publicly available financial services datasets, particularly in the domain of emerging mobile money transactions. The sensitive nature of financial transactions often results in the unavailability of public datasets. As a result, researchers face challenges in conducting research, especially in the area of fraud detection. To address this gap, a synthetic dataset was generated using a simulator called PaySim.

PaySim utilizes aggregated data from private financial logs to create a synthetic dataset mimicking typical transaction operations. It introduces malicious behaviors to assess the effectiveness of fraud detection methods.

Overview

This dataset simulates mobile money transactions based on real data. It serves as a valuable resource for studying and developing fraud detection methods in financial services.

Content

This synthetic dataset is a scaled-down version (1/4) of real transactions extracted from one month of financial logs of a mobile money service implemented in an African country. 

The original logs were provided by a multinational company offering mobile financial services across 14 countries worldwide.

Note: Transactions detected as fraudulent are canceled. Therefore, the columns: oldbalanceOrg, newbalanceOrig, oldbalanceDest, and newbalanceDest should not be used for fraud detection.

Headers

step: Represents a unit of time in the real world. Each step equals one hour (Total steps: 744, simulating 30 days).

type: Categories of transactions: CASH-IN, CASH-OUT, DEBIT, PAYMENT, and TRANSFER.

amount: Transaction amount in local currency.

nameOrig: Initiator of the transaction.

oldbalanceOrg: Initial balance before the transaction.

newbalanceOrig: New balance after the transaction.

nameDest: Recipient of the transaction.

oldbalanceDest: Recipient's initial balance before the transaction. (No information available for merchant-initiated accounts)

newbalanceDest: Recipient's new balance after the transaction. (No information available for merchant-initiated accounts)

isFraud: Indicates transactions made by fraudulent agents in the simulation, aiming to control customer accounts, transfer funds, and cash out.

isFlaggedFraud: Flags illegal attempts where the transaction amount exceeds 200,000.
