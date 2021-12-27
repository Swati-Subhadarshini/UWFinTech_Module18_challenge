# UWFinTech_Module18_challenge
Assignment on creating Blockchain

This assignment is based on building a blockchain-based ledger system, complete with a user-friendly web interface. This ledger should allow partner banks to conduct financial transactions (that is, to transfer money between senders and receivers) and to verify the integrity of the data in the ledger.

## Technologies Used

Leveraging python version 3.9.6
Git Bash CLI
Visual Studio

## Libraries Used

import streamlit as st
from dataclasses import dataclass
from typing import Any, List
import datetime as datetime
import pandas as pd
import hashlib


## Instructions:
### The steps for this Challenge are divided into the following sections:


The following updates to the provided Python file for this Challenge:

The steps for this Challenge are divided into the following sections:

Create a Record Data Class

Modify the Existing Block Data Class to Store Record Data

Add Relevant User Inputs to the Streamlit Interface

Test the PyChain Ledger by Storing Records

### Step 1: 

Create a Record Data Class
Define a new Python data class named Record. Give this new class a formalized data structure that consists of the sender, receiver, and amount attributes. To do so, complete the following steps:

Define a new class named Record.

Add the @dataclass decorator immediately before the Record class definition.

Add an attribute named sender of type str.

Add an attribute named receiver of type str.

Add an attribute named amount of type float.

Note that you’ll use this new Record class as the data type of your record attribute in the next section.

### Step 2: 

Modify the Existing Block Data Class to Store Record Data
Rename the data attribute in your Block class to record, and then set it to use an instance of the new Record class that you created in the previous section. To do so, complete the following steps:

In the Block class, rename the data attribute to record.

Set the data type of the record attribute to Record.

### Step 3: 

Add Relevant User Inputs to the Streamlit Interface
Code additional input areas for the user interface of your Streamlit application. Create these input areas to capture the sender, receiver, and amount for each transaction that you’ll store in the Block record. To do so, complete the following steps:

Add an input area where you can get a value for sender from the user.

Add an input area where you can get a value for receiver from the user.

Add an input area where you can get a value for amount from the user.

As part of the Add Block button functionality, update new_block so that Block consists of an attribute named record, which is set equal to a Record that contains the sender, receiver, and amount values. The updated Blockshould also include the attributes for creator_id and prev_hash.

### Step 4: 

Test the PyChain Ledger by Storing Records
Test your complete PyChain ledger and user interface by running your Streamlit application and storing some mined blocks in your PyChain ledger. Then test the blockchain validation process by using your PyChain ledger. To do so, complete the following steps:

In the terminal, navigate to the project folder where you've coded the Challenge.

In the terminal, run the Streamlit application by using streamlit run pychain.py.

Enter values for the sender, receiver, and amount, and then click the Add Block button. Do this several times to store several blocks in the ledger.
Verify the block contents and hashes in the Streamlit drop-down menu.
Test the blockchain validation process by using the web interface.

### Screenshot of Streamlit Webpage
![Streamlit Webpage Screenshot1](http://localhost:8888/files/UWFinTech_Module18_challenge/Images/Screenshot1.png?_xsrf=2%7C9c94a471%7Cc3ce1085c0ed7f44b9db9f78453f052f%7C1640580942)
![Streamlit Webpage Screenshot2](http://localhost:8888/files/UWFinTech_Module18_challenge/Images/Screenshot2.png?_xsrf=2%7C9c94a471%7Cc3ce1085c0ed7f44b9db9f78453f052f%7C1640580942)
![Streamlit Webpage Screenshot3](http://localhost:8888/files/UWFinTech_Module18_challenge/Images/Screenshot2.png?_xsrf=2%7C9c94a471%7Cc3ce1085c0ed7f44b9db9f78453f052f%7C1640580942)


## Contributors

This project is designed by Swati Subhadarshini 
Emaid id: sereneswati@gmail.com
LinkedIn link: https://www.linkedin.com/in/swati-subhadarshini