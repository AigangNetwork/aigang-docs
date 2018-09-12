#################
Insurance
#################
Space for insurance products where a user can choose insurance products.

Insurance products have two main parts:
- Management part: insurance product configuration and description
- Financial Blockchain part: auditable contracts with money movements and policies details.

Successful insurance flow
^^^^^^^^^^^^^^^^^^^^^^^^^^^
* A user selects insurance product.
* Read the details, terms, conditions, contract about the product and if everything acceptable continues further.
* Follow device pairing instructions.
* Our services will check device properties, compare them with contract rules and if the device is valid DRAFT policy with calculated price will be created.
* If the policy details are acceptable User can pay and activate the policy, or delete if it is not acceptable.

Successful claim flow
^^^^^^^^^^^^^^^^^^^^^^^ 
- A user selects active policy.
- Follow device claim instructions
- Our services will check device properties, compare them with contract rules and if the device is claimable change policy status to Claimable
- User Claims his payout and payout will be withdrawn to his wallet. 


More details
^^^^^^^^^^^^^^^^^^^^^^^ 

.. toctree::
   :titlesonly:
   :maxdepth: 2

   architecture
   batteryInsuranceProduct
   links


